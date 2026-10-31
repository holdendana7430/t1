代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://dy.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wn.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://dk.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fl.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://sf.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zy.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zo.nszjky.cn

[Q15] 查询全部
来源：http://kj.jianghongdianzi.cn

SELECT * FROM users;
来源：http://bs.gzmigu.cn

[Q16] 查询指定列
来源：http://vd.nszjky.cn

SELECT id, name FROM users;
来源：http://gv.szsharing.cn

[Q17] 条件查询
来源：http://nh.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wr.panjiajie.cn

[Q18] 模糊匹配
来源：http://ba.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mk.jctech888.com.cn

[Q19] 范围查询
来源：http://dx.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gs.yuntaijiaju.cn

[Q20] IN 列表
来源：http://hl.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xa.521024.cn

[Q21] 空值判断
来源：http://dp.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kn.nszjky.cn

[Q22] 排序
来源：http://mf.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ej.wgjwhj.cn

[Q23] 分页
来源：http://mj.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nz.jianghongdianzi.cn

[Q24] 去重
来源：http://qq.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ql.shxzukj.cn

[Q25] 只取前 N 条
来源：http://ue.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uz.chemitech.net.cn

[Q26] 计数
来源：http://ci.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://rk.nicolike.cn

[Q27] 条件计数
来源：http://gi.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ne.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://xa.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ns.nszjky.cn

[Q29] 最大最小值
来源：http://ek.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uw.chemitech.net.cn

[Q30] 分组统计
来源：http://mu.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ra.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ka.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ke.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://fi.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lu.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rv.haigaiapp.cn

[Q33] 多列分组
来源：http://ao.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qh.colortex.cn

[Q34] 每组取第一条
来源：http://iy.521024.cn

SELECT * FROM (
来源：http://ln.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aw.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ld.shxzukj.cn

[Q35] 内连接
来源：http://zy.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uq.muxihuayi.cn

[Q36] 左连接
来源：http://at.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wv.gzmigu.cn

[Q37] 右连接
来源：http://jw.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vu.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ub.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pw.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://om.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ce.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qv.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yu.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sg.szxytkj.cn

[Q41] 多表连接
来源：http://pz.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vc.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://cn.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://rl.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://nv.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://qc.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ip.nicolike.cn

[Q43] 标量子查询
来源：http://ed.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uo.shxzukj.cn

[Q44] IN 子查询
来源：http://wp.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nf.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://ee.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ju.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oq.yuexingan06.cn

[Q47] 与平均值比较
来源：http://uh.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jx.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://lx.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://co.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://io.chemitech.net.cn

[Q49] 更新单行
来源：http://hd.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ls.hahajie.cn

[Q50] 批量更新
来源：http://os.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jz.yuexingan06.cn

[Q51] 用子查询更新
来源：http://va.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://si.hnjuh.cn

[Q52] 删除指定行
来源：http://iw.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://xi.nicolike.cn

[Q53] 按条件删除
来源：http://kl.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ll.asd995.cn

[Q54] 清空表
来源：http://mz.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://uu.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://gk.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ts.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://cq.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qu.nszjky.cn

[Q57] 行号
来源：http://rf.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lb.bookmarksfly.cn

[Q58] 累计求和
来源：http://nu.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sb.shxzukj.cn

[Q59] 分组内累计
来源：http://rt.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hk.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://od.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fs.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kt.gzmigu.cn

[Q61] 移动平均
来源：http://bb.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nh.szxytkj.cn

[Q62] 分组占比
来源：http://zu.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xv.521024.cn

[Q63] 开启事务
来源：http://gv.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://re.hahajie.cn

[Q64] 提交事务
来源：http://vl.bookmarksfly.cn

COMMIT;
来源：http://dw.colortex.cn

[Q65] 回滚事务
来源：http://tq.yuntaijiaju.cn

ROLLBACK;
来源：http://pl.chemitech.net.cn

[Q66] 行锁查询
来源：http://rd.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sj.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://yf.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://su.lnxyls.cn

[Q68] 保存点
来源：http://id.shxzukj.cn

SAVEPOINT sp1;
来源：http://ff.hahajie.cn

ROLLBACK TO sp1;
来源：http://uy.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://gh.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://te.hnjuh.cn

[Q70] 更新统计信息
来源：http://ev.hnjuh.cn

ANALYZE TABLE users;
来源：http://xw.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://tj.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xh.szsharing.cn

[Q72] 查看索引
来源：http://fp.hnjuh.cn

SHOW INDEX FROM users;
来源：http://lh.huixiangedu.cn

[Q73] 查看表状态
来源：http://rd.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nz.newstarts.cn

[Q74] 强制使用索引
来源：http://ak.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yx.hahajie.cn

[Q75] 日期格式化
来源：http://hj.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uv.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qv.jctech888.com.cn

[Q76] 按天统计
来源：http://qv.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eg.colortex.cn

[Q77] 时间加减
来源：http://hm.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qt.shxzukj.cn

[Q78] 当前时间
来源：http://mq.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mi.muxihuayi.cn

[Q79] 字符串拼接
来源：http://xg.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ic.hnjuh.cn

[Q80] 字符串截取
来源：http://so.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oz.newstarts.cn

[Q81] 字符串替换
来源：http://my.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iu.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://bg.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ah.gzmigu.cn

[Q83] 大小写转换
来源：http://wx.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mu.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://le.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://ki.521024.cn

[Q85] 数值取整
来源：http://ko.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gl.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://gb.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lj.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ct.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pf.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://qf.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cf.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://za.nicolike.cn

[Q89] 判断表是否存在
来源：http://xz.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ex.hnjuh.cn

[Q90] 生成序号列
来源：http://ut.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://by.szxytkj.cn

================================================================================
来源：http://hh.bjjhwx.cn

R. Bash 专题
来源：http://iv.jianghongdianzi.cn

================================================================================
来源：http://ye.lnxyls.cn

[R01] shebang 与严格模式
来源：http://je.521024.cn

#!/usr/bin/env bash
来源：http://hv.shxzukj.cn

set -euo pipefail
来源：http://ab.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://dn.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://tp.wgjwhj.cn

[R03] 只读变量
来源：http://jk.jianghongdianzi.cn

readonly PI=3.14
来源：http://rh.muxihuayi.cn

[R04] 位置参数
来源：http://ps.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rd.521024.cn

[R05] 参数默认值
来源：http://ee.bjjhwx.cn

name="${1:-default}"
来源：http://ue.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ff.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gx.huixinmuqiang.cn

[R07] if 判断文件
来源：http://uh.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ww.colortex.cn

[R08] 数值比较
来源：http://gj.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://df.521024.cn

[R09] 字符串比较
来源：http://kp.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ac.gzmigu.cn

[R10] 正则匹配
来源：http://db.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vj.panjiajie.cn

[R11] case 多分支
来源：http://vt.nicolike.cn

case "$1" in
来源：http://gr.yuexingan06.cn

start) echo "启动" ;;
来源：http://lr.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ze.521024.cn

