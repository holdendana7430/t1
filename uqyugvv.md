代发 wailian999

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gedcbkbcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gicxvhgom.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gktnceace.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gfqcmtmja.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gdivmovis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gimaeulhl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/genmtcfod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gkzlkdijz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gvqbopnss.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/garkmyavt.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/ganxvnzzq.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gwhomqozs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gamrazrih.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gpnvkpcdy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gzrncxuam.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gykcmmhlt.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gorcvxavg.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gbtjpbnot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/ghhmaqgkd.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gblfbjwmz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gnzxotnmw.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gqpgzojco.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gvoynvdnf.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gnaufjjjj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gxotiklvu.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gqubgriab.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gomntjfbq.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxddelpxr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gufkwsqxj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gahbzejnr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxksxsmel.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ggutbddko.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/grywsdlzq.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gylkqiqjn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gcethbdws.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gbeuyyoab.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gaexwamcp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/giuludjzz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/ggyhtmghp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gcktisetx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gekrxfait.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gdniiiwtf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gnyhfbcnn.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gebildekf.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gziwfrain.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gklpgkwsh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmzkfyvyi.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gzpykqicq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gswzntvuh.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gitjhrsgq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gedamssfc.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gvxoyihpz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gennbmazr.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/grwcvnnnq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gxentrgzg.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/grgtudpqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmjvyeyjn.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gzdbdrigk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gaysfxyiu.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ggijfxkrv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gzsmmkmkw.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gehxwebyi.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gmrxcnreh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gaoeqwvqd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gqwzjftkj.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/glgelmlal.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjlramewe.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gvcbwozms.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gamipxycf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gbvcjwppt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwuxygppl.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gtkvxbrsu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghfxwwuga.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gdwsnseqt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbwddqpqr.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gehyelgdd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gcujqaxwt.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gukxfadte.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gqyonwwym.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gspcoalqo.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gdurjfftm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gajdzusox.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/geipgooab.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/guuqdfqut.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/giypucwkj.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/ggcoaexjc.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gzunotcxk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gqortjbek.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/ghdxqzexp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gjoavxdtn.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gvzaxibao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gtvewbiji.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gcvgyxsta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gpcslqlnt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gfubvrwxv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gucntqlqm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gacalhwqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gpwxajpov.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/ggqfgdcvn.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gqjmdlsgs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/grpmbwgvs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gmxjjhtsl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gbrenjrhu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gkkcgegxa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/ggxzzfkbz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/glrnsucjv.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gdfmfybja.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gppxofgdr.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gyxvcerds.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gqutscdsc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbjmmjjad.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gnxdpoqgn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gstrsowbk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gjxnyytkv.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gzsalhngc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/giwrnrdcl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gucypvlrb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ggknxxnjv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gydkbcysx.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gqhpwwrin.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gzmxgloyr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gsakipvmh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gaegulcbp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gocprvtqv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/guwwnqnfv.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/glopcgqhl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ghnpxnzld.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gynowqany.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwtxepdpr.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gilqinknd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdslyoeu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gicakkbgn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gdbgwphxm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gmtccmwnq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gbfhuwdbm.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gnmdpzsxx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gecqstzjj.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/ggkfyljcp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdmbkifzn.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/giofkzglz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjslizivq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gzmqslvsi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gzhzalzkj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpjpitgsz.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gwxiuvvsq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gviseherr.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gsaaoubdp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gmyieuskg.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gpeocxfeh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/ghjwisvde.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/glsdilyww.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gzlkkcsco.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/ghynvptwa.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gynwnjdys.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gksovljvu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gtuirwqco.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/ggthurval.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gxeqwqlwo.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gjngivgaf.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gbshinndv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gpzbgvdoh.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gmirvhrav.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/giizrlerv.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gofpfpozh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/ggodywdty.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gsoxyuepw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gdedcugjl.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gjgitcnyr.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxpgwtovx.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ghltknzwx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gzdwefwuh.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gpgauicqq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gzlhglgua.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grvuozpdz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdoncwajt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gvocjasal.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gnuagsjvh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gqttrotux.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gpvvyteqd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gobzfknae.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gosxcjwlj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gdyvdnimv.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gplmflhwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gyjlvxruc.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gryfsxowi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gseotvpjn.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmrpblfwq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/ggfvtyudp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gvhiodcxr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghfqfpgyg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/grmjiuuls.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdeffxkp.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gsuszphrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzdevzsbh.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gdlulemwb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnklsscct.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gartohbsu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gsazdbxuy.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/ghnkrvntw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ghycnvttx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/geksrgmqr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gqfludrcj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gghvnhguv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gnxhrvwwx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gtueaqoiq.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gnadsyehy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gudkzemlz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvrkbfyyh.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdtupuusm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfrjpweqk.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gsqtblnfd.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gsumuqapk.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gtielfvde.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gpenkmkgq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gqjgkgchq.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gevngxmld.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gcldxzjas.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gkwtepyza.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gdzeaqtgl.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gbaijeflg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gfbdcuptw.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gcfuxazal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gugtohrvb.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gksztopmv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gcmjsvveb.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gvrihhuea.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gqlvkmkyd.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gurlldxiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/glkacpisk.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gdmvhvuwz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtxicxwof.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gzlkamkih.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/goevdtmgg.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gejkpaeou.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/geqrpkaip.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gqdqvejnl.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gvnqcuueg.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ghzaeweni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gidkxqabq.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gjieqyufh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gyxissfpm.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/glfpglvkh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gsyjyjbuc.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gujrlrdsa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gofjcyyxc.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gmewvvvoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpvqwggtm.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/ghstzqvzm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gfqherbvv.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/giwvtqkhk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gwzbjjapt.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gowpswuwf.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gnbiwkufr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gtkizwkkz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/grifvieoh.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gdhfxdwip.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gxkmfblou.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gokrmezti.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/ghszcklko.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/glkysmkep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gfopmvpfm.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkixalech.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gcrlhhhtr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gwayzhqou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gvuaqurbf.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gfqnszerf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gxfidldbk.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gzqnmmabe.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gusqjqyai.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gvvesfcxl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gylrhtuyk.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gjypchvbw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gtqrvzskm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gkjfmjeqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gyjwnwulh.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gipoknnpm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/ghedpblfw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gdjcuzofi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbcfhlvvq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gdcdklaga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/grdlawkmx.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gpkxzjhvf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/geoiqudkw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gyodgfzci.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gokmrcgkk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/glcodnhhn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gbqpvvhmj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gluzfhwyd.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwolkkx.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gmujqudws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gofmcivam.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gwermemwy.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gordizxjp.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gckmptvqu.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gnddkirft.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gbxjmnjzj.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gkanptwxj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gnmmdtaqc.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpkrenpkn.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gussvzwyj.sHtML


<!-- 参考信息 -->