代发 wailian999

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gqxurkgfq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/griagdoxt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gacaaibac.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzkanzql.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gxxlaxsss.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfmjuqrt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gysyvfbvw.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gatfmoebn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/geqfrsyzr.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqkfvvp.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjsffwuj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfzyowgr.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnuwztzw.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gbvzlnofk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gpfsvcnme.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/glmjzytjs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifzlknwq.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gcrjrvkmx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaofqswo.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsjycujx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynqptbky.sHtML

[Q07] 删除表
来源：http://baike.fanxiaobao.xyz/Article/details/gkiszqkaz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtprujhuj.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gihnxcrzq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnlsgdwz.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gabvxtznb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeqsjumq.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjryysvjt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gqknfecga.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqilatixa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gwupucaso.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/goljokafe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdqbcpp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gftiskeef.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkokkbxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnebqbxuy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrcdogxb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleotpbir.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmzjilrw.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gsunxgbzf.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfrsrzzq.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gapaoeuwd.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyckhducj.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkxhyvcwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gpngkgioi.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gphrcbnjx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmaollmb.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhdpket.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgvgcapw.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmxjjjeq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggklgukbe.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbbpkzgx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnusnzdz.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzhylrynt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gokzstpei.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gxygmnlzq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkncfcelg.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigrxabrq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqpsguan.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghffftojb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gtoittgzv.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gquyoaubj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaemkgqm.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guamwdpbn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gohslvmcn.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxluuuokq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glzwssjmj.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gxbndwsmv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmfadkcq.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gmwrfhrwn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gmcsrkndn.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrubhax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkkgiwe.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmcuorlg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gitercrhf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwimzzqke.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gdhlkcjul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcohwlga.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gtdrmmlcq.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjvqnzso.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/glhnzivnn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwffnkqoi.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmuyovvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garlutjta.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/guqpnyezt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdzjguim.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbvyeni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdmsrjem.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqfcijip.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgawaplr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjrdvxtv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkuvhncl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbcfudkq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gskdkhiyz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqkqqiza.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqdzpgwhx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gpxwdtsor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlxnppxs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/glehmykdu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmlqupc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/grayvhxev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnhzjdhk.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghzrczrdj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/ggkcueexl.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gidlmbtec.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gjpgmwfsy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqftpkmyf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqtetxumi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/giredizep.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guryebtwx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/galaekoiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/guiurprwv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzvdmvnam.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgclulyg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqjhmzku.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfxbupzp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpmawkag.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gygligdkx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyspulte.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrljvhex.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gasbwukil.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcvtubfu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghndhhlup.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggmlzbxzz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjllrusn.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gunrprjmp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavcuvwu.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimvdjki.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllftyata.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpazwipd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwyqoits.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomvokxbl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghsrghlp.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiaktnll.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbojvxi.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwintjek.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnrjgxayw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gogxckwbf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhimegu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/giwdbmudq.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gecexhecn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxzqgqzn.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gretcjeeo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpctwkaai.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpdodxshd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gievdtvfh.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrwdzrpw.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/grdegepwr.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpssrvni.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gumrlvnsd.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gcqcmnwrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubtqvpef.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/grnioreju.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsttzslgz.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gslsvbvnz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gagevsffx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiiykzvq.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/giyewpghd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/govymehbq.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gpssiwkoe.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrvokqtg.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/glorwnxtv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gterhrnxb.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/guukyqrag.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcufehbe.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpbnskzn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrqssmpz.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsywysdk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gzvdrffjp.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gntggraje.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjreyqiz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvjkbyng.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/grysqszmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfisvkrjl.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzjcwssn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvupvdvnt.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkxbhmrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjvlwqjs.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjwrflrt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqxdshhq.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gzfmbebez.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbdzzhpd.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/guuxsnxwh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrgqhdsh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaytexkyx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmknzpjzu.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggecmvgpp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godqagxhv.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gbbiszcda.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkwxtgqi.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gntygqpwi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gniyphmij.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gxspieltt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyfdhzcd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdbfgwsgp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvyoguj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvokgrkhe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoxdfdrg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glngquvim.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glmttcxjn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/guerugybf.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgignpvd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gosugsoxl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyzdofuc.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjtlqtsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glyqixniw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtitqdeky.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/guqiasbxo.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gugzumgvt.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gphjqahng.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgylkbyq.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhabnngs.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjtxjcpk.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqypsibll.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqtbsyiq.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqohdgqka.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaqoryni.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbuzbwxm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfvwccbp.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaudcczxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwvgvors.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gemesknqm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcdapeyob.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaueuluh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqftzjmud.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjgiffuyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjaynyaj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsuvervu.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gnorcsgds.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geprxbxgw.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhmusjil.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqpvnqwa.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gthyzqqhe.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/grzubswqe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcaxrqih.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/glofpcdiw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujnbkjkz.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrpbrkt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubjnganh.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gujfopcrf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gucmgbjui.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/glmowlxpp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbwiyfcco.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdclvvdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytejmdoq.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gtchgmunx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gycnoweko.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbfgkfw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnnirtfn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gifryyijq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstciooy.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwgvjskka.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxkysahv.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gaiddplvi.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdcucjvi.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtravlwog.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/glxchhmfg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgcjucth.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpddcph.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gifobwtux.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzzkwosei.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypidmfbr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuiwrood.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbfhbxvf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlftxxj.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gilmklucm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gogxeviwd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glausjboj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghxcpyrbf.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gisuddccw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gnhsocqla.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gziomysen.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjkfcqm.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/goqpbomvo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gblsuoebr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpjjesn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/ggfdrzllc.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpunjuxwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gntmldoyh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gmconrali.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gafhvulgp.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gssvfarer.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/grgaxagho.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjgorjep.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiziwtqd.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxfhmck.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzrjoepp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gijanphwi.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gawevennu.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gueyyteav.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdqphzcfo.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqcbipgn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gjdbnxsio.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghddwmhpu.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtugmgevc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeyrvjeu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbmeztaz.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfjnfnyeq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/guvmjhhbf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmemsunue.sHtML


<!-- 参考信息 -->