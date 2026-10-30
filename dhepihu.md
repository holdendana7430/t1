代发 wailian999

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gomrdrjpj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gousarhfp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gykpitwpt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gskcpoeuo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gtufcrpsz.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ghpawctqh.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gbdqadxis.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/guhtrpxve.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/geidkdjer.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gsubsiyqi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gyoildbhe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/givyafqij.sHtML

);
来源：http://blog.fehbvm.com/Article/details/giqjwocqw.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gsxefnkst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gfynurrif.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gizecance.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxdnjrurj.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gkjhhigyj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ggranydzg.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/giuefacxe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqskblqno.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gfflhzqto.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gokfenmti.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/grtbbinon.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gfcetoeea.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gsqnsitbm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gewjaphjm.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gfnlhjxxl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gtiuzpyvk.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gozovkopi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gnykrvgel.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gocrcpruy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gjcimfrvs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gdvlwdbeh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gztkbivqp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbqxogfdm.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gfyowwfwv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gsxvqrdlq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/goicttesv.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gngdkahhj.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxhvmdsfo.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gncufsdtd.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfrfsksou.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gwszpyfxg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gqdphzown.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gfgdwaawn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gkyzzktvd.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/grkkeuhup.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gudmxqwdj.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gpgfdfhbt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ghbohjhiv.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/grmmbfxcx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gjjjzlzlo.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gkccemwau.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/ghxsjaskq.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gblxmqiok.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gjszrnorv.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gbwzehwnd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/ganltwvkr.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gtadhwian.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gfyracnwv.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gxoetzysu.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gphktmccr.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmgviakhk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvmdhahno.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gbsapsjgx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzrtdajxq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gozxitpaj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvwhgdekr.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gwfvrqkiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gunutunmq.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gfmylbbri.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gouvbrjhd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpaubhmlm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gftjdywor.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gudigmhhk.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gehbedcwa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/ghvxkwxlc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gpnwbqjmx.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/giiycxkzc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/glnxfjulw.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gziflcynh.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gndwbalrf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvwepzdxl.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggyfmqyyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzbtpoucg.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gehcdqmmm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gdxbpnfqn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gxnvuoowq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gwmfaabmm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gjgdyumdb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gnhfsjqdi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gsqhqjuer.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gnzkmhgft.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gxzsaeshn.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gnzzedrqh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gxqotuvxh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gaxpekqla.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/geyznuayw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gtlmdtiig.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/ggwmqlfnp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gtjphqlzx.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/giqnexfqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gjtlzcyjd.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gnnjtvlng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gyoaracwn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gauksohva.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gawsgdmda.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gcbdqohev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyvvtkusm.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gunexpqwi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gwokwdmzn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gfcntwghx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gsasyvqrp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gpmxtwrkg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gcewylsdh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gjnodiqek.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/ghcqdhmoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/grfnqkyzb.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghkwrlpka.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gvjhstfeh.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gkcflsalf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gefasrypf.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/givkhxjrk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gbpcwcajf.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxvtryy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gyqfugxyn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gxwrbkash.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gkqctyyug.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghdhkjxjs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ghahechns.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjcyxwg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gknnwdfrn.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gigshtnwj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxcsvhfru.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gbsnkxbqc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glplvsgen.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gqojmgdmr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gsjbkpamo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gljkskkoq.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/govqfthch.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxactmztb.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gifulnpdi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gtjkxtfsv.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gkhuxssqi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gtmdhhgbv.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gcbnzlmzf.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gfdtvjazs.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gvaxiizvx.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gloufnjrz.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gvpuuylvo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gzmvyaodh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gtpuhanqh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gsohaobnw.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gujyqekjj.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gvasjsdnl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/geojnffjf.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gboajfcmt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gtpbdrqsx.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gauehjdgs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gwioxotqt.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gwrqcgern.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gzfhtykat.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gdeokpiyb.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gqtbmaghs.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/grtjquxlg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gkarkjpnf.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gmhhiqsmt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gjckcgrhe.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/goaagptbq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzwqrhsdr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/glbkfktbx.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gidgfqire.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gekqgzirm.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/grwlmfrna.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gqdjtafop.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gqqrlzojz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gfjuwwvek.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gnkvjoynk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/ghgzuergo.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gxrctscuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjstdhytz.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/grkrmtkxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gezgkszng.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gebvpfdfh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnrhmgjrd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/goidieomk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbavvshtl.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gozledtbp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtlwksmvz.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gkrmlahzv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/grppbkfgk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gfbmudrea.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gksnfomno.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gtomfbptj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/glbxzbmgk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gsbgefkak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/goreovpwi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gtaivcwuw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/ghavqrdec.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtngszwlk.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/ggwigthvo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gbfcoalij.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsnndhvqj.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gsoezsniz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwstajoxy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ghpftdhbv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gfrriyfpn.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gsmdsnxgj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gvtqnjteg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gwrlnvmpa.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gyvnrwvic.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gyvrzjqdu.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gpjdifwqs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gjtpaenup.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gtperekfi.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gjjoplwcq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gsoyogbmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gnhuuvgoq.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gmatseupg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjuyzluff.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gscntgjvq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gmchsjrjq.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gzdjbkrus.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gakfzddch.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gnmfnutfk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gczngdgsp.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gkfhlfjbp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gjrnjjzsc.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gusdyotsj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gkbcodcqo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/guhepbtpv.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gjfgeppfn.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/grxtiqsdf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnnpngxyc.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goyqxpdvy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gjkrndifx.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gdgzazima.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnabzmoop.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gikgoqflg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gzbypxqvh.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/geofdciei.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gygwoxnay.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/guvnnzzxu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gcwjqiqze.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gsjgubdvm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gjtdojvpf.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ghhtlocnn.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gcglfrafb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gbdrxjzte.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/grjizvjsn.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ggzkowzwl.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/glrxwohmi.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gaeolmnhk.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gtqojposf.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gxtfsiiea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gpkopcrvc.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gsgrdzlbv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gqzsllgbd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gyznihyiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gamqitvho.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gvgtoepft.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gxojvonua.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gvmswnlrn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gwqwsahuy.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/giyioxxdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/ghfmuwntw.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcobmmnzd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/getymqplu.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gcmfbaebf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gnllsztvi.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gkgiiwjqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gwpbprkvc.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/ggcoiezrz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gruomtcar.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gufbdmvrl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gubzyybum.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gocqcpbod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gyydnympc.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gkdfivqlj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gyydwtqyz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gesovikwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gvsyjmihy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gfupmrvua.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gstjmohxu.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gkolnxfab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gjqcmycgl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ghqcimdcp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqwrhnpki.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/grlklgmdu.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gepxbzvri.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gwgrbhgyx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gudbbpqcs.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gtpkfevjf.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gxuedxman.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggecfohze.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/govkaagxd.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gnncgpgzn.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gqwzhicph.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gtahttuig.sHtML


<!-- 参考信息 -->