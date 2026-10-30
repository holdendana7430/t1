代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnsighoe.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjnzdeqz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlvymdmc.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbluocz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtklbqgll.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gftbexxsb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfciknblg.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpydcwtzq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkhngzym.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gbuzvwuro.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gwnpnpyld.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/guxxsxdlc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gqdkurxgc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkymzwf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/glaqhzyst.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/ggdaszfec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gimayajqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjwtfxz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gaeljchva.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqdgsqxo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gcryvretd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpxbvyc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/givmymluo.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gepjkqkwt.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtvfbxnpn.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/giegkcair.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgswluys.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/grflengvm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgetrkgx.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gemjtdhkd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmmxidte.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggpblzjcn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhuughq.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gjimqskut.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/giefbmbcf.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gselmlxsr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiermar.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpjiavybl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gweulyktw.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gshxmvqkl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gwwefgjgi.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gbqwwdyor.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcgnqonr.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gduwlithv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxnofrn.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/glibyvpeg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvchawjw.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gtejkarmm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfruvnok.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrvciktl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gflfntgpl.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gbnptubqz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjattgvxf.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gekqcwkpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafriklbx.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiwxpxyv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmynmlbk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhksssg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwioiiwp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdcwhktj.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghogshsdx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfdcpba.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/ganmwlamo.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpllumum.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/glswifvaz.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkthwgoew.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjtnlxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdjssvnm.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdnphlhh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grltflztb.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghkjpnnqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhozuubd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrbvfjun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gfllqldqd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpoccmnj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gukktjkmx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyqsukgg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggepdonfy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfifmszhq.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxkuqmbx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gjpktwoei.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gigrnebps.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpppgad.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmzolzd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcrmlpgi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnatorjq.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gcztxdsea.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwgrfgd.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gawvcolwc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhmamkbw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbwqezuf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypqeojnh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpnbdalz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/guiqnjgcg.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyhzocem.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/godxdesbv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjaoyccig.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gwjsjtalr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmxfgzjg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudzqtha.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gevzueyvk.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gaswjbbsi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkprtpuxp.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gzudvswgz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkmcuxbhk.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gnshusapg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmmvyqv.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gccqqrkmx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ggpprkbjd.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmywfgvo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjafeqy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gucewndzf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgkkpylp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gtjhuaxwd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcqujptt.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkrknxyye.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwublmzik.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqjmrhqco.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gofqrcatr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuwdvigj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywpjpjjm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvyxhsnlf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gbudkuarl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gihzfirym.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gecyscupa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhrerke.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gkkrofyqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/grpexvofq.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmnnahgi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/ggiwovkpm.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggckptxxr.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxeqerkg.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gsdcekboi.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegicattc.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpdjtvbz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvlbamgx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkdbgry.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjdulnzu.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcgwdpuf.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gugtaupje.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbuafhe.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gxqvnjnlt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkwikzad.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gagfcrzzk.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvribqujs.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbnujigo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnklrlsc.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnkxeejeu.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwpavtlfh.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdizwpw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteeqksag.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxvvmnwe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyeaquds.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtqggfoiu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/giykibpvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxndatwuw.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gtldjutwe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldsuthtf.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdvxyzl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemfnurdg.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbqewhsb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/giuqnvmrs.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfuthnii.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/grrsxbopw.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gcgqvpnok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipssjqvd.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnycdavje.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamffyltx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphcevqhw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpbwpkha.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdqgelpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbypuhrmz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gbicdqlgl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwgbdbea.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvbswmkz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmdejga.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkluiqkpw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwkxdqu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpxwxhar.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/glputbksd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyludvgt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/geovwunku.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfwqaru.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gdyrkwbof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gdymqadwf.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrzpgjzl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gdntthznk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvwamvz.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvrdzszmi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvblxlml.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhfyhdtq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbsxwmwr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gikzsrusq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gywonzfaw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gqotsputf.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlrbwlkz.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqwknjfe.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbxnbesde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/grruqvagi.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gscmjxlmj.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqgvtyl.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmjwkfevp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnotymsqm.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfghasgk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmacvrgqi.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzmobpupa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezjjyrst.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/girplnfme.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gsldkmukq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxedtkxke.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaulecbm.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnyxnqul.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gatdwsmks.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlnlsofv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkmshyh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gizhdhlmi.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/ghtocetvi.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gchzyuxmo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbwfabib.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggfdbnalt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwyxufpq.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gotghecku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxljdlgrf.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gotiiixpa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjagbyjtx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbqemery.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnujpioy.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggptzlnjo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrwvmrqp.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/guohzyqul.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzkjtas.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grupdhwks.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhdfisha.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtleijbqe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ganjnoaek.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giqpvpeah.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpizwovtt.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpweeuauq.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkjiymaxd.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphsoncjk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtjhcqhiz.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlwziosy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdiszfvg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gbplkgdjx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqfczaia.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guavgjtdo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gengrthad.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gjyvddrot.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/garzkiiyx.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomcmoee.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gubpirlyy.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gctguuhyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsmfqrebe.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkiwfbxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gdhvbyvik.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaecqsmi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgloihok.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbpyfxhuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpavuvtpg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gipenwhze.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvbsghzl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahopbtph.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtkgwxwsx.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gqbowtdad.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihifznz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gukkecvip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidfmcpfq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmjnegs.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbvmrlyc.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmirhid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gyncfdovy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyooifpb.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gefmnsewc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjexvyvd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwfemspt.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gciwksbuy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grtlgmhqv.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/genjlstuv.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhoqrau.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggwgffkkf.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gewkhafam.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecfqudhi.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqtpicbh.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gmqgroqhg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gvfoxlbhj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gonstwqns.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gmdihzdlw.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gylajnhov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gggrjapoz.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfglmbtab.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuiaxswf.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqdhrwmxr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzznjqcy.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnxdklfp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxkytztxx.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gdlspqcdc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxhruzwhc.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gspvgyenh.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzfjtdhx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqcippsa.sHtML


<!-- 参考信息 -->