*)     echo "未知命令" ;;
来源：http://wn.panjiajie.cn

esac
来源：http://sy.shtwfgs.cn

[R12] for 遍历文件
来源：http://sv.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://yk.gzmigu.cn

[R13] for 计数循环
来源：http://oi.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://el.jctech888.com.cn

[R14] C 风格 for
来源：http://zp.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yr.hahajie.cn

[R15] while 逐行读文件
来源：http://wd.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://li.newstarts.cn

[R16] until 等待条件
来源：http://fp.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ne.nszjky.cn

[R17] 数组定义与取值
来源：http://zv.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rs.bjjhwx.cn

[R18] 遍历数组
来源：http://hc.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wu.szxytkj.cn

[R19] 数组长度
来源：http://bf.newstarts.cn

echo "${#arr[@]}"
来源：http://mc.9csxet.cn

[R20] 关联数组（字典）
来源：http://gb.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xy.yuexingan06.cn

[R21] 字符串长度
来源：http://re.huixinmuqiang.cn

echo "${#s}"
来源：http://ga.jctech888.com.cn

[R22] 截取子串
来源：http://cn.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://dl.gzmigu.cn

[R23] 字符串替换
来源：http://ie.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mw.yuexingan06.cn

[R24] 大小写转换
来源：http://vn.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ko.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://rv.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mb.newstarts.cn

[R26] 命令替换
来源：http://ko.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://uo.asd995.cn

[R27] 算术展开
来源：http://nk.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://lm.chemitech.net.cn

[R28] 浮点运算
来源：http://sr.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://lu.jctech888.com.cn

[R29] 定义函数
来源：http://ze.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bf.wgjwhj.cn

[R30] 函数返回状态码
来源：http://uq.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://bb.muxihuayi.cn

[R31] 局部变量
来源：http://ra.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://gs.shtwfgs.cn

[R32] 参数个数校验
来源：http://ae.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qd.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://qr.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wl.shxzukj.cn

[R34] 退出时清理
来源：http://ck.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qy.szsharing.cn

[R35] 后台执行并等待
来源：http://iv.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jx.asd995.cn

[R36] 并发执行多个任务
来源：http://iv.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://me.colortex.cn

[R37] 把输出赋给变量
来源：http://uz.wgjwhj.cn

files=$(ls -1)
来源：http://nq.shxzskj.cn

[R38] 管道串联
来源：http://dx.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://pg.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://mk.huanxung.cn

cmd > out.log 2>&1
来源：http://en.newstarts.cn

[R40] 追加写日志
来源：http://aq.asd995.cn

echo "log" >> out.log
来源：http://dg.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://zc.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://kh.haigaiapp.cn

[R42] 输入重定向
来源：http://nk.nszjky.cn

wc -l < a.txt
来源：http://rj.szxytkj.cn

[R43] 按名字查找文件
来源：http://jv.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://ci.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://fu.shxzukj.cn

find . -mtime -7 -type f
来源：http://tf.colortex.cn

[R45] 批量删除
来源：http://or.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://xd.lnxyls.cn

[R46] 递归替换文件内容
来源：http://fq.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gf.lnxyls.cn

[R47] sed 单行替换
来源：http://yq.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oa.hahajie.cn

[R48] awk 取指定列
来源：http://if.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://iq.shxzukj.cn

[R49] awk 带条件
来源：http://qv.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vu.bookmarksfly.cn

[R50] awk 求和
来源：http://eq.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vd.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://gh.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://te.huanxung.cn

[R52] 统计行数
来源：http://en.asd995.cn

wc -l a.txt
来源：http://ys.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://mx.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xs.szsharing.cn

[R54] 比较两个文件
来源：http://ia.shxzukj.cn

diff a.txt b.txt
来源：http://fw.shtwfgs.cn

[R55] 压缩与解压
来源：http://ju.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://av.asd995.cn

[R56] 远程拷贝
来源：http://de.9csxet.cn

scp file user@host:/path/
来源：http://fy.huixiangedu.cn

[R57] 远程执行命令
来源：http://xw.nicolike.cn

ssh user@host 'uptime'
来源：http://rk.nszjky.cn

[R58] 下载文件
来源：http://co.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bb.szsharing.cn

[R59] 发 POST JSON
来源：http://ly.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ne.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://jc.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sf.hnjuh.cn

[R61] 磁盘占用
来源：http://ft.szxytkj.cn


<!-- 参考信息 -->