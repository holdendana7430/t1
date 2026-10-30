代发 wailian999

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwrvxjfmd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gilqtepzf.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyeicxgjn.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ghzlmarpk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gexwekwkx.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/ggeplcaxl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gpxucpcbp.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gevlxfvmj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gwghjyvpu.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfvacoosw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gouuymcgl.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/ghicytvyh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gascewcjo.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gulxonstj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gixakvgsb.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gjswccldy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gsvflgoyp.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/guynajogi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcpndjyhx.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gevtjpujl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gdsqpfhdl.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/ghjejuuhn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbkwxtcqx.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gcbsuimob.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmuydiyjp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gjuxrsgfa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtvutmmkp.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/ggeuwoxmo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gityoudth.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/ghflmujtw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/goskxcwnt.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gqelxnxjv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gtckjqkak.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gbrqbgqwz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gldeskbeh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gahpbnbzp.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gurvsobsq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gmlgdmkfv.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gatlkgikm.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gzkpslwpn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ggsleutyt.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gxadawvba.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gdvxecamx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbqvwjpqn.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gbriblckl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gibwlchdf.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gkmyhfckr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gemvqvkxd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/glwjrtusa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gcedfrocq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gtxuxqkfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gbxbtrrhf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gsmtyxdrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gxkwumceg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gekmfdfad.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gebpywolq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gemqhrrge.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/genrgwpea.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gthdnbzlv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gtzwiqqzo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gbihsecsg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/ghzdktwfe.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gozsdaltp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/ghuaouqfr.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gwmuoefpv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glofgajey.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gckztgwxm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ghwjfxxmk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gvphcogzg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gysugzziy.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gptyghsez.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/goxfkipuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmbssszim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gzvdimeng.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/glqvrsszi.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/ggxxnbksx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/geeqosscm.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gtezjtgmv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gfpgwhbes.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ggujtnvjp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gerrmlbjr.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gapbxkxhg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtrgdeucm.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gwmbvdofg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gwinwsixw.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gszvtdbwf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gjbcolymq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gnqkvvlan.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/giltjsbmd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gymagufwo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gfuekohuu.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ggqjroexg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsvohycbo.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gzozjyxmz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxxyztxzw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gtfkzwexq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxneasa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/ggpmtldsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gkdebijul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/genbyrecf.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gwihfyhox.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcscdcokp.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gjzpnqwbj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmcqbuhtr.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/ggduoqsol.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gnhrutvzf.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gqjhwlvqw.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gwdaitxll.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/glaekyyhj.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gmjtquhsg.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/geqecydsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gywcsxnif.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gkewwpgbt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/giolipfcz.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gqcvtxyqs.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gqyseoiyj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gwuukrhpk.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gvyjrjgor.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gqpfjsoxe.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/glhwyodaq.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gmbksmxrn.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gygxzocft.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/ghqsmefxq.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gutsxexzy.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gqffvjpsq.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gnncvdnfg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/ggolobfdb.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gnceuqpmk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ghfldujgh.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gdxxttowl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guwprkoru.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gxgywqnzx.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gotihelay.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/ggiwtympv.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gegbwzcka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/garpiodjo.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gjgldhtdz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gftjinrqu.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gvfesccbe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gbvvgmrlh.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ghvowvbll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpnlotmwy.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfmomwnxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gefaowzqt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/grcmniles.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gosdlrszt.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gadqmhupb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwxnmzhev.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gymzzuxrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqwwggnff.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gqqecajba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gmrazwgrf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gzljvfdsg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/ghvtexyqa.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gnkphwfve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gdboroffl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gjaozkrto.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gechdcpzb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggufnungy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gosgtniit.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/glsudotkz.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gdeudekan.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/giuwkfnrf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzldplwzp.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gbjlapllx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfrjrsnpd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gtnwaeqny.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gnzkcgzur.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gshiizdie.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/ghotqmkgm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/guyxdgxsd.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqcyxpgfg.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gpxnnqaty.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/grexpycfi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gwedazzel.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gpbbdckkj.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gqqiknqwn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gzmrdkqqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gniezugql.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdhezwpkl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gieptcsup.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gbschclgi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gfprhjeua.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gycoygkan.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gatuvcdcr.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmucstnwv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwhhqajgi.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gniepyrss.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gtswtotlg.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gnhqzdbej.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gztepmmhw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwqfqyxdx.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gbqleyxtw.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gzgkxbyjh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gwflbhlvr.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gzgwdqayy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gvsecmjjk.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gqiyzoqbs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gejedmohc.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gamqifhtf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gltmomwqf.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gamggffyx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggttgxulh.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gsvdmqwdo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gomstlzmw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/glqpuvtgv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gfzyntmxr.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gaxeiufat.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gxdyxytzm.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/ggzzvhwmt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gevuclevx.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gyhbnjepn.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gahxbuhan.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gvaelawlp.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gxqndxrmp.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/grkrswnfq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gqxyzikno.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gzlxeylxp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gpooqnsit.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gmuuobbvv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ggkdokliy.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/glwyyivys.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gapezncpr.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gotqjnzba.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/guthezwpg.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gvvfbbrfy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gjwcuyubl.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gdtglckbp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ggoveknba.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gkhtzhjma.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gggwkgvly.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gcdqyrnqb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gnxjeezph.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/grkuikqlz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqbbvsutq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gydxxjfcw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gazfnwtlq.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gfjlhupon.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gtemusubv.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gkjolvenr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gizxnzlli.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gdqmkckxj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gmbjccljx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gpcuhdjaf.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gxdpzzrpj.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gromketdb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gqlzbhrbl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gnofpfblr.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gnefpbwqj.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gwvelmoie.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gownehyus.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gupavnemq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gfpltvsld.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gotdlqirv.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gxbnmllca.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gbkmalzge.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gtnpegioo.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gqwrgsahp.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gtjvtbrsc.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gpwzamvmu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/ginzyjchz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gonkifwao.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gqrxtddfi.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/grfeyeaov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grmsvsddk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/ggrmpfjhy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gstptxvkz.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gihinkbyr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gecsgqiii.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gjaghwiro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/geyobhstc.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gfwspfpix.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gzawujloq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gcqernluk.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gethtqzav.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gdzqthnia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/guogdogca.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gyguvfpis.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfwzuwxsb.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gyyshbhjv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gwahlcqwe.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gqzcddaec.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gfrjgiipk.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghkfdpgax.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gjyfvdhmf.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gqtozarfv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gdqqyfsqc.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gmabdxvpv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gowtjokhp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gebjewsxi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gdsmcxwez.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gpxllpjxl.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gemgaxofp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/geyropwrf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gorrkvhdq.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gzfuynjht.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvfvgxsqi.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/goxkdyveb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gevxizywo.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/ghlwncrry.sHtML


<!-- 参考信息 -->