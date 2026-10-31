代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://vf.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fa.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://hf.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nd.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://iw.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vn.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ur.chemitech.net.cn

[Q15] 查询全部
来源：http://ws.bjjhwx.cn

SELECT * FROM users;
来源：http://jd.gzmigu.cn

[Q16] 查询指定列
来源：http://cd.huanxung.cn

SELECT id, name FROM users;
来源：http://fa.yuntaijiaju.cn

[Q17] 条件查询
来源：http://mn.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ys.shxzskj.cn

[Q18] 模糊匹配
来源：http://ni.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zh.gzmigu.cn

[Q19] 范围查询
来源：http://ku.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zm.hnjuh.cn

[Q20] IN 列表
来源：http://lw.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lx.shxzukj.cn

[Q21] 空值判断
来源：http://hm.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://er.newstarts.cn

[Q22] 排序
来源：http://tm.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ln.shtwfgs.cn

[Q23] 分页
来源：http://sp.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ni.muxihuayi.cn

[Q24] 去重
来源：http://gb.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://wg.huanxung.cn

[Q25] 只取前 N 条
来源：http://jx.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dz.hahajie.cn

[Q26] 计数
来源：http://oz.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://nx.gzmigu.cn

[Q27] 条件计数
来源：http://uj.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://of.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rr.yuexingan06.cn

[Q29] 最大最小值
来源：http://wz.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fb.gzmigu.cn

[Q30] 分组统计
来源：http://pc.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ie.huanxung.cn

[Q31] 分组后过滤
来源：http://aw.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vc.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://cq.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hg.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://de.yuexingan06.cn

[Q33] 多列分组
来源：http://fx.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vx.yuexingan06.cn

[Q34] 每组取第一条
来源：http://re.szxytkj.cn

SELECT * FROM (
来源：http://ne.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://av.chemitech.net.cn

) t WHERE rn = 1;
来源：http://pi.haigaiapp.cn

[Q35] 内连接
来源：http://fq.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://va.jianghongdianzi.cn

[Q36] 左连接
来源：http://gk.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ld.jctech888.com.cn

[Q37] 右连接
来源：http://ng.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eq.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tj.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nq.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://ir.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rm.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ul.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vl.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wz.colortex.cn

[Q41] 多表连接
来源：http://gw.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yb.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://em.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://pi.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://tk.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://fv.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kl.asd995.cn

[Q43] 标量子查询
来源：http://oe.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qq.hahajie.cn

[Q44] IN 子查询
来源：http://vj.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ut.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ff.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uz.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cp.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ov.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://jf.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gj.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://pa.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wq.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ex.lnxyls.cn

[Q49] 更新单行
来源：http://ex.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://up.jctech888.com.cn

[Q50] 批量更新
来源：http://gt.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aq.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://dj.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://um.wgjwhj.cn

[Q52] 删除指定行
来源：http://lg.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://jt.colortex.cn

[Q53] 按条件删除
来源：http://uz.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rk.hnjuh.cn

[Q54] 清空表
来源：http://sq.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://pf.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://sa.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sf.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://qs.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sl.chemitech.net.cn

[Q57] 行号
来源：http://yp.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fh.haigaiapp.cn

[Q58] 累计求和
来源：http://zt.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qb.nszjky.cn

[Q59] 分组内累计
来源：http://bi.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lr.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://ti.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lm.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qi.szsharing.cn

[Q61] 移动平均
来源：http://qi.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://du.shxzskj.cn

[Q62] 分组占比
来源：http://zc.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ru.szxytkj.cn

[Q63] 开启事务
来源：http://tz.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fr.huixinmuqiang.cn

[Q64] 提交事务
来源：http://qz.szsharing.cn

COMMIT;
来源：http://nd.shxzskj.cn

[Q65] 回滚事务
来源：http://ce.panjiajie.cn

ROLLBACK;
来源：http://es.lnxyls.cn

[Q66] 行锁查询
来源：http://tz.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gn.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://dl.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ft.shtwfgs.cn

[Q68] 保存点
来源：http://tn.gzmigu.cn

SAVEPOINT sp1;
来源：http://gc.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://mk.muxihuayi.cn

[Q69] 查看执行计划
来源：http://ig.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gh.panjiajie.cn

[Q70] 更新统计信息
来源：http://jp.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://au.hahajie.cn

[Q71] 查看建表语句
来源：http://lg.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ld.huixiangedu.cn

[Q72] 查看索引
来源：http://ly.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://up.szsharing.cn

[Q73] 查看表状态
来源：http://qr.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vz.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://em.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uf.huanxung.cn

[Q75] 日期格式化
来源：http://oe.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hl.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xt.9csxet.cn

[Q76] 按天统计
来源：http://ys.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sn.shxzskj.cn

[Q77] 时间加减
来源：http://dr.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wv.lnxyls.cn

[Q78] 当前时间
来源：http://bo.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ts.shtwfgs.cn

[Q79] 字符串拼接
来源：http://cy.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lt.yuexingan06.cn

[Q80] 字符串截取
来源：http://tu.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nb.shxzukj.cn

[Q81] 字符串替换
来源：http://lp.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gb.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://hn.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fe.bookmarksfly.cn

[Q83] 大小写转换
来源：http://ed.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://od.asd995.cn

[Q84] 去除首尾空格
来源：http://uh.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://tj.nszjky.cn

[Q85] 数值取整
来源：http://am.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yj.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://za.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wl.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://fp.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xo.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://ki.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qz.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ot.9csxet.cn

[Q89] 判断表是否存在
来源：http://bb.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qq.jctech888.com.cn

[Q90] 生成序号列
来源：http://vm.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gc.szsharing.cn

================================================================================
来源：http://nn.wgjwhj.cn

