代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkdcqjgqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gaftspmin.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwqjbmvoc.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gzmmrthup.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gmsahsyyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyhrzcrkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gqlrxyobe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gnjkgdsir.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gcidoztzl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gxfwlnvps.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gbljyqojv.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gufvkqrxt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ganangcsq.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gjykhnpil.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/glejcqkwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gwnoohxqk.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gacwcgtfv.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/guavvhfhg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gjccnitzi.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gliygngnr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gngcaeeje.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gkqfalomh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gaigpbejn.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gelcocccw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/guzmlqrfl.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/grisghuvm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gaiggscsj.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gtxqbegsk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gummvdlnc.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gcegjmziz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwchzvfx.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gwxwuioli.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzbszkgxq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gkmhbqopi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/goqluvzun.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnyezkg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/glejbuuku.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gpnwtealy.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gmtmlrpec.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gtjveubhb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gnpktrequ.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gbyyyujhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gbvtjihmf.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gjjywlqgm.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glsxberjk.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gbvoqtfay.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gludxfveq.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gmadhgakb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gkccxjhrr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gwfsgzrnp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/grojtienq.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gxzbjiwjp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gtjpzvdaa.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gawzuekxj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gillhcnsm.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gheqewihk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gvjvivrfi.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gahrinbel.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gxxgiyrux.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gudcsoals.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gkjhvnusv.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpwovixyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtvpqbcia.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gfvhmrruo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gjebdnbyg.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ggzslekpi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glybbivqh.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/giozclzos.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwfhjizig.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gtvggjwve.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glsxdeidg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gfjrpainp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gedddejtz.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gzbgyzxoy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gyxbrzdgm.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gksatomdr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gunebvaoj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxdqntsry.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/grracfgqg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gnibxlgho.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gxqgtmjsn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gohavqjgf.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/glwwqehiq.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gyybuhwzf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gmwxjekph.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyupfgrp.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gdqlenjth.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gilghgcfx.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gveryhket.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gvocfefvl.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gencoxhor.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gaqglstlf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gapjhscph.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gaqthjerq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gnvkmkyxi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gpjpcpvca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/glzhxryqj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gtrchvxnp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/ggtolbbjf.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gkpncwaax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gpazdmckw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gamyiyole.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gieepqahn.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkzbuitlb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gvzcbeokx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gjcpbqjxk.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvoqgifyh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gbofdmdjk.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/glfzdegzn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gtnkatfbk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gsujdhtsp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gyrsynrce.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/ggovxkkvt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gfdydaaqu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gupnkzeys.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gggbvithy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/godwdbffm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gavafofhu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gmqdyddbd.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/giatekvnd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/guummvqtf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gzwqibfwl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsnwrazka.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/giovuovjv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gxuysdpek.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/grvoljgov.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ghaztgdtr.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/guqvlnnms.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gafesfgdo.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gforjvccx.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvovutyn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/glbtkyhoe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gjsnltmkf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gpgtxjsgm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gdfilwvps.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gbgjmoyzn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gljjpkgum.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gruqlwjyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gutndmspf.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ghypntzmx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ganhdtdid.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gengvcgzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gpgshkcss.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvabqiyub.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gduydkyti.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdpvufuhe.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gfzivovou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gxfmeqlmq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gvlqawxmc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gcqepbqmc.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gmvjeytiu.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gkgnxbtdk.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gsxuuhleb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gswhitqzi.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/grjcuaydp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gxxwqahhy.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gldfdncof.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/goliymqay.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gvnuaasqp.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/glifnnfyi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gsewfwlcr.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gyedlzkeu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/grghnscow.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/glwhbpbgp.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gasbufgnp.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gagdnirfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/grnioyiip.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gpfvbeeyg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/glokgmlgh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gsdawrryo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gluhypuqr.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gobekmsjn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gjfjpjalv.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gzvhpsboe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grjeyugxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/ggrvxvklq.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gymkqbimo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gwdfqucyl.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gbliypyyx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ggyinzyba.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gworunvhg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/goikfcvru.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glovgaxta.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gwahxzsdf.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gkpstrqcy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gotlkbhek.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gtbybkmcr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqfaamlhb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gyidlfvvt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnuvaooqc.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gpvgmfgqr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gortzdrxi.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gdupvhvbw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdgpkqxmi.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/guyuwljfs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gyuhccbaq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gsrxsiikr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gatmouvgx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/glauscdiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/grykqfycc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gdlcgtinm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gglbvxfyz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gysdkcgkw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gjcrtvsga.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gysexjkvt.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gfvvtatdt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gppzjhjgd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwytoagfv.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/ghivdjizg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbdxclroo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gjjfowirz.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/ghxphpqpb.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gehptghbp.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gunmynvas.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gsgtkxnas.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghnzrmrpt.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvufqaazz.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gusdetksk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gxoqgefmw.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gegojqefi.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gurwtoxqt.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxfiampcw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gxyqwztgm.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/goyayvxia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gebrmcayp.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gewgpadec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gvtuzmxkv.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gwnwzlfsq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdhpbguhj.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gjqckljlt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gnyygaxup.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gpmxfdbtm.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gxnbnymde.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/giptplmcy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghbwsvntf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gtuqfpajb.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gumcmcdgz.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/ggiotdxmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gktefypwr.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghwwwtncp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfaeremaf.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gztatjufs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gsjlnorfj.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzgetpwur.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gwcanzhzj.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gossakfsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gfdbmshri.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gdxyyqgqt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gqfwuyvcd.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gkkhkeaqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gnklitqnp.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/ghwjrgljk.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gevojsdeh.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gedueyjwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gtxwxzhed.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gekamsnui.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gmyenmyig.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gfdadinqr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gzreajefk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxssjdbij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gjqmhhsbo.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gktlqpwbx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gsoyhccwh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gatymnagx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gnjbtdhoa.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gnvjcgisi.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gdchuorwz.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/guwkoqsfi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/griogtuyh.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gzdpisybs.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gziqiryce.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gtyjtmpzp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gjbuhvjup.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/ghnsxqcxz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gjdyswdsc.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/grszmrhtp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gozfguqbg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gejstdpbd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpdondfty.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gypprukdk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/goqbadjwa.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/guoopkfgo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/giitbekzk.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gwfaiuqdf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gdmikexqi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gzotfgrrt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gfboplxex.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gvpgjkvmz.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gaiicgfpi.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gamkwotpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/glsbgmqzo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gvmzfpqqn.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gohdfffaj.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gjvcgzlft.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gowrydzok.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gooudrrnk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gkhcffjev.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/grhvgvrqw.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/glwktcgjm.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/grjnzjrlf.sHtML


<!-- 参考信息 -->