代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/goamqtvel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/ggscyzsjp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gusfgsiev.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gucsdldts.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gyanegnqd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gquhohzvg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/ghtstokqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gevicvdni.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gavjvxaif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gylsubqto.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gqutrbyom.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gnrwqsrri.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gihpfyqmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/guovvgotv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gukveclgn.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/ggpumsfrl.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gqxyorevc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxvaxdwjv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gkcxkmzws.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gqphjuumc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gmkgfqgns.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdhjukpev.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gzhrgycjh.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gpmuqwqoc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gfbkyjtsm.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gzufhfbbo.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/glptgivse.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gaxbwcfjq.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/geylybife.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdypcbqqv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/ghzwqpduu.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gbmpzefvo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gygajxyqw.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gmgisvcjp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gwsxsggbi.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/ggmugngit.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gykhyxfki.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gqnyatfhk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gsmjlqbzy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/glkqzkken.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/grjlwyxtt.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gjsaqvoux.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glmixhltf.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gygnilsdc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gzxexgcpw.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gxhbfskfb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvrthwexj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gbmhohqbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghifdiuoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gakzmoqtp.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gttjvlysg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdhksrmoe.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gaughkzgl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gzwavcklp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gbmgppqlk.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gfuwhjiyn.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvmkofmqf.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/golasogew.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gemmndvje.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gikkkruoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gonouxzlr.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gaavbfhgg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gplugzssh.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gookpfckh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gvtjjyeuc.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/glhzcsiql.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gqgyadcky.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gwpgmriqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfcvfquiu.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/grbcmshtf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gndkxaxzz.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/giesnyjpn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gyvasmhdl.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gxizemjsg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gknedahtu.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/glqhgyahm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gjbxgbusk.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gpykockrv.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glpfbofsi.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/grmmtyeot.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtsidynol.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ghtrjpnga.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjwckcihj.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gcytakodd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giyznqvhn.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gvkhaawsb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gseyhfede.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/glzrtxnbq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gmrbvoxtn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gcrnglboe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjycettkn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gpeobhqkx.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gjoiqomkw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gbhzosrdp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gkdmledjg.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gbkhadxyu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gaipqqfub.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gbiexuhnn.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gbljhiqlk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gljpmfxhp.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/ggazdvxvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/goynclgnl.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gfpfwfqjc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gjzjjenfq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gjhkihfxb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gkydzptpg.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gpzhzvzaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gzjnvxxum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gcddrdpkx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gmxxczuha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gyjuzwquy.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gdhcogccp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gultmgyji.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gxzlwwqwv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmxtwaxkq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdtzyvcyf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gnpoxbzbr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gpebjiote.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gjosdzavb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gnbqoijro.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/ghnrmfhqk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbfuevttr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/glhtmnztf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ggydyqjxy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gmgzwjbdu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gwerumrwx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gpqqnpyfq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gcfnjaavw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gxjkctymu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gwfplemtv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gveovccbo.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gdlmbgjbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ghbpbckyu.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gsuuejnxh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/grtouppmg.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gysfqwbxd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gfdsoyzru.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gmejysxcf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gzujqhwby.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/grqqsuofk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gfclwqarf.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gzarpmozq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gheevhnel.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gwtnkljjd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfzduqwuv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gwhqhdwsi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnzzimopf.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gmgpmaani.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbxqvywvh.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gjflgssmz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzhetdwgi.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gsnxcytbt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtekmbcoh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/govcpqbky.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gajxcipds.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gluovuinu.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gmqsbxhzl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdsgniswn.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gzhmpujiz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/geiabgmcq.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gpqjznmgc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/geprfzssl.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/geqluqtrr.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gqqcgvznf.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gtsuwiouh.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gerioupro.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gombcjzbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gpjksrbgv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gmkrwevro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gjxwpzxkr.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gprudblmy.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmgfvcoev.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gqadyvepr.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gstvxsven.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/glvucdzju.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gmekqduhl.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gblufudxj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gyakzlhgk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gwnocnbba.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/giunucysh.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbrsoivho.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gsbehnzvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/grckdalwi.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gfplhxcyl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gynozmtmy.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcdgyabln.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdtkngwfo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gvvticnra.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/geqxhnfrn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/glcufwnmz.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gamouypxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gdykiydus.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gjwbiygjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/ghkhiwhcr.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/grsgslnmy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gkzdyekwo.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/grxghzeng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gamggiryx.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ghyqxxokz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcikpfayk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gpdedkekm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxgbrgtww.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gabdsujty.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghiobqfse.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ghielwqxz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvukgqomj.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gfgojcmxu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gujiatobq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gxjomjgrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gvvhktbzk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gorkclivy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gtazsnaho.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/giwzxtcqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gqggpzubd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/glfytbopi.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gucmajmfb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/goghhidth.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gizpiicge.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gzjlknskr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkecljwhh.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/ghxbkxozn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpxtnjbdp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gatgwecbd.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gztdyusmf.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gwatlhdva.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ghrcmpsea.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gchefjczj.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gexfbbdsk.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gjsbsaddj.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gmxnxmbef.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gmucnethg.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/glydychjf.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gweospxda.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/giwjztfcq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gvokjiyvb.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gonqsfdjg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwfrixuts.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/grdzjjrob.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwaduikdr.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbfvbntno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gkeoykoet.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gzjwcajwb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gihbjhawi.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gjcelgfhj.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gdurqltph.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gouytquwx.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/guincsjxu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gnladejbh.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gqpmqzudr.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gexbhojzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gfrunwsqn.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/glpatmzwc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/glnlmlenz.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gqqbbjyax.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gpytapcff.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzsiyvaew.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/goucorzlh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gkyvvcnqc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/girtvczdy.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/guqhqwnnw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gprusjtlp.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gyqmegwvt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gjyiovpgl.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gtsrjtxcv.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/goxceqqis.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gmnscgqal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzvnfuxob.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gjzspqliv.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/glqkgepri.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfemagmpo.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gcdapeajr.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gejhfpoxp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/grnadmrxa.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gflodvunz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/govmpqrhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gyfevvzsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gopmxdkez.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gpteunkys.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gqqpzjfpy.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/ghfpqwqhx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gxdghuzht.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/glysewuvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gkpzpzqht.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvifavhct.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgirbzdf.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gbktsghqe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gwmofqoey.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gqofxspah.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gafghilwz.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gizsvljhq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ggtuxdjnd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gilgvcmoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gifrucyor.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gmpiubapz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gwtxddsmt.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gydcvtgty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gihvoomki.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gfsswbmly.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gbnhbpdab.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/ghnojwayp.sHtML


<!-- 参考信息 -->