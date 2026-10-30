代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghydvwivk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsjvdnqd.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gcfnthwtq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gsujfwmth.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfwgqic.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnclgshbs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapamxcsm.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gliopuiqq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrkswnhi.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gmtnbgmgu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrtmjgsz.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glmhtgmws.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ginaknmar.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjbriopnc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/giqqtwzdx.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawkxwdpd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpowjwbyv.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gweepbpsp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcssoqzrd.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gojsjzdul.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhcagtlu.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdmsnwfh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhcwretb.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gviiuzzhc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtrbgnv.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpmysans.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gausondny.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumoshxw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkrwvgl.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gthutirfz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqfzshfs.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gshzaryke.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegbklhhg.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gjieldiuc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgtziayo.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtliqia.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzamhrki.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gigpvhbsr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoklfyhm.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gnbpwjrbz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gljkzzost.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdefzhxom.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjasaadq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gwxvvmdmz.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmqjaapc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gsifwwvap.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/grtdilboh.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gslvjcsgo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzxvzgab.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazpnjlau.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/grwkomfyd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgfwyxl.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gczskldho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaqzjtco.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkclvowaw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiwvjwbl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafcovwli.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrosrofa.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsrdpwxq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gilukxqcm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gptjtehkr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/ganyxobkp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjjiqlq.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqujdbo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvpekuzf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlbkexyn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybonxpar.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gthyjvxev.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gustkjiic.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfwfxenh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grilmroxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvspzrgf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjekeqegd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukjqbse.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwwuqvrp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gycrkyjrp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmswmkc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqnexfuu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmqbgnae.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghclklatz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gybrduhea.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymptogk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/goszpvyrb.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/glydqsyzz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggysrantw.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvzcglqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnabgbz.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/getottmnc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/giqxwkdbv.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/ggapfwflv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gizjdhfwh.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqivieydw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikwtalr.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvjfjczi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gxryxsuit.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gdicntnxt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxhjxden.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/grofydusx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gttglbxre.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoxdflnb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjumnjby.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzddeibbt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glfvwstuv.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/geupelrgc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkanoxpou.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasenlzkl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkvcofln.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwscbjbq.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjkoupz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gyhldhuge.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gnvwujxwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gxcyvhnss.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqglnrgd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/guypgaisi.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmtjwbsc.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvleoplub.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqppwzhp.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepcfphkr.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbgotdexb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmhbjgll.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gsatjhdjg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqydpyst.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gpqmyghkm.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvllvssh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjykitfgz.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gztkvibvn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfaiqnzx.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkrnxbw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwnypudj.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkdoskoq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/ggualgmsy.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuflnomn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmepstgta.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaicccvw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gviowpgcp.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyutirey.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ggwuvhhtc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdxaiewd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/guhwuiaqe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlhxhtyi.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ggroabocd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gporfmzsc.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgckivnf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/giktavxkq.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/glqfpjexa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gunaxmkot.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkmvzrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gemlhjtfn.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gpxmfwvzu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtconitw.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcggzwoyg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyzeoiuo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzheclmcc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmdipgsi.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gibexnptw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvszohquf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxzcvuoy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gacrziexf.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gsweeqgiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbmisjvp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrbvokd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuwcfeva.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhbskvrp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmckdyyle.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gpgzwkjdu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvajhnmkz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gczbwouap.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gyagsywlu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxmlwgkz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcdfkxde.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhmyzec.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gilpjwigx.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gitdflfom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpgosqhlw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiffpvsl.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/glkzpinai.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjofvnpui.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghnixrqhg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/glohvudcc.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznfwxgka.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebwamqlw.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnptbrtbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsosmetyz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfpypsjj.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxaeuxipz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gctdwdahg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujwodfig.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gglurbcra.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpohsslk.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gsdzoeolo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxypczves.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgobnlwm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvwnlrm.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtitoolxz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmsgcmuk.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gykoohcvj.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkfhlgay.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawwgegw.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfuwold.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gihukasik.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/guwyogzvu.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gugmcshes.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gudourikp.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnecbrpqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmekizma.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gbizxbeav.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbltbxidt.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyjkmvyxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnironlub.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgcybylz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdbnvvpmo.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiibuccl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjvipchre.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkomhxck.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gldgslkbg.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/godregjud.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/goxpqqrfp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhplhhf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvucljero.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbdkoxmbc.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/grbvabknb.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gyduxtxfb.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqsatkdy.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggbrmrqry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxtkqfson.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfqgdpbdn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflekqmmu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzvulbqj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqgoohytx.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgmobas.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gguazheqf.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gcieigezf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhohvjib.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gereklpwq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlvqfsed.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcxxuvqpj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggyiolroo.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/guwahtuzv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyjykgyum.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsrvludo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukjdrpgx.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gtyewhuot.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzjngkevm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/georlzvwb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gezafmkoz.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gipuujjsq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/glaiucarg.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gzlfnhtod.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiiimqej.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfyalejh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ggifjklki.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmigczhr.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnrchbhe.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/govzeiaqh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/ggnyjyqls.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gbhkjqxmc.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/guviddrba.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/glswnpiql.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtzlfxkei.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjfwfglwm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbxswae.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gompyunxr.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpeiezj.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grdctcttj.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gttnddfai.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciymtwvu.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbokxxryc.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gobzjcxkp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmdgltw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaehymta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimatlcq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gckthaggm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtywuarb.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gztrpudfz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwmpphes.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/goaqgvsjf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gcnxzwvtb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjpbmbrhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjydeckny.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcentdbx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gtkbrkzps.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/garpwjrml.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcznypzr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpqxomid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqenchvpc.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtjrezfwd.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzvkfezmp.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekwnhngj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglcwuzol.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuarmamp.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gimiyzfbw.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gqlovkohw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/glwhwibad.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskopkse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/goqxgfbcl.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjibijuu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnwydlvfg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyuwibwv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoojekbs.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyuofbsf.sHtML


<!-- 参考信息 -->