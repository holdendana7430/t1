代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grucjxzyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gggbamvjp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcgewfbt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsufhqite.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gocmohvnm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giltlljrj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqcrmnrh.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gksnljkgs.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvajadm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gokezmzdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/glppwncmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gpuvpdvtr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gznkeueob.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkcxhlin.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbayqjepu.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtolbihp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvufeveqt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpuygmhx.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/ghydhgvdk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfxfcdqk.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gudiszsaf.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkeujrdr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gipjfdgcr.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvvorfbf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gohomhxxn.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/guunutufk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gwsruxmbm.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gvqwlobbd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscwzpbkl.sHtML

[Q07] 删除表
来源：http://baike.fanxiaobao.xyz/Article/details/gnyqzbmtn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjabphdwi.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/glhdaqcol.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gougxmwjd.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxmnlisfd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgsamdrf.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnycvtvs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gydwokjie.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/glharnfei.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkokrahb.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvrgkznf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxajvmj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gfeyyhvjz.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gdgwxeryb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gwixhjxwl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiymkhrr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/grpdlogpl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gnblnqpdj.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gznftlaiu.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glgjvhrfb.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gtzffnlpu.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/groincyww.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnpzqyjx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuyyarvu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswrxjskp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gtucpoypu.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwkhtsjk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnnbehnk.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgzhjtq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfqekiqrp.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghyaixdok.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvuttxmb.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/grnzqvzcd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfsovswf.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbaqhmox.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gofrapfea.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmjkntsh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvncwuep.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gslcxbbyy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gweywlehf.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemhhawz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkidlezku.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gfvwgqlmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gktiddwgp.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gqqnombds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsnyrhtl.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gyunxswiy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkwquvuij.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gcqlovwjg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gcepcitcb.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gridoajwh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqzexquw.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnsxaxakg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gmarpgvgr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjzzacju.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfplvlsed.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gafzswgfs.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgkconhd.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/goyydgkqx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/giduvabnv.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guovvyehl.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoprelpk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxeajqig.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/guzfwkhth.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpfviwvq.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupgvczgm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmyeigyl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfushipi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyqbbeyq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gdzcbrgom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gvqtxraro.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbztxcw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquaorzio.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhcjcjh.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/glhsosxvo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyrxqhy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gbkzurrts.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagywbfls.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghtgqeczj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqmbtnk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlhfcrvu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlohabrs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guesjevfk.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnxvbdei.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtkkrixm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/glseiiitl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gltibwueq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnwulxxvn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwgshwqp.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfafceohm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdurarvm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gjhmxtilf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepfyozql.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzkjmmo.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/grfbnefve.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsyjmkmq.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gornwhnqf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcolifdxs.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgekgqsr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnrumtybo.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gokjsrdrr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfowsbmi.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmgjajo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gnlcmwycz.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoyzbulq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzkjivoy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjdeuces.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqynffdwo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbgcbxhq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/goqnmnmyk.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeaczfky.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmzzrcms.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclrdgztz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsscainlt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzuywchd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtnzitmsk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gskwktakl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcszbquk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvyeqanxa.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuyizhgz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkmogbxu.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/goeyufhbn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkriuogo.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxhxzepwb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqxhxosd.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxpwknpq.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfssgafyz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggyqnwph.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgvcojq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwmbmjops.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiyeaugp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscklvmz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsndgdct.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxmikvef.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzvxhxrv.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcallvnvm.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/giyznxkae.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpqucqzt.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/glwebmant.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gybdoiimv.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gavzyaqol.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gwftfajmx.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gkizaduhq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxmkgriu.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gjcfnnedm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxeatlg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbfrvfp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvqtuauf.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gaosqrisz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhssibmk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/grrefanhv.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaqpyili.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwtmkgz.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gstbbmadi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfeahhip.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbofyppqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtjfncmm.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxbujbwn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gceglbnsv.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gmcumjanu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrpbcqhy.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gonhlhdyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsuerngag.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjamzao.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumxywao.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaswvuhoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwadvyl.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfabolk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqzwytcj.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqdywkvs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbsnilgi.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/groorghns.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gxepxeasq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gintzjetl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gurtnjmte.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdwjqti.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmrqpoas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghovxndgw.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gibyswtrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymsppewm.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/genmahfww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnnmgmf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girpbbnhs.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujklsrj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqorhapxq.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gmtubrcib.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gvekyyilo.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfgcczch.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmamynpvd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfqbkmnw.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqilmij.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnqvcnxb.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbuqhwhdo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnacwcawf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gltgpbfkp.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfimyhwmx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjkfnnpx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjkzfxwu.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiatxfrv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqplazaxc.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpvfommjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzihaucg.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgbngcwi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkaflzpy.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxuefiutq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gujatiayt.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcnqenct.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gfjzwopuj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtubnrbs.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqaemovli.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gottjubfi.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gwlyqnygl.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfbuoivby.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guitscvwu.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjkhszw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/getvehnjo.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtgqypmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gckblnxqr.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gigddkfov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrgxmrkh.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gomzohjdh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggawjpkpu.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtahnkjmj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gflysofnx.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuiqxvl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkshydixz.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghofbhvrm.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grfrpgrig.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbelfqezf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghcmxpsgx.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkowrypmi.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/glhxncgen.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ggekbpspw.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghushlxsl.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcitfckz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhdtzqge.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gggktelvu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpsguqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gkipalwwd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdlxcagok.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guolrbupv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiicluyk.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gklwnimuy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrlsosv.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznzyxivu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/golvvpvgs.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/glxvfcijg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlcpdfcy.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrsyutrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavyqxbg.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvnopeds.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygungfms.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gzpomkhnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gghflysmo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gzncbowni.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/geudegmbn.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqarfusd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrkrlqbh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwhphriz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrhbsgsu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeuitsdo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseeowoor.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigxolwi.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gukffacmn.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhcxginc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyqapudu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuyfnctd.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbuyvwx.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsjjukgcu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gzipsfvzg.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/galimaqgh.sHtML


<!-- 参考信息 -->