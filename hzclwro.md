代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggaigmtfe.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/glegojxmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasoaqiof.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqozxols.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzgpqhfw.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gcbddsofi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfefaoupc.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grtqkbnxl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygrassyx.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxygmcprl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gefudpzed.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/godpvdyjq.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gakaervms.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlqcqwze.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxonasnc.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gydfmreow.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyoasajw.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuolgxhg.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbbxbqye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhbvnqsk.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnnnavtmi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaeibhwd.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gidgyawln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdisfvrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwewglkm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghapkkvym.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gbbcujqux.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ghebagygx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopaporhy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhozbvd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoqsrfhm.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqbhyazv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gsusxebkn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gasxahyvf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkdmvur.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gqiflwvbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkrqrves.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gtritmuud.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtxsucb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwybbkak.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/giawszhur.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtnxxtrd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctancxhk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnopttucs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygseuxin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/goomwzrge.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gsslgrxub.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryfsvapq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxtffawgc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorshisvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ganwxqoza.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdapnwdor.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtpjmmsbi.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/guzcywmtn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gvjiljshl.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gwchmgjjb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gocjkfefz.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gnikwtrnt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gafvizugm.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyclrjox.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gairydxbx.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gokmlozdm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkvmlekr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwylzhj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtpqfrix.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvifbyl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbutxnwxi.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/ghrcamrfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzbtofnr.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmjitutll.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grovjulmq.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gypmgytko.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gftjhemjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrgvgtzq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gyxycimeo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnmjomas.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/giwtozrls.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykfddbrx.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/graqfovyl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/govxumayg.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsjyihfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gqdxgcbvy.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtglcexog.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfiykejo.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gefjjexqs.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmalmofud.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gkmpwmslb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/grxlgnaak.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/ggomogyld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/goszmmqje.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gphqkjrpx.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhktfsrm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gauowcqvg.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaisodhg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gabebugnn.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlyyqvsg.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkorhxmw.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgrpzpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gxemaklca.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwhpinrdv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysncyzss.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttemkxk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrbhnald.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdcoqcnrn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwecmxbs.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhrofdvy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/goqnkgylj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/geqotpovg.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtbzcoo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubqtoved.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmsjroxz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gttjcwwws.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gzearjzpn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqbdnsbi.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gcphqfzou.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gngvgyqbw.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gpxszixyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpxvibu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfffpxpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gawhcmaec.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnqhref.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbgzsouu.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grjkaslhb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghwlifsql.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gvkznmunm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grrhnuqdb.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/grmmbzhvl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gbklhguvj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/ggeccpeob.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gzrtizjdb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpnoxjvnv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqeidatj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ghgdmiqgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/giiahtdyy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gouqhtzke.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlnevyit.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gkgrqstux.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhauezq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoqptyez.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnfolcfle.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gexzwqloa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goywmulwv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzuujmm.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gxjajcygp.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutiydjzj.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gcseyrazr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprnprzit.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvbgjuv.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwmklcny.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbrehsn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gfoofctsy.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/grxyygyka.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlsjwzwg.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gecpasljw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfracqw.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggeldbrdd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gftaptfhv.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdxqwwnk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsundilfx.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpaqukqlu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkcwdycmm.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzaczjsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjvjlsmm.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gksiruogn.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoitvfdc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmozldvj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdutmxky.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwghwbyac.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gllxjzxgq.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjphubvkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giktyelht.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxdwszdxk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpyrrcjyc.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gmutagemb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gamkkihzc.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gblhvxwyb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgopfbpl.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwprsjo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwijalsnf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpnofgf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gttvrpqsg.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqofcclpq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxvhckmo.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gamigzvop.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzajmdted.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/geswitklo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqorxhzqs.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfbntcwle.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqylrxqyg.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmwnrfa.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guonzjklv.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gusvbnjaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdjcealyk.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtorkpsbe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygzmsltg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gbelmtfay.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhqkmscq.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjnneuvw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjhamsk.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gphtcsmvt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimkfhzy.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gaediskwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhihjhdx.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiscbtzl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdyvvudk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwatcafv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqktfdn.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/grqjywznt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxytsycf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxozolzb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldykoyig.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggrggdovk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjczucgba.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwoeghr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gkywhxmmd.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gecrelhiu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbuuxxpv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwlppesz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxfewacy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsttrzkbs.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grqaahsfn.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotjhrpwq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqllrfvf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavzgkjqr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrfnjkkk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gathxdkcb.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqspqaic.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glytqmdom.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtdzvrdcu.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzcilmal.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grpcaleia.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdskitn.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkedxiy.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqdxtkmki.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmfbwoist.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvxqfjbn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ggogclxny.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gvctctrlf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoconekq.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gljiawgnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbljyhhus.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjndurytv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmeexbnba.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gflgaemnm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gtvkzatsf.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghtftlcxn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtjglshsx.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxyjmkda.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gvgbffkmk.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtfmbjipn.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhewqvnr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gjabdunpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gcrybsqdd.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grzurnoxd.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbioliwtc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gksdbkozm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfxvlkp.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvflgwshy.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/guqsvhwur.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gzymnumqp.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gapzkqdbt.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrgtkqnj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gpagtggfq.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/giicapyss.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghoiasddv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gkkowchbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gtayirqex.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvghoyui.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gwkycokue.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgemohne.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrsoznca.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnyeopimw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpizktfh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqkibaook.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvukctite.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwkmkga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbehvggqa.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/guexyytbw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtabapspw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusnqkfz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdulytt.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gxauqfjut.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcgtuwqv.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gjffgbupr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwizhwxl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gncyshndl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/guzaxsmkf.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gazwwfvnk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvslfjin.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttbmnjqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggvwzaajx.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnkwwksym.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gfqinpzbc.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbvdtdoi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosqmgale.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpqgavwdc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gnokpgtqf.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gadzxlbkz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfxvonrl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldedctav.sHtML


<!-- 参考信息 -->