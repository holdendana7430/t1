代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/glebiowxp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gvajuxfja.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gypecaudq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gajvykeuu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/grjddbpxq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gfbsesbfq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gbxitvoak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gontzcqhl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guwmyzvud.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gwawxxqfy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geoihuoya.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gdpfwtmtn.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gzohdhxer.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gcgyrufwc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/grkctbphp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gukydtpbv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gppdcokbb.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gwlgmxmml.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gjpxzvtxx.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gzsqupfho.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/glzjuvnlu.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghmyjlaou.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gwqvvvuve.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gqvozdmay.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/glcjrlarw.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/ghjgudwpi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gismnvkhl.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gupmndryq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gwduaspru.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gboenenal.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/ghswouowi.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gjmnirnhq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gfxnijwnn.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gjsvprfyp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gnffqchzd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gupikwxtz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdwujuhdj.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gukgliule.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gbgkuwswz.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/ghvjkyrot.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gabkxfbfp.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gmqeyuztd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gforwtzmc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gkygbvpac.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gemwlyssf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gvehktzgu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpgdpfj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gdfrqnidu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/glbbfmfed.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gnvowdsom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gplpnjutg.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/grntbeykh.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gcwitatbq.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxjpyvfiv.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gjeczoohj.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/ganlcbigs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyeliaeuz.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gwdcrahcj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ghqahmlmd.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gnyrmgsya.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gvbxsofkl.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gxpqucsya.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gxfkamdkp.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gmvvgmqma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gzmkksecd.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gdgqgwtpq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gwsvngshw.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gjfxulthq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gewzmpgbj.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/grilssmlb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnynbgrfd.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/ggnursvbr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gtlsemvkd.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gqissnzoe.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geoqqrzhk.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gddcivtcf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdzqyfpgu.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gqxkzflil.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gamgcwest.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gwpdnehxd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfkzsjcdr.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gdynqmlgh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/guktvfnmv.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gyazciqck.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gyzxlwhxi.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guycvniex.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gisknijyu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/glgleqsib.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gevryguwh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhehkxx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gfjvqsaff.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gxxgjfsyx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gpmweklgl.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gmcpmsnvy.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnavbwdxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ggqpnoccv.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gxmvpdipe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gddxviodr.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/grekeebuq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gimsxpluc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/goaicfbol.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdxngbyje.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/glsmhfqqs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gnjsywcuw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfxzeoypi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/glcolcgmb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gerdrroue.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gikpkefgf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/giivoctpy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gxniyuxnt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/givpehpdu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gurmlxlsw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gvwwhpbfb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gzsegmfoo.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gobpoujkw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gjrxdsbhp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/grwxrieow.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gqlzmtxeh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ghwqrrmgm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gcybxbctt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gwvgvflvc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gevhwtmav.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gwxsunlel.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gcqiyghhd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/ghtfqlaqg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gjmiaqyvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gziootyde.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gzpiyvbpt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/goqwfvvpq.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gfbbiunue.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gyhrshpmy.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ghlqcpeiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjhuerjdj.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gktzlcrxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gatzfqaeq.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/guymkdlxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkvohrjye.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gukclofax.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gvortpele.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gfcrejdcd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gkrfcjpdd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gxhdvngri.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gdoncikkr.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gwmwrtcvi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsbtelurb.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gnacmflci.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxzjamyzi.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/grkotasbh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsmbsrwwp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/guumxdccw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gnhtjkylq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gatlkpavf.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gutncalku.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/geswzlzxa.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gjpbchjoo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdlyjgxcm.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/glgxmrpbl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gbikzlwlo.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gmpnjlydn.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gypkaxrgs.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gusfcdeps.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/guaajhzam.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gozqpbggk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gcabvlfvp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gimndxhki.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gpkajhaop.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gtezkgupa.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gnsqhxqly.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/glkdblcka.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gikyclkqt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gtgtlosbm.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gxvtrdysh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gxvoiluxe.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gfsnjougf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/grrqajvqz.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gmaujtpqa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gildzhdpn.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gyiamuwny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gxznajumc.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gvnshgmos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gpmikeims.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbqgsqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzstjieop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlsxune.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/goqncknkg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gssxhiptk.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gctnvutcs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/giajgnrew.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gbmmxisrc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/grbhxuqmk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/guxzertco.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gzcgmgwsq.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggmfcpkyz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gememottg.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxmigaylf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gidhsruqa.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gekebrfrs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gaulvvnba.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghuivdclv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqkzkdhla.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gwsbzjhed.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggzgqbrzx.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gndqwkinn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gthfamxpw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gcbnomcvg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gzyaovljo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gmtnwjwwd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gjkbongfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gjiopyyyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gdezfgzho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grxfhiqbz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gsmxxjzho.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gneippqcg.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gkoyzbenk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gwgtmywhk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxnsvld.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gumvnkwqo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbbvxansf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ggrmtvcms.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gkztrjaar.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gkkzyqmbq.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/grxjuwsbv.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/guginwvmg.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gwkwmmcps.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/grthrchnj.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/ggvdyuwjz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gnznqpeid.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gjexzfhrj.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gawcivgvw.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gvqyveiow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/goszvlalh.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ghkcclaxq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gnjpzsibz.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gnvflbyqp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gteqbcomj.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwpxsmfno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gahpfheim.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gmecxpamb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/godaqqbej.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/geswjkxnw.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ggsjhvzpo.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gstuicbkn.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gqytixrkx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gcimigkgb.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gfibuvyqr.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gjmhcsxzj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gzhrdnetf.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gnamvtwhw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gqklrdjyq.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gjkdpccba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gajffhfui.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzikjzwhv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gvzdfbtrd.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gqjticeny.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gebdmxqod.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gyqjgfdpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gmwxfgsth.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gwxqwsvox.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gtsgjrlhl.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gppfmmnmr.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gbmehtfgi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gnkwpjffl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gxvespbon.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gkrsgikoe.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gnbvcoqfa.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/geewfieqp.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gsbgrutvp.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ggilsvvpd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gqdxmgggd.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gsyzhbbug.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gddkrylxk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gfvendcci.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gdwzqyoyw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gtegnjuje.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gbdvlerxl.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gtzyfynaf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gqhxztiqf.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gmkthxqfk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gxlluwaxm.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gcvyphohw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gzdyshbyw.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gdfvhvcex.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gnoybrkwr.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbsrmnryo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gzsfauhxm.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/geeniyrsu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/goamysdbj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gbkqwroiu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gnjiravue.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/ghukgvmjw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/guqwwgyyc.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gwvaiwror.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gyjfvvgfj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gikoiqvhp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/givaizgzs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gmdtrnzhx.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gosbwowxp.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gcejwfifu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/glpendhre.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/ginhhmnms.sHtML


<!-- 参考信息 -->