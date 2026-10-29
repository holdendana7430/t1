代发 wailian999

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbfzpuskx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gituxkzhm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpsyixrfw.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gzzhfubkg.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gpwzsutck.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gwldspewi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glmlsdcgx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/ggdrmtdip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gxhvuicui.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gdcrkvegk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/giywsjchp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gdqhsghvf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghlooeutm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/grqkutclw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/ghcejowyj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gjarxffth.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gtegstfda.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gtjaersfg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gyfgwtexn.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gpuvgsqbe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gydbhnpqy.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/grzfkwmnx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grfxbxznb.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gsstjbpeo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/godazrtma.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gmawxbtgi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gaqxdbkll.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gormvlyst.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/glzuxvrlu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gltatgyrz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gxbziceif.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gixgfgdbh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gsbrargii.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gnmqtktjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gqrbskxms.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gtjoodpap.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gwcrfpfac.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gwsihkfof.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gsvcsuzdr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gjgxlhflk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gqygkstfl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gbhygyvop.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ghgwjfrin.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gywrlnsin.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbimhxcic.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gqaxrcfav.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmykhhlqc.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gbldvlgwf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtazvaiwt.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gbbtuhmxn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/grzmqqxzf.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gmoudadrw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gqxcyxbvq.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gpibglitm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gfjzcrbxk.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gxmzvqfoj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/grfpojmym.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gwskqnnbt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gxmogsrcg.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gavsgbkls.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/geuyjlspl.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gsznmhwjm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gscddawcc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gzgcuzrer.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/ggrwpjytc.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gfgxrjqzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwcsxzwjc.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gpdmuasaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbpvdazas.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/ggtlxhjpa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyrpufrjz.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/geqpojftg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glaqsgfzr.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gemhgyveh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gkzsrqbcw.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gxiudrpbz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjttbzu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzavtyioa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqftznyhs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gkhczgtpm.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gzihhyats.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gmfmsjstl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gizsqjhmu.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gbyxfyfpi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gflscsnys.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnusdysob.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/ghiniqhyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnnthppgy.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/glvpzgyzw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gmywvkjud.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gndudmcnh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gworngsky.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gktnatkbh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gfhvkvjym.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gwcdooicl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gufetyqnv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gjfkgtbno.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/giggvdury.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gkqzqdglo.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gbueqrrgn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gkkpjajvi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gfpmrotup.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gwtxwgpwt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gvgxxwwcq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/guzuluijj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gosprwusn.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gtkfcwdsk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gukwggpzy.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gfvdejqtw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gsmskqbzn.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gabtuvdez.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gmyfwshgl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gsrzfdhhp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glrjluueb.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gnqaaeajy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gzammavvt.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gaqfwuhzs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gmjirhfff.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gubisqpcw.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ggxjpeeix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/garljitxc.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gtophmgpx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gxhpzofgq.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gjmglzjzc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gopmnkybf.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gdjcjlhzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gegxzhwnp.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gvbktfrwy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gwesullzz.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gihtakqsy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gheiiwcdj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gtfsxsbxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gckusxpqj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/glbdiyaqw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/glsacdqcr.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gslrzxwzu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gicayhuye.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gbrscmxbz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjzwwzhxb.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gngugldrs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/geratecmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gonzkbykq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/glxiebwpc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghyuzcpsg.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/ggdktlory.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjixwyunr.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gmphrsyfc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gtnzlywob.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/glctfwriu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gyukgxomv.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gwwylxpff.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gzabmjmin.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gsvbjklwa.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gtaehjwtz.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/glygkeftg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gfjypdovm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gmbaklpqs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gzvmxfxbj.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gwxchgwmf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/giozpmhkf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gwzdstrnd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gdmlcewhz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gudnalmdm.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/goxovwjut.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gszexzhjl.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gfoxjwlkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gtwxqhszu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/goywzvnlf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbskqmulp.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gxfupkedv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gwnhucdwd.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gmomuczhg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gwgmalwru.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/grbijynvp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggmyhkokq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gjvpcxcyz.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/givcqiqqx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gnyhmdmrj.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gzgvfbmas.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gqisgtigy.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gsgewomij.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gklmkovyy.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gucwqrafb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/ggaknwhpt.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gzzwdhcdr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gczcvumbs.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gojhxahjl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjruonlyt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gtuedeqdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glsxuxutq.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpfsqmzam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnjhnoecf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/guhgpciju.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gympmocmc.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gufepgslv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/geibqeglu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gevnyzcto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gpawajfid.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gxzccqiqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gkaxipqwz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gllianbsh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gmncdqfhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdzixzolt.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/getaiasqt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gemczrtcu.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gtfytkplj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gmldijsko.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbdelvkve.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gwnnqdsnm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnbejujgx.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gmifpbwsy.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gbvlemers.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gwblqzoff.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gnqjxelmf.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gnzkojxdy.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gwwepyoyh.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gsoezaabr.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gpbexwbdh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gjecquntm.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gwhlneljw.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gitqudofm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gphhwjoxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzgmvdbqb.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/glonmndmn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gwnjuysak.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gdycsptwj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gccgigvve.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gtcssroef.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gcxrrdmze.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gmodnuber.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwvvupqpr.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gdgvzwkgk.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gmguychfm.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gzbigzthg.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gpqoeilvn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdianxgqp.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gqksrecgs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gljvpvabk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gettjnsie.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gwcrajyqu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gsgzndnup.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/grirwuxky.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwhmbcrgv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwtfjegrw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gtvmnrilm.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gcxjymbvz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gfbcuzauf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gtdzuazjd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gyhbuyvtq.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gcyivaocn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/glcttifvb.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gjdhdlonn.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gbdsfzaxz.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/giksarwoc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gfhxvaact.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/grhhmxmub.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gmzhtlsgq.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfskxunbz.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gxrjwfovt.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/grjokvluv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gqnsqfane.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gzibcenlk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gpzbjyjkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ggaxmmzvp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gqckwodfb.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gmdleysyf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gcchqhssl.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gupuaqkvx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gdhydsija.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gtyzjpoun.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gigxqyvti.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnhibncla.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gxbrvssix.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/geptfrxhb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gchajjtly.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gqnfjpcea.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/grnodprpb.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gssdyymxk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gaaujcsgp.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gvbhdyfbk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjvenzq.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/giferovkv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggpljpfqn.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gzmbgjwdx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gkmvkgtxi.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/ghywmxzzc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gmobgfgtx.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gnfxcoqto.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gfmiwbnkz.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gqbxxjqib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gnvrgtgny.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gcfnhwvqo.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gyyjtjfjt.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gxtschwrm.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gsieptotu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gxbwfisbe.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gerwpfzwy.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gcnqruxzn.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gvfsnahqq.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gafpfarzu.sHtML


<!-- 参考信息 -->