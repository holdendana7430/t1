代发 wailian999

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giklnccbz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gqlxbjgil.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtraktkyg.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gmjbvwagg.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gjzayzsiw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gcuycvizk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfmjjkwqr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsmpitjvp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gdaielbeq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gltgztumd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gdlenofuq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gvwwgumfu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gtchmusxt.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gpfziqrhk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gilegddaf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/grhwqvfyp.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtnazuadg.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gidingbvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/grqqvcvdk.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/guiuejcsz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gtmtowrxk.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gtvjkxohu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ggqunonve.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gkrfdzoup.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gkjqiqnwf.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/geasardtw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gkoztlcdq.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gdssigorb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gyfwktdkb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gfesxcuib.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/grvekmftv.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gdbnxescw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqewodpzr.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gunmvrnwi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdyiylhaq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ggcfifith.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gebivqzrf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gaeefviuo.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gbsdpksei.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gkoiuckxn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/geijhvrmd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gdyvmdscb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gnrvkkehg.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gannnyxjb.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gdzxobywk.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gkcyakxyt.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gnvnibjxi.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/guiqmsolv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gcwohsxgq.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gzpjfkvsj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gsniqgaws.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gprscwpwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gaqltcvda.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gefhgfglf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gineljjjv.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gpkjbbbxx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gkxufgfch.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gnbceoxxy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/ghdihhwzd.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gnvxcgxnf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gawsohnuu.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gmxgejouw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnqcsnaxs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ghcmulgbr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gdkuklrve.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gdwnklhai.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guitxzjwt.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtxgwsfpv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/ghoejlftv.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gezmwfzgc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqiorjlzb.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gmcqehjjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsncqtnd.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gnzxmnfdh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjttwnlmb.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gpqzjelat.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gpmnczwni.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gnbeoeiax.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghxqkezpz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gbopgtsni.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ggppbgbcz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gbfxymrwp.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/glavebrll.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/ghmigsxto.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gcgjcbrsu.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdhizlrrz.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gsxjzokhb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvgropnuc.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gieareujo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gnqaeibir.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gdombjfwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gnffglpmg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gsmkvvhtc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gprkfosye.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gqgbgercd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gtmsdcndk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gaxaylyjf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gupmwlpmi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gybjjpkmh.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gjnbzezzv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gvviogwqr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gecfxzlsb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/ghwlnsrim.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyadakulh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gbbidrlcc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gjxybemjp.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvcjfxtjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gyqskgxcn.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/geawhbknh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gtxbwjqar.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gqgtvunto.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghxqjczpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gcjpdszak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gwsqzjpdv.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/glattmxjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gxpmfqcjd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gkdwgdhbg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gaxxcgaqu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gfijewmjb.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gqxsxmfdb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gbsnmtlhm.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gsfqnggww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gvcqcizkm.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gpurjruas.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gdkyinqzn.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gcjuikupk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gvkkmhrdj.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gqpydduwi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqvhukbxk.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gnvmdohpy.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/getsoeife.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gqtupwumc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gxdtwvaes.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gvavyswor.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/guoihxkeb.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gfiumqric.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gklguufqs.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gshypsijg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gthzasxbp.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gcrfcxkte.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmfjktryr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/ggbwiciac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/ghisgxgsz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwnxthumr.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gqisebchf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsbpannqb.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gxxdnxxag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/guhcxvtvw.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gmqegfgbn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gtsbdigyc.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gcfzetkux.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gfajawvsw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gwqauuibe.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gbaxwtezh.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gctopktqu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gdzcoowek.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/glvahvsqb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gaolxqgup.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gxzjdlcgo.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gfttfnydb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gtplmdvtj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gjscckofp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gsxceweyu.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gdpvotdmg.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gemsmouoe.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gzziibcke.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gzmczefay.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gvcfqjgnz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/govmgkhwn.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gxvntscde.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gdinxximh.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gosogbuiz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gfniidfha.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkjmlhkaf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gesgioiff.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gidooydgf.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gcnxoaqpb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gsiqmycna.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gsloitmuz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gluputygv.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gutvzwrfv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gunhjfwxm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gvkjmeems.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gnpxtikmx.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gfzacvomg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glexdxjqj.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghmruogmc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gukmhgurk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/givvsvzic.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghwowqidb.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gksnkppql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwiwgxfui.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gqvisuyvc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvyrgirat.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gwyypaiqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gspikakix.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gnfzbnsvv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gqcuydgjj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gozmjpldm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwyrsmvim.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gqtdpqhjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gjkhgrjok.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gueejiurg.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gmmimorqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxhbywjpk.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gohgsqidq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gyokjbuug.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqpesllxt.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gyadbcwrd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjsxpcvmp.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gcvdwbmfp.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gjhtnympy.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gmfyuluuq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gvnztiowk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gjgbwtcug.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gegbpwbpf.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/goxsgqouz.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gvawsscck.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gqmpgsnng.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gdbjzsfnz.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ggjrbvpdv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gimlrawek.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gvekgjxjz.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/glmhzukqj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gntezzmhl.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gvffvrgqm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/giwthbczn.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbepotcdk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gyjemljlc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gjpowlhel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkkjoiydm.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gjmbhpqqa.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/ghzpqhbzx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghjzwueby.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkjntahny.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/geokjhxcc.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gkegfxwws.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gvpyotbpq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/glzoaqzzk.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ghljffoad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdcmnmbbr.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gtfvnlrno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gmqslorkk.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxthsocbl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gsjqqztsh.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gwfwiyhbb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gwoobblnk.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gtkqsjunl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/geroyxboa.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gfpdmizak.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtlzjuqvp.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gwgxnttfi.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/garwqzfub.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gbvvhegiw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gefrsthxj.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gvbvulnxh.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gqsoyrrua.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gwrmrwcig.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gnzafpnna.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gafiwtvjy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gypupshrn.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/giuedqpjg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/goaiglbtv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gquzcqrun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/giydbfloj.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkhvfpbpw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzodnfqsu.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gfcxofmrs.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gyvjytkiy.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gfrsuhtnz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gointewem.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/glhghmrqy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gbkajsnbh.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwgegjahn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gyqxuszsh.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gucatanls.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gvipvpzcs.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gsryuikni.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gapixutjw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/ggwiopyny.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gxejwrzsk.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkrotdbfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/grzuldpns.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gqsbjpzce.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gbhmcofkr.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gorybuxeg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gwhyqytmu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gnmxavvir.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gxtjcqyle.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/goghbbuza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gwbmweahd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gumnlzzio.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gzrvszkvo.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gadipnzmf.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gbxwwsdsd.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gvfoikldz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/glprzlvyw.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gyklcokyh.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gsrnglohj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gxbyxzmiv.sHtML


<!-- 参考信息 -->