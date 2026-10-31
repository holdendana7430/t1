代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ve.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gs.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://sn.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gu.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://jo.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vz.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xu.wgjwhj.cn

[Q15] 查询全部
来源：http://ma.huixinmuqiang.cn

SELECT * FROM users;
来源：http://oe.haigaiapp.cn

[Q16] 查询指定列
来源：http://ej.wgjwhj.cn

SELECT id, name FROM users;
来源：http://qe.szsharing.cn

[Q17] 条件查询
来源：http://dw.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qw.panjiajie.cn

[Q18] 模糊匹配
来源：http://pi.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bc.hnjuh.cn

[Q19] 范围查询
来源：http://xf.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nz.shtwfgs.cn

[Q20] IN 列表
来源：http://ck.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fl.wgjwhj.cn

[Q21] 空值判断
来源：http://wq.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ym.nszjky.cn

[Q22] 排序
来源：http://tu.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mj.9csxet.cn

[Q23] 分页
来源：http://tw.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uf.shxzukj.cn

[Q24] 去重
来源：http://hf.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://wl.hahajie.cn

[Q25] 只取前 N 条
来源：http://ij.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ko.panjiajie.cn

[Q26] 计数
来源：http://bm.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://jh.haigaiapp.cn

[Q27] 条件计数
来源：http://wn.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zk.chemitech.net.cn

[Q28] 求和与平均
来源：http://uf.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rb.bjjhwx.cn

[Q29] 最大最小值
来源：http://qj.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mi.huanxung.cn

[Q30] 分组统计
来源：http://jk.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fd.hahajie.cn

[Q31] 分组后过滤
来源：http://xl.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ec.huanxung.cn

[Q32] 分组拼接字符串
来源：http://mo.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lh.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rj.panjiajie.cn

[Q33] 多列分组
来源：http://gm.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wa.hahajie.cn

[Q34] 每组取第一条
来源：http://vd.yuntaijiaju.cn

SELECT * FROM (
来源：http://gu.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pn.lnxyls.cn

) t WHERE rn = 1;
来源：http://nc.jianghongdianzi.cn

[Q35] 内连接
来源：http://qg.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hd.hahajie.cn

[Q36] 左连接
来源：http://wt.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://td.asd995.cn

[Q37] 右连接
来源：http://fm.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yl.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://is.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yo.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://ug.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yk.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eh.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ht.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vi.jianghongdianzi.cn

[Q41] 多表连接
来源：http://kl.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sg.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://lw.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://yp.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://jh.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://oj.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pl.asd995.cn

[Q43] 标量子查询
来源：http://dn.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pm.hnjuh.cn

[Q44] IN 子查询
来源：http://km.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ik.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://qu.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sy.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gi.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dn.nicolike.cn

[Q47] 与平均值比较
来源：http://ju.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ot.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://eo.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rk.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://sm.nszjky.cn

[Q49] 更新单行
来源：http://ek.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pk.yuntaijiaju.cn

[Q50] 批量更新
来源：http://bj.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jb.shxzskj.cn

[Q51] 用子查询更新
来源：http://dv.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yr.newstarts.cn

[Q52] 删除指定行
来源：http://xh.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://xv.9csxet.cn

[Q53] 按条件删除
来源：http://yh.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zr.panjiajie.cn

[Q54] 清空表
来源：http://do.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://jt.newstarts.cn

[Q55] 排名（并列占位）
来源：http://nd.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ng.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ke.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ga.shxzskj.cn

[Q57] 行号
来源：http://mg.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xh.jctech888.com.cn

[Q58] 累计求和
来源：http://fd.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fh.yuexingan06.cn

[Q59] 分组内累计
来源：http://io.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cn.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://al.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://va.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rp.nicolike.cn

[Q61] 移动平均
来源：http://se.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ws.szsharing.cn

[Q62] 分组占比
来源：http://us.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ws.lnxyls.cn

[Q63] 开启事务
来源：http://uo.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lm.bookmarksfly.cn

[Q64] 提交事务
来源：http://tb.jianghongdianzi.cn

COMMIT;
来源：http://kg.shtwfgs.cn

[Q65] 回滚事务
来源：http://dq.wgjwhj.cn

ROLLBACK;
来源：http://lz.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://cn.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://el.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://rb.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vz.wgjwhj.cn

[Q68] 保存点
来源：http://ny.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://de.huanxung.cn

ROLLBACK TO sp1;
来源：http://lx.nszjky.cn

[Q69] 查看执行计划
来源：http://eo.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pd.colortex.cn

[Q70] 更新统计信息
来源：http://ff.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://az.haigaiapp.cn

[Q71] 查看建表语句
来源：http://ot.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://em.nicolike.cn

[Q72] 查看索引
来源：http://gj.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://oi.nszjky.cn

[Q73] 查看表状态
来源：http://iz.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wt.newstarts.cn

[Q74] 强制使用索引
来源：http://ht.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xc.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://rs.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ie.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dr.shxzukj.cn

[Q76] 按天统计
来源：http://yp.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bl.nicolike.cn

[Q77] 时间加减
来源：http://pb.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qg.asd995.cn

[Q78] 当前时间
来源：http://ox.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cj.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://xx.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ja.gzmigu.cn

[Q80] 字符串截取
来源：http://vh.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wf.gzmigu.cn

[Q81] 字符串替换
来源：http://gh.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hv.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://ok.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lh.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://oy.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qz.hnjuh.cn

[Q84] 去除首尾空格
来源：http://hs.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://he.szsharing.cn

[Q85] 数值取整
来源：http://bq.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fz.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://ms.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hh.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://zu.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://md.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://mn.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gq.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zd.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://tp.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pn.nszjky.cn