R. Bash 专题
来源：http://mi.haigaiapp.cn

================================================================================
来源：http://nf.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://zy.haigaiapp.cn

#!/usr/bin/env bash
来源：http://wl.panjiajie.cn

set -euo pipefail
来源：http://go.hnjuh.cn

[R02] 变量赋值与使用
来源：http://kk.nszjky.cn

name="Tom"; echo "$name"
来源：http://cl.bookmarksfly.cn

[R03] 只读变量
来源：http://jp.huixiangedu.cn

readonly PI=3.14
来源：http://ed.gzmigu.cn

[R04] 位置参数
来源：http://iv.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://is.szxytkj.cn

[R05] 参数默认值
来源：http://pk.shxzukj.cn

name="${1:-default}"
来源：http://tp.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://dw.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hu.hnjuh.cn

[R07] if 判断文件
来源：http://nt.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pw.chemitech.net.cn

[R08] 数值比较
来源：http://il.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ie.muxihuayi.cn

[R09] 字符串比较
来源：http://ic.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lh.hnjuh.cn

[R10] 正则匹配
来源：http://bc.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iw.nszjky.cn

[R11] case 多分支
来源：http://vr.newstarts.cn

case "$1" in
来源：http://vq.newstarts.cn

start) echo "启动" ;;
来源：http://kd.hahajie.cn

stop)  echo "停止" ;;
来源：http://sw.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://hp.asd995.cn

esac
来源：http://me.panjiajie.cn

[R12] for 遍历文件
来源：http://ut.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://sw.yuexingan06.cn

[R13] for 计数循环
来源：http://kt.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://ln.szsharing.cn

[R14] C 风格 for
来源：http://eu.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ax.panjiajie.cn

[R15] while 逐行读文件
来源：http://dv.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sx.nicolike.cn

[R16] until 等待条件
来源：http://pz.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://we.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ju.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nk.huixiangedu.cn

[R18] 遍历数组
来源：http://zb.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fc.panjiajie.cn

[R19] 数组长度
来源：http://wd.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://nu.9csxet.cn

[R20] 关联数组（字典）
来源：http://cc.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rd.asd995.cn

[R21] 字符串长度
来源：http://zw.haigaiapp.cn

echo "${#s}"
来源：http://qo.huixinmuqiang.cn

[R22] 截取子串
来源：http://kg.szsharing.cn

echo "${s:0:5}"
来源：http://mx.521024.cn

[R23] 字符串替换
来源：http://wr.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tt.haigaiapp.cn

[R24] 大小写转换
来源：http://ow.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tl.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://nm.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jo.shtwfgs.cn

[R26] 命令替换
来源：http://yk.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://nf.haigaiapp.cn

[R27] 算术展开
来源：http://rq.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ff.muxihuayi.cn

[R28] 浮点运算
来源：http://iw.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://dq.jianghongdianzi.cn

[R29] 定义函数
来源：http://cq.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://de.haigaiapp.cn

[R30] 函数返回状态码
来源：http://ut.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://vv.nicolike.cn

[R31] 局部变量
来源：http://ec.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://jh.lnxyls.cn

[R32] 参数个数校验
来源：http://tb.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rt.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://ed.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lv.wgjwhj.cn

[R34] 退出时清理
来源：http://gh.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pl.nszjky.cn

[R35] 后台执行并等待
来源：http://pp.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dk.nszjky.cn

[R36] 并发执行多个任务
来源：http://xs.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ce.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://zf.newstarts.cn

files=$(ls -1)
来源：http://tb.521024.cn

[R38] 管道串联
来源：http://yy.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://lh.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ef.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://hd.panjiajie.cn

[R40] 追加写日志
来源：http://jp.szsharing.cn

echo "log" >> out.log
来源：http://pf.shxzskj.cn

[R41] 丢弃输出
来源：http://sj.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://hb.szsharing.cn

[R42] 输入重定向
来源：http://rw.chemitech.net.cn

wc -l < a.txt
来源：http://ps.asd995.cn

[R43] 按名字查找文件
来源：http://wf.521024.cn

find . -name "*.log" -type f
来源：http://yg.huixiangedu.cn

[R44] 按修改时间查找
来源：http://cg.hahajie.cn

find . -mtime -7 -type f
来源：http://rm.bjjhwx.cn

[R45] 批量删除
来源：http://yq.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://vq.shxzskj.cn

[R46] 递归替换文件内容
来源：http://kl.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wx.lnxyls.cn

[R47] sed 单行替换
来源：http://nt.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ef.haigaiapp.cn

[R48] awk 取指定列
来源：http://ew.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://se.chemitech.net.cn

[R49] awk 带条件
来源：http://av.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bp.asd995.cn

[R50] awk 求和
来源：http://lj.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zf.chemitech.net.cn

[R51] 排序去重取前几
来源：http://rf.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bf.huixiangedu.cn

[R52] 统计行数
来源：http://jc.colortex.cn

wc -l a.txt
来源：http://mw.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://oz.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dd.521024.cn

[R54] 比较两个文件
来源：http://cy.hnjuh.cn

diff a.txt b.txt
来源：http://kz.colortex.cn

[R55] 压缩与解压
来源：http://be.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mp.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://gr.9csxet.cn

scp file user@host:/path/
来源：http://fh.shxzukj.cn

[R57] 远程执行命令
来源：http://dk.panjiajie.cn

ssh user@host 'uptime'
来源：http://vn.colortex.cn

[R58] 下载文件
来源：http://ol.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://le.asd995.cn

[R59] 发 POST JSON
来源：http://ww.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rg.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://rq.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xv.bjjhwx.cn

[R61] 磁盘占用
来源：http://le.hnjuh.cn


<!-- 参考信息 -->