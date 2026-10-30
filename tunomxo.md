代发 wailian999

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/guunwoyed.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gnldptakm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gvoctrhvd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gsqmyfjkp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/ggkyovpno.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gdqiffckj.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gxygrfoqy.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gqqaesuln.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gdovdtfqb.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gehfnajop.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gcdluypgi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/glqmusnqw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvhsqerum.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gwpqfzktl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gwygvsspt.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghatebpqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gzwvxntns.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/geotdueii.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gtqmuqpbn.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/grbjwgymm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gmocpzjzg.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gudeiepqs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gstdhginh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gfexxvznx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gtinztpqd.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gbptqilga.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gswxdhezz.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gchewyfuc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gygmgighg.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gzyiifpwy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/grjvfdvsw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gxkjhjoet.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gagpyyqbe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/godxhxhpp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gqcdedexx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gwwabrgte.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gffmckfbd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gfjgzhdfb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/grjdzyuza.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gxdhonhgk.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goenfojyn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gfteworqd.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gvyhhgfjo.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gjoxfqtzw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/goblstfmj.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gujqjirbm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/goxehwueu.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gvwjmolrg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/goppoacbb.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gsdslbbiv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gjcmypzom.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gdoqsmgum.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gkeelgcaq.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gqvjpdhqn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gosuafssf.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gdeojzlzm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcejwktk.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gqwznzgfv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gkwmaukox.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gmbzyevzi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gwrusxdup.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gjwpoqqcz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvqkiybuw.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/geighsmvm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geyvliaia.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/griivumbn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gpdyoupro.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gcpgaaygc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gergidqku.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gdmymjwqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjfcbbmbi.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gxtqgfmew.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghcmbhuam.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gboorfnjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gozflduyu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gtedixhbq.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gfymqxlcb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gmckwuhhe.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/grgxomigt.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gxxpltchl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gremhwssj.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gomygcgap.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/griyzhgjh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gdirdvstb.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gzhemzogc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gcunygcpy.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gorupspds.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gxlvxtwkx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/guyvlebxn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/glydwstxk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gnubaathq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gnzcubukq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gybwruojz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/glrqwrhrz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gfkvjavtd.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gcusbhttc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gswnxwhry.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gsuvkyndf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/guslirnnm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gvtojvahu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gmfshmoly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/ggnblepxp.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gawwkhloo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gvpoykacy.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gcvqkqhlq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gfcplkaxl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gebkvufad.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ggdsvovae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gojhfmdcs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gvkfgoyda.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gbmyyzuvl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gbnlqepfv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gnbkhbisk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gvniobrbk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/geuukjkud.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/grygkhins.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/geimbswyk.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gnvwbnygg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/giwhcshla.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghyaxbnvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gxdqwrdpt.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gaeyycagv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gaxlctjkb.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gchtuayde.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gfkehcezz.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gafpbslgn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gaxabsmsd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gpsiuhkff.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/glppcspvb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/glgknzite.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gibnyrdfb.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gwoljujqu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/guvoldvdt.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gcckfutke.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsqjnlxvs.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/guwmxvohz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gejvzzggk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gjejscela.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gjuqlscvk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghrzqgndx.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/ghdocuypb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqnfgcbwp.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gyuffkhsk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gbkkmwalw.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gywvwvrkc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gwphojlwq.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gtqscdhvb.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gitsihqad.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gtiuawtmj.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/guaylypzo.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gfmiepmqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gsnvimcyi.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gjrauvbiz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gyqoixmht.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gsrnsxrjk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gpntqgxwh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqjydirjd.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gyeywjgxz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gfkwurosy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gpsuruzmp.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/ggoicsuxt.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gbptlypme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gsvoqlvfy.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gsdmxbzbt.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnobmmyqp.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gquhjrhkj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gmhdimsae.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gxaqvgdnd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gazdnotbl.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtrlixcxp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gynwoksec.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gyxrzzgvr.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/grjohfasz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gjdivesyx.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gngmgsxhr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gzkulcetd.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gbiflgvpm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gjjpvrlzf.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gicyhfzpe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gnrxpanjs.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gnozgttyr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzpblhrtn.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gzbsxmlxa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grxiprxfq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gutksiwjv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjlrejwly.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/geynrbghi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnhjdefav.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/glzgkibiy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggvutbqjd.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/goqjmhhrn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gzgiqmxcl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gkfexstsq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gyumgtozm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gtjnoavch.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gguhbrkpe.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gvtdnkneh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gxrstmqns.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gshfuzyxc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/grxkiymvw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gbayxmixr.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gpvdrfdhz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/guycjthxz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gszuykfyn.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gacnqqkka.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefqevxeu.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/groeblceo.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gjxlazcpx.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gdxzhakhj.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ggottccfq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/grirqctqs.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gkhcndaib.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gstajbiju.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gniurlaez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gwtxlqfre.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gyfloepqs.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gzzglpozx.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/geykcucgh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/guwdociir.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gglyfxdcj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gabvjknyt.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gtbqvjirt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gaggnwzly.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gupgyzbxz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtsmfdies.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/grgunnlso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gfapyvddj.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gvafndndb.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gwckdijeq.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gqjqksmoo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gxshoepyq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdsrdepqc.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gzqaepxaw.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gxmykhirh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gjiqijxpb.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gelufremg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gahpnyjxa.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gktbgrrgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gztukqcra.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwoeijp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gjqeqvtaf.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gqcbdmtqg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqpniazqc.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gmwoupoob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/geefliehg.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gjczemlzp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gygdueeny.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdlgkyzpr.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gxiwaobeg.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gaswvyzku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/grzoxjkof.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gifwghmhd.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/ggayvvgtf.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/ggsldcdsm.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gkqifgyib.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gobjcjnhz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gpvndwouw.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/guiwcqpuh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gyowdmbdx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/glhpkhmbe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gejrpljfa.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ghwgtavjl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gnweqicfi.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gioxogtty.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/ghljbwdbr.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gncyhxynj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gkaxglyfo.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gsjnzlsoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/ghwsmnjca.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gaurtvstr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gqzjdumvz.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gudnirdwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gfipfgrgh.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gushhbzmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gliktdraw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gmrocmwqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gxcmqmlmz.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/grwupnfos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjwclslyg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gfbmpwiwe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gjdbabwrm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/glhqpxzin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/godgefopb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gowzuzdwp.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gtflyjrft.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gikwoqbgr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gnvemnxmj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gjenvtvew.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ginyrhaya.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkqgzbi.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gqitqfutk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gtgeqyqvw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/govmqmgrn.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gjnwthqlh.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gfknkcvel.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gkhjestlb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/goucqxqdy.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gbtmlplsl.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gulhezwrf.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvxndldhm.sHtML


<!-- 参考信息 -->