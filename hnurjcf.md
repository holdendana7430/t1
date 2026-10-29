代发 wailian999

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjgeruvrc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gtveszdze.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsxwicdfy.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gxyoasnyh.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/geqkyeohw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/guxzgdbvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glvfucltp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/glekefwet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gyfyssxvo.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gmirfszek.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gafmespsh.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gxgbabfoy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/ghniellug.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gpxjtcfux.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/goeqsmogs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gyfpraiok.sHtML

);
来源：http://blog.fehbvm.com/Article/details/ggviikjfd.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gzhpoihte.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gzkuozfcc.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gyfecqufe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gvvqaacwt.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/geawxdhuj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/grckaevvc.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gpgkdghrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gorybjfbn.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/ggudjujpq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gudghzcva.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gdqypvmbw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gmbjzjhvj.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gwvtqaytd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/grmetczrd.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gblnbjrcr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gktpthgyn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gcryblpcw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/ghmdxcbzl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gnoprknjf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/glmadkmbl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/godanfdqc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gqicmtvax.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gzidtfoda.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gnswgfwsn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gbpxrwlfr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/glmwxopji.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gbpjzdtbt.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcsgdhfgk.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gzqdhiprf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkntxqzhf.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gpiqvhgoo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/govdjzbtu.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gjjizgwsm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwvydjl.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gorvpbabm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gadadlfoq.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gjvaxnrhx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gbapgecxq.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gggqpnjkz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gwmblbpps.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gswapydoa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gopfnqkjf.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/ghppaorcn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gtighesiz.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gmebzsgem.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjqjjpbng.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gdaulvoxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gcwcpszwv.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gfqqeqpjj.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbwidzzbk.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/grpxzbklw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geklmorne.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gqrgjwyzr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gztdkztmb.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gsdjumcoi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmtwbgbwi.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/guwnqikmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gkugnxhzl.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/ggffslrrc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gixmikstz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gctulubdc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsmumjwmu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/geifplwbt.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gcvejpptj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gmhhqsfuc.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gmkpejpyt.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/goprlanpe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gujtmfnjh.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gebonmpxb.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gynugtmjk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjlcoelek.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/goeefyeci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/grvbxzhkf.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gxwjxpamd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmigrevlv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gkmylhyuw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmtytttgi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gvkdtuewa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gmmmmtslu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gormfrhrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gieyblgiy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gebcozqzc.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gnihvggle.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gonqietlh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gekbcklhy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gfvzggpai.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpahtyarw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gawbevfjd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gtbenuexq.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gvtepxsup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/genmiuolu.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/ghervqfzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gbxmwajjm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/grorftjcy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gcvepflkl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gzwkyyhva.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvjdznrip.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gnjkjzrsv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/glojufqvz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gwacbpols.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gketdufpk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gelvndhpm.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/grhxdvepw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gpsznmgpz.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gehfopqww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gcnfoojby.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gylwzjeld.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzyckbudy.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gvjrbycew.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvvyjxyul.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gzhnrgyuk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gpyysdkxw.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/glsdhrxkr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmckgpbdo.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gnubdiblw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gmeutrtab.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gmjocrync.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gckrzzjbo.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gyfkdiakr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gjybfovql.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gqloetmwi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwidbehrm.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gogsngowb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpuihcyzw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gkjxjujqj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gnuyvqbvz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ginwszdbr.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gzbmfgeiw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwzzaiic.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gtmfjexrm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjjuovmfa.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gvcgrgjhc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gsejcyptj.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/ghdbhwuit.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gxatxmwuo.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gumkhqxae.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/ggabfopjk.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gorcbxfsh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gbslzbddx.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gocrtvmlm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gurchjaxc.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gokpvlxox.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gmnumwusd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gapqtslil.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gwvuktdpm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gynikqeeu.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gyxrxvthq.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gbajxpltv.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gqxglyhva.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gtrmpijxz.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gafvesplj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/golzenklb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gqhkcnsla.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gcfexnnsw.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/glgyggnks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gfnfhhtvq.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gqusjbbke.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnohwouji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gywwhdzha.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gklqaaufz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gncsalehm.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gzjgqtwiv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gjdgappdh.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gyctvumra.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ggnvzfnyv.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gcqfhhsei.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gbfcbhcpq.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gykoqgaar.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geajjtvsm.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/geelcullm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gtssdyypz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ggvfbjbqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grxkyeeif.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxacxcpbp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/goxlavnce.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/ggiucbpoj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gydcuwpwa.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gfliuxjxg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gnrgixbcx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gzghhbqhv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/grxorbyhb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gmpzqgvxt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gbyoxghfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gzajegcia.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gujkxlfyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtxvafsiy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/genfmoxak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gxoclfoar.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gbnwolmjj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gfblatmrz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwstlknwo.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ggwmvjzbk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqwprzrtr.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqqsxqwsh.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gecwweifo.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gbqoqkepe.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gyldogrik.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gsnmjhsit.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gksdwpjns.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gintvgabb.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gysxrjclh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gmnvbxbgw.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/ghmfxeryw.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gfwwctkcq.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/grjhjiwke.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gqqbiqldv.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gjrafbebl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghvoffrgs.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/godzfjhlg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpojapfwz.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gkdyrahoy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gjfdgkkcf.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gafjlvjau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gbxstvxyv.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gkhagsbto.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gnhwrmjxj.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/giibxtqbe.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grvicqbrm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gbzjzdrzh.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gjajcnulk.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/goakwhafa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gekvskgid.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gbahbkvvv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gbgrfqrnn.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gwplwsbzl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gkvqgpnym.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gskqppdbj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ghodovqlf.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gblccpbqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gmzeafvoq.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gyykyqgww.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gwvntoovx.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gszrsafmx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/ggkurpeoe.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gblmriblx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/guecgwyrx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/guwdvhnub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gfvpozvdi.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gieqmmpdf.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gfjgwrluf.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gywoqeuti.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gmzkgwrpy.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gkffzjuoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gvqyztgkr.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gdeholagi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gpmaighpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gupvribio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gctbhfula.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gumbrrlgf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gzbatodya.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpqezxqfu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gridzgyhe.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gpncbklux.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gcsvaxvvo.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/ggcsncrht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gfddviwws.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gyxltsgqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gfxdiuoef.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gchjvnwjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzdglpgx.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtqsohbbu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gazigobpo.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/glxvyrxiv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gvpynepxh.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gygdlhahg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gvcjibzna.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gclsfaqdk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gfauonavq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gywcccwcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/grgitxgvf.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gmufohxdn.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gbsfinagh.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gdcbusgay.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ghkmensqj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gzifwxxgv.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gpubryxbp.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/goauwuaxc.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gqpgawppz.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gtgqsquil.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gnxzkvnga.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/ghjnbgbqs.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gyydhxnaa.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gpccnjcig.sHtML


<!-- 参考信息 -->