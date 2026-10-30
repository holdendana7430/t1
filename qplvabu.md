代发 wailian999

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjwapfqs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpotgii.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gczmdphky.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gwganregq.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdfmffll.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/ginavaftg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gxpoaqqtr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gkmkopezc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjdreqt.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaycqdumb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gajmqawoz.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gysgzqiix.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gkbioenrg.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmfpwak.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/grvtgfvfk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gjugbhxad.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjwrtgss.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejlwpgd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gugspxurq.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgpvqcps.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmomkmqd.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gweykvprb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnfczrpj.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gatnecmom.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gthphkrks.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxricfekl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrkabwxr.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggytwscph.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhpukrki.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnezuoco.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkhnyszi.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjliiein.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhzbjndf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixcptkfw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujlcyzew.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvhlwzjv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gwuozuhxa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnjbfehc.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmrmzdvf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gsujuacqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqlkoyu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gponqsaqg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gjgxpndvi.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqledbq.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gemxgvyrj.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjvsadgt.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzgxpdkfy.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/guzehpzci.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvlwdfjzj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntbdctmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrfnsvde.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtvrtemt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyymcksjw.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/grpzcwmkl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/giolzhple.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gzigrgipm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/ggcliqtvx.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcevujxmq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gfvaefhld.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoxvxabo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvwslgng.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gisipzwhi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkuqwlmob.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmjywlmj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gagntoxlj.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdercwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmeascf.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcpwtnot.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqiusple.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaosqulto.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtprplcxo.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gqagimffj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gejdtgzkq.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gizcfkgki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryphvgkb.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqzzlvmf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gosapjiob.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmbeudokh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmictjpkv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxjefwpu.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdwmxzjo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhwyrvce.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtztlvlng.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gkkukonlv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gwekgtovz.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxgfuzw.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gipniyltf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdnahadin.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gppdqalqs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjlyusgb.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdkovkzbw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggonbssat.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gbpwtuovq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpylvuolm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gthmahsct.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/ggttmsdoi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdlujpjny.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhjejzmm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbzevsax.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgfyyxli.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gvefusilp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gozuwhpjq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnhpzhkup.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxdnyvvj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gunuqkver.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greuihuzs.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/glrjepteu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyaorpqa.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxpjppuvr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmurfnak.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guequgzsx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gomnhpshx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxhmvmvgj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzlbnzfj.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gudbjuyyc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxtccbvf.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/geiphvrch.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gccrvtuwo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goudlgwob.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrzzboat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnekqjixz.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gzhssgchy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gvnairhny.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxiegjti.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gegmnhecj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvekqabzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyziwexq.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmabxrbeu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqgmzgrv.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gyanwfswa.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gsphzgwam.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gumqgmtvv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpddkzzrr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/guqetlylt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gknfymyou.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwpvcoizj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnosfdwz.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvccyuohl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gekxyyubb.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gobkejhoc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gberienaq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfkjwhoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrseahpi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcyiekvxk.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfvuvcee.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxevhmvln.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gqxaxynfk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/grcjrudss.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganbxoljd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfpdjdac.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gphyerlyq.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gafzgmfmx.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gvdtrhngh.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/girtfbomg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysajkqu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxmdtbna.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzozkrtq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/guwrxtwil.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gkntxyiwq.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/girhhazeh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmcsudd.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/ggowzwtpk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gltaqaikr.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gahbbtlya.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdeumltm.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gtqzqsfkn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfjhkvi.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyutefyh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxqnhim.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ggryyayyw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnksbejff.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glgpqlbwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnkoyfou.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghjfkca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaqhdaem.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhlkpuwb.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclvprast.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gsbnboetg.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gipxzlulb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpmmvey.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/giizogxkk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/glbaqorxz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godqrksty.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsachonz.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxpioioc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkgasjfo.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdpzpaiq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvbhwwnw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glpkfwmyf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gznnleasi.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwoiiczvs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyzqejsmh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgdmfmyv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdinjkkbt.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gveghvwnk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giphwzkmf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbveuxkdf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gloqyczke.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcbnwtiby.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/glgcckazh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqecdqegy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gmwyiidfj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizoxhvxl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghsjfkpwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtnsbgmr.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/glrpofkdr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwatvoma.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpgqxhvt.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqesxyku.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwpwgbmws.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gwpmshmqw.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdsqhndk.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gbcwuoynp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpybzgzjy.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvxeytrjy.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/guwxnojpp.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gamrqdbcb.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpahvvfz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxruxta.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlkjtljk.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghphumgat.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/geujyfkwo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqbjpblru.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gapxioyct.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrgzevsg.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjbyxtc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkdizscqc.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxthnwnid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpszxbdnw.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghetdavbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdscwqcq.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeobcbai.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/guzjwimxz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhoiegnl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqkymek.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfczjsspa.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gaivsiisf.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gppkmuqfy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbojrcyuf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugxptmpz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbydiwcc.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwxuglq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gosqkssdr.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guldiyigh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqgvrxcd.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmjmweyv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkqaccdlt.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gymkpschx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzocmlqex.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganueldpy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzasqmavf.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrbkfmsq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpssrqljb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlttevsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwzexwrrn.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyidogjrs.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/geoazqgqv.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkiqezwe.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgtyhtf.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgbjivfu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtibkby.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvwoixgxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghhuwxtez.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmtyqnfl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtewjycei.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gshhzdbkv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxykhfqha.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glnxwieoh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gywnlpavn.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvmdusmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpwjuwra.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guzwkswux.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/guqwowoyw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gkswwvenz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/govuajclm.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzpfavpr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbhhzkpq.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gvletkauu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyftidxnn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxnurdae.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomrcjtp.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsriecqb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gaftlfwsk.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gtdqkchqy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gebtagpsm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gypybryjs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzjfswsp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkqqgutpc.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeyftejf.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gvzewsfre.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gidekipth.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppieshqd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grsnvyfhu.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbgktkls.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gogvquzxd.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykiunoza.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdkawdfxq.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrtuhxzm.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwffnfdpt.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gczuggtwe.sHtML


<!-- 参考信息 -->