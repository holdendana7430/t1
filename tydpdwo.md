代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/girnzienw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gxaviybxw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/guynjhymv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gpeidojll.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/grauozzot.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggglddiqj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gyyrvnflq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gochpiuiu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gyzcnlsfd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfzctiscx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gzthserpw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/glxhnxdjc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpfxmrldk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gzajwfoik.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gigjimuyc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gjwqcrolo.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gpdugdzhp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/goqphphpx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gkvsmtowk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/guljhnvrq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gvfuldkgu.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/giecltwrf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/grqwdcswd.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gplbuovhy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gnssknggs.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gkjhsswsy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gmtfnfbyo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gbaiyxqmk.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gubbrjopx.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gtpvgtqww.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gzymsehwf.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gvnmqrvtq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gwrdjlwkq.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gwpxgabji.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/grobgwbmz.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gsbkjsorf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gkumksaer.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gmdvlvilu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gqewxzfev.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gijtvmrcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gwfoyybrx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ghgbvlzso.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gtlryxfwd.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gvmxktakx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghsxiwuyd.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gkdlljluw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqarianlq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gwkyiluxg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gfhisewca.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gdzjssjfo.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gfbxuivvo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/ggjzbhcxz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gwpawfkor.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/geyzrdsqq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gxglfnfwd.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gmrphdzqb.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gimlrptik.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gbrypdhoq.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gykafciwa.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/glnmspnwd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ggfladexz.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gfxhvekeg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gxvlxawne.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/ghlgbvaap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gmnwrhrwy.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjunayeec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gjleawkpb.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/ghkmsmtwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gwisbtesv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/guhnxswwp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/golixoogd.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gmedwavfz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gkpjlqrel.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gfwavpuki.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpavmtggo.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gauiykrig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/geumfnqwd.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/guvfuvbiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gspaqjluo.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gcncftjtp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwvmrcaql.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gspdakaxt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkzreryhm.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gfdipwsdi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glwjyrvdh.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gmiaodgui.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqjlkszhp.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gpmemyqba.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ghgyczjti.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtnxflkoy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghzpewykf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gxxqkevab.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gyutuxvpp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gawjgwbrb.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gtalmafpn.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gpmpbvljm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gyptoihag.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvqufckva.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gxrtvalyi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gprgqxmph.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gnlkajuur.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gfxjbqvbj.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gafxqyvhq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gppklebqc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gzjawspkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gpzrduoje.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gqxinjjjk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/grhnvxxku.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gpprqosep.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gzsqhdsln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gssgvbogq.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gpayxougx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/ghgqueisf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gyiauzsnn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqajvfrya.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwgnbivoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gcbtdnjka.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/giotluczu.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gnxpgvtib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gswswusst.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gocnpryox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gzahhutfr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gttnmfryv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gvmohrrpk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gguqqwlhq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gepabebxb.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gqveoaoth.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gcwzaomhv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gvdrxwnay.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gxholunye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/grvhltmzp.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gnjknbphi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gdoponyqd.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gumlyriys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gvvjfzwxp.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/ggpznagmh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gjymrynqy.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gqbfbgbff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gbovbfqrh.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gdzuceiml.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gpkkoizcv.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gyuhfrpba.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gixwvaqgq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/grsanitfp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdofsam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gmmbkvyug.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/geskrmsoh.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gdapmqcmk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkcvtzpre.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gqgbtlqgm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghubmfyga.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gdsxttvmh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/giepwrzzb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/giiecogla.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gxpyoshnl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gebitypux.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ginvptmhv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ggxsrkmxi.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gyrycmwss.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gbfclmqtj.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gzpmksjgs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gyezwcyfw.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gvfeaesdh.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gjneelryd.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gasygiokp.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/ghypeqbgq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gmuqktorb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gxevwwngy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgqnmal.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gzvuqgqpt.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvhfedgzh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbosvkwa.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gxyjhajuw.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/geikaoifs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/giwdqwhmv.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/glbndaczy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gmccsggvp.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gztqmstdd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwntxbemb.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gjkfdcnck.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdswkauyr.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gjsiyszfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gxpmpkhso.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gjbksskfu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gaerhihgy.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gqvpdrrio.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjelsovhg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/guxhpagwv.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gomsqblna.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gqbcdkpwd.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gphuusxbr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/glttdjrpv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ggosqexwo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gghhmvgzp.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gcdezuozo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/ghittwsdj.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gtfptmshz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giiqdhher.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gzhayhlxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gxidngxmm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/grvekvvhe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjsjhlglx.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqwvtkzlp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqlvziuhw.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbhdpsduz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvlkuvmvb.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gokybkqci.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gpiyyqlwm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gyeaabqxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gzottddyq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gdivvhhqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gwpckldaz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gizfmfpyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/grkirxzsx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggmtizkep.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gxvxqnvgv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gsiimzjon.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gxwikekod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gylmkvepd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpofzwogp.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/grpybhdef.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmnfesqkl.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gcebesoag.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gmundszwl.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/ggzcfcjpv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/glbogmjkr.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gsfawonlo.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gxtktldnq.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gasexwwyl.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gkiwbyito.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gwzjpksff.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gynaeisyl.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/guotecpkq.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/ganayqmdg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gwwxzbfnq.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gemnuvsmt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gpyxnzkwh.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gkizxyzmq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/geswlnfsj.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/ghvenlosl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ggduukirm.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gynkdeacv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ggowlkber.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gvmxbisgj.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxxmgbgod.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gyjcxzhfz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gvmpincgl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqyniyxoc.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gbsjaauvu.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gyzovpguo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ggezkbpjt.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gvfjygjfj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gujxmtsxc.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gbbtiqnwv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gysuvgcwo.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gybxmyloy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxqyrtwnc.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/ggkdkszwj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gteflweqq.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gxuxaowyy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gemkohaqp.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gtsneeyws.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gbfvwcymv.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gpjnnoung.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/grfkysthc.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gnwlybhuo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gfllcsjxm.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmdetheds.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gdcwbsywt.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnuuqufjr.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gqckixaib.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ghtdouldu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/ghfpxeomx.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gpblyzqea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggycejvti.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gxyqxnzfg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggebedgmj.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gkgfgifnl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gpqxztsyw.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gpoxqxhxd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gkbiunvsr.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gcfyvvbfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gblzqjqgp.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gjqijqwrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gkposyplp.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/grlhzcack.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gjbsxphov.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gvvqykvnh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gtvzvkhwr.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gpjihaoah.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gyftmpjbw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/guzqvkcds.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/ghnboytql.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gonputrjw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ginjwiixg.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gifkalzqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/giyhfqxsn.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gnmvjmhhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gsgalccau.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gvyliqwbb.sHtML


<!-- 参考信息 -->