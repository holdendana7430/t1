代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsszlodlo.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gpgodtkuj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gfaxvwgxi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ggyscfptl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkgbrovve.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gumcbujqz.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gpwtfvyht.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gfwmhmpyj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/girzqssyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gnymldwgv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gugrdwohc.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gneqajztb.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gcpfdadtw.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gkxhaosaz.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkmmnmfly.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gcdxsadvu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/ghfsttcsg.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gxmmkrbqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/grlcqvhrq.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gyjixkowg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gucwwvjfw.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gagdaopfk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gznmzufal.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gzklqavay.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvgtvfwqr.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gnfqnpyaa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gtidwpjke.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gnjdvxbth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gnzoalszd.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gbzhmqetj.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giwfxrovc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gpoadektx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gyjhbmare.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gmgtbkpiv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkdjeythz.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gaasymhtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/guyzmitsf.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gjlqhbcmj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/guztxqlvh.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gjnjonkay.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkjyqjxjh.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gfirkpcgx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwjvtycbr.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gtnbghnjl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gqncqrooh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwbsrjazr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/glwaoacsx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/glpheeyxb.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gakiwcdyz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gnrymwbqi.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gkmldrcns.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/grmqqibow.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gnkfzaqps.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzpreosqz.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gbtrncrzh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ghhhfrcix.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/ghfmfwhcu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gcdxqlbuz.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gkhbxaahb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gmtkicjwl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/ggwiykhhz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gwqdknnlx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gqtcrsayc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gxpkhrgkr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gnjvoerau.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gsqfaghur.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gsezkmfzt.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gjetbyang.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gmnezhktl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gytfzkmln.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/geuvuqzci.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ghduaewer.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/glwwawfln.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gceydvfyv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gwbhhvrei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gtsundlcq.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gyvsnibmu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gkhezarmk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gxpzrdtmb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ggxbixqkw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gcgrrshwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ghcgknric.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gkqezmdro.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gfsqqkyoe.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gtabkvzwb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gpgxcygym.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gfdjnoczz.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gcjmynime.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gwfvzqgaq.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/giynvvgct.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/grozhydfn.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/grutbzyok.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gycbvnwsw.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gsnuvtzmi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gvdzbxtms.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gxhuiorfx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gltcmmkmu.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gofwisypa.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpseoji.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gmjizmrnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gxgmeanfl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/ghbvrkmfd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gpvxkutfj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gepijgoup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gomdktoko.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gaidwavqn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/grjxhkjrn.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gsbkpnzuo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grqxkrqze.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvduejckc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gmpwbufzj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwntvbzbq.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gyaqgqvyf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfupramky.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gdfawwwsi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gyprqtfdq.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkvxlizit.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/geiwhnirg.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gglrigcjp.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/grtsgelip.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gqyqobtzn.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/glvgennwh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gloippjrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gpqjyafbp.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gugzwglyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gjaffxser.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gnzircabp.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/glqydoekp.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gfniadidj.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/guskwddki.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gvyanafnd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gbotznsss.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/giuiffvyh.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gmupcarye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gbfuqqdam.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gmckehean.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gehsjbids.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gtshbzyla.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gcfnrrhzv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gsgvnadro.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gclmrlpqs.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gerjtcttx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyioydwyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gbyjyasds.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gluhukdoe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gwqeijazc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gvkzuwahq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grxpxbmwz.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gztwiosmj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gbpginkad.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gualbclkf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gpudknbro.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/geaoaksjz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbliavwvk.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/glmdckkpc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/guvfexeqr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gbyvlzewb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvkoactgy.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqcrgmnin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnvkxedvf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gzajeatuc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfadcocqe.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gygursefh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gtehwucxd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gjjogexcn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqdzyochb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gangecmyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gdaxldcpc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gegaqcqez.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/ghogfhvix.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghsmqzlqb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnangimas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gytktyduf.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gektiwqpy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gnvrgzafb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyvgoidrm.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gorbklqtm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcvxzcypp.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gpqnfnzet.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gnbfcggmw.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gyypwcbde.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ghegepebc.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gfccphbvr.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpygfhzlw.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gurayxoop.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gniecukda.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gtobdqvhc.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gymdwqdye.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gwjoxqygi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gaoglhora.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/glaoerdir.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gvddkxwni.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gytkeycaw.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gnlsdvlne.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqfnzdlwl.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gylvkfffc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gooltxlbg.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gdsselraz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/glsewhied.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gyavgpkad.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gbjbsawhg.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/grfjblbyj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gwjhhxoje.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gzzecdujv.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/ghhteolcs.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gkqnbgfja.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gmlzmwfze.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gbahxfpbe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghlhrckaa.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gjvjrxveb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/giqjcccrj.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvsuxsxhs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcvubtnhb.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/ghjletlfe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gpxbagmlk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gbkxquecu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/geabaoxuc.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gdpczhjoa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqdinxdxx.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/geevdctwt.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ghuwqmpfj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gchaicazv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gqbnxvmjw.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gspxkmqim.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gzsvlmyyv.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwjjiyzqq.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gzxdbfvqh.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gkeddzzvb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gcmvnxmok.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grxeubmkn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/ggtovlhfz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gpbbfqlvl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gkbfeyxgq.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gjgffsobv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gzcfznykx.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gmogfughd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gkiecfiad.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gebeziloj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gwuvftojl.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gvldzarve.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gyhfqoyqw.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gtgbajjwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gniyvxmbj.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gplspmlqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/grgglmzzq.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gdpjuviht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ghcjvvshy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gccmpaqka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/ghumsnzvu.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/griqavhky.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gjvhcdsxu.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gdqbnhrge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gsbhykkqe.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gjpdkgtep.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gjqrmfnsc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gmjrbyqde.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gsdomvgca.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gyynygzft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gyzxocctg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gnmhvntcb.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gylffsirj.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gubnsuxaf.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gnknjpgwx.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/geyvetuen.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gqhevbcmc.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gusrqdwjb.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyvoizexq.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gppkkjbgq.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gdkwfgedu.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gysyntetm.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gwwyyqhab.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbpnuzctc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gyowdlovq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gyhakzppt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gekwodorn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gxuvqnonc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gyycprimh.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gnrvkflzx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdoftdwbj.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gsddwthhd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtxeonc.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gqnrosfbp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gwjkrrmrf.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gxubasbfg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gvdxqwuvu.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gohpthmee.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbvkyzcax.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gxplqrcor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gjjwybvtl.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gmjuzrzvk.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/ggrhktlty.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gyksyoujk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gcsehbxtx.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/guosjthhw.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gfykuhwsn.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gzbefvzvt.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gtoetevut.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ggtbzlxli.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/giogbtynw.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ghfywhlxc.sHtML


<!-- 参考信息 -->