[Q90] 生成序号列
来源：http://iw.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iy.muxihuayi.cn

================================================================================
来源：http://qh.bjjhwx.cn

R. Bash 专题
来源：http://ui.haigaiapp.cn

================================================================================
来源：http://py.nicolike.cn

[R01] shebang 与严格模式
来源：http://ri.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://zp.hnjuh.cn

set -euo pipefail
来源：http://du.hnjuh.cn

[R02] 变量赋值与使用
来源：http://iq.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ne.wgjwhj.cn

[R03] 只读变量
来源：http://cc.gzmigu.cn

readonly PI=3.14
来源：http://mc.gzmigu.cn

[R04] 位置参数
来源：http://jt.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ju.hnjuh.cn

[R05] 参数默认值
来源：http://jf.shxzukj.cn

name="${1:-default}"
来源：http://ii.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://xf.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xc.yuntaijiaju.cn

[R07] if 判断文件
来源：http://of.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xp.colortex.cn

[R08] 数值比较
来源：http://tg.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ym.hahajie.cn

[R09] 字符串比较
来源：http://nn.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oi.jianghongdianzi.cn

[R10] 正则匹配
来源：http://op.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vf.shxzskj.cn

[R11] case 多分支
来源：http://ol.asd995.cn

case "$1" in
来源：http://yp.nicolike.cn

start) echo "启动" ;;
来源：http://ow.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://bu.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://vh.9csxet.cn

esac
来源：http://bz.hnjuh.cn

[R12] for 遍历文件
来源：http://ya.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://et.hnjuh.cn

[R13] for 计数循环
来源：http://rl.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://yt.521024.cn

[R14] C 风格 for
来源：http://lg.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vw.szsharing.cn

[R15] while 逐行读文件
来源：http://cf.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ny.bookmarksfly.cn

[R16] until 等待条件
来源：http://ko.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yx.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://ik.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ei.lnxyls.cn

[R18] 遍历数组
来源：http://ld.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oo.hahajie.cn

[R19] 数组长度
来源：http://dm.hahajie.cn

echo "${#arr[@]}"
来源：http://gr.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://cl.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jc.colortex.cn

[R21] 字符串长度
来源：http://lc.bjjhwx.cn

echo "${#s}"
来源：http://ty.newstarts.cn

[R22] 截取子串
来源：http://yt.521024.cn

echo "${s:0:5}"
来源：http://cs.9csxet.cn

[R23] 字符串替换
来源：http://ru.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jp.shxzukj.cn

[R24] 大小写转换
来源：http://sk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ni.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://rq.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ce.jctech888.com.cn

[R26] 命令替换
来源：http://nj.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ov.huixiangedu.cn

[R27] 算术展开
来源：http://rx.nicolike.cn

echo $((1 + 2 * 3))
来源：http://fl.haigaiapp.cn

[R28] 浮点运算
来源：http://xy.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://rt.bjjhwx.cn

[R29] 定义函数
来源：http://iq.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qc.nszjky.cn

[R30] 函数返回状态码
来源：http://lb.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://gc.chemitech.net.cn

[R31] 局部变量
来源：http://jc.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://pd.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ar.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mx.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://zg.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pd.muxihuayi.cn

[R34] 退出时清理
来源：http://zs.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ry.lnxyls.cn

[R35] 后台执行并等待
来源：http://gz.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fb.panjiajie.cn

[R36] 并发执行多个任务
来源：http://pb.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wi.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://ab.colortex.cn

files=$(ls -1)
来源：http://xx.hahajie.cn

[R38] 管道串联
来源：http://od.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://pp.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://hn.haigaiapp.cn

cmd > out.log 2>&1
来源：http://kr.nicolike.cn

[R40] 追加写日志
来源：http://nj.hahajie.cn

echo "log" >> out.log
来源：http://nn.9csxet.cn

[R41] 丢弃输出
来源：http://xq.asd995.cn

cmd >/dev/null 2>&1
来源：http://lc.gzmigu.cn

[R42] 输入重定向
来源：http://sy.huixinmuqiang.cn

wc -l < a.txt
来源：http://fc.haigaiapp.cn

[R43] 按名字查找文件
来源：http://iy.521024.cn

find . -name "*.log" -type f
来源：http://vs.lnxyls.cn

[R44] 按修改时间查找
来源：http://lu.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ix.nszjky.cn

[R45] 批量删除
来源：http://fw.asd995.cn

find . -name "*.tmp" -delete
来源：http://ee.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://zh.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uo.9csxet.cn

[R47] sed 单行替换
来源：http://fp.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yk.szxytkj.cn

[R48] awk 取指定列
来源：http://am.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://if.colortex.cn

[R49] awk 带条件
来源：http://aw.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ag.shtwfgs.cn

[R50] awk 求和
来源：http://wi.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bd.huixiangedu.cn

[R51] 排序去重取前几
来源：http://yn.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sx.bookmarksfly.cn

[R52] 统计行数
来源：http://nx.jctech888.com.cn

wc -l a.txt
来源：http://xi.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://la.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://no.gzmigu.cn

[R54] 比较两个文件
来源：http://qm.haigaiapp.cn

diff a.txt b.txt
来源：http://ah.shxzukj.cn

[R55] 压缩与解压
来源：http://sb.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xy.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://jo.chemitech.net.cn

scp file user@host:/path/
来源：http://sj.bjjhwx.cn

[R57] 远程执行命令
来源：http://nv.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ze.bjjhwx.cn

[R58] 下载文件
来源：http://um.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hr.chemitech.net.cn

[R59] 发 POST JSON
来源：http://mu.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kr.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://by.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gs.asd995.cn

[R61] 磁盘占用
来源：http://he.jctech888.com.cn


<!-- 参考信息 -->