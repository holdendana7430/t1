代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gzqigewdv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gtnakxvih.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gcjikygbm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gydczdboa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqshuubup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvvfejbbj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/glmnbuwtr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gvdycztuz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gfhepoaoc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gzvtgzcqa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/goldccdxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gwhykjtqk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glndmyhtf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/geyallkbl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goynywhge.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gvhltoaqh.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gutdfaapl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/giugkycke.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gecwdjelt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/grwgeeydi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gbcjvfdua.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gvmpojdis.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gaadfmrfv.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gfeigskch.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gwkttnbgq.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gqkidukxq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gfqaxyjxu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gfggxviaa.sHtML

);
来源：http://baike.hesvh.cn/Article/details/guqvujzqv.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/ggwscwvyq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/glgynsfzk.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gavwwuwjh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gbwwutabl.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gqawopwet.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/goyyyhlki.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gxycwjbdo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gadygkltz.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gwfmbnxyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gvwriomyw.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gactkxqau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/ghpeqhndk.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gfbxydpqb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gqhrupqxb.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gutkuxaon.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkszsbylt.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gghgoqgsz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gauqstajl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gklgvixaj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gmqxyshoo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gnjcfxmfy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gxdvomxko.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gmvqlkzft.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/govvhsowi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gpimfsjyv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gfsvwhkrg.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gumvpqxrf.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjzcwympt.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gyvmtlsjc.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gmzeadwrx.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gkiewuxov.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gpepehpjo.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gopveczeb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gubnnscbd.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/geyvqnqwv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gpltvtueg.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gikbjrbwq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gciuccwrf.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/ghcxoejpv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gmihsdkza.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gkhwobgna.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gyrigaobu.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gdmavvrlk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ggobvmjzp.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/glbpdpken.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnovkgqpn.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gzldmorlu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gqoxbbjmg.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gzlmzdqwa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsnpsitvm.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gfcgvsqxe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/goupfchav.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gezkgalzb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grpjbisbx.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gomxrdfym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmexwbvjc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gggtaawej.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjcgirtss.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gyghiueec.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gyfuuacxb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gssdjxlvu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gejmyifyk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/guemxnlvz.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gdlpdsflf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gnfkiajun.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gwtevvppt.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gnuyhbote.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gzwhmkayc.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gdnlhsvla.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gbbywvgbj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gwobfetyy.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/glqxwtzwo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/guxecrlik.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/ghyrobswl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpkhfvokn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gjvikzsoc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gqirzaieg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gizkbhxcx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gpmpqqaea.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gupdsiwqx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gojgjzeyy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/guerrpcvw.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/ggnvmwdks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gmxssvbig.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gjutqfztt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gtywccale.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gsgiguxen.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gepmwxsjm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gdogxwsyu.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gsuodrzjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwjwltwea.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gfqwpjglq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gtdhhtqno.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gphyunzzo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gxfzurqsb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gkzopjxrl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gpxntnnum.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpjuuichv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gddhbzmbj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwmbqilax.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gntwxosoq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gxhlvmcsn.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gkispqbvw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gqroxihir.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/govvclupc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjqwsrxwd.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gljhagiup.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gkfhrjksp.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gbciyqunt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdezxvjeu.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gajjowsyv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gezedcivm.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbwvxqjnb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gvdxnpsax.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gnjdisibf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/glhaotqej.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gpcvjmoih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzwlmgwaj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gssyoqhci.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gpkumwjiu.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gpaxsouuf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guupiykpn.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gxljnrnuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gozrrdpmu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gugwbtpbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gsvmknrbs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gghvnhpmy.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gusvhkiop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gadhiqzyh.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/ggfpcvdzj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gbehqwcdx.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gtqdmzxxd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gujuboyns.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ghaztjfas.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gswltmekj.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/giscykctv.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gyjuumdkm.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gpjaelfbs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gqbcdipjg.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gqpztthup.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gncvfpuhi.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gmvhwrwdz.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gjlatlegd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdwdokosb.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gfotssdkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gqqrtbtwu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ghdhvzscc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gfizhylka.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/ggeymaaki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gieoqzozt.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/glorbifca.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gyyyjewkc.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gkwetjuwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gyoluxabx.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gahayrilo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gmqfxtaox.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdzrzsbym.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqndmwmgr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gkktsxvas.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gctqwovib.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gtkwuwnxq.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/giiejgwij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gmqaypvbf.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gdkausboe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gariteksk.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggzulymod.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/glmbcvgyw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gtliiaraa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/goydatoec.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grlkehgpj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghvkdabdj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gfiqlwkib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnmoeow.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/girjkjwvx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdfsmniku.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gbqrtqafh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goognsdfo.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/ggvsemhhm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gcpuegxjf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gbrvcutif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gtwdzqokr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gjntgiiln.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gmagjybrz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gaemnvtin.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gpffsjibc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/grevuzoes.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gjozzcigz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/grjfpskzc.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gfdjrktqs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gkdpcnciz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymdbiahw.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gprlfldsw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gttdlddrq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gcantkbvd.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gkqqjpjzq.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gdsvomzgb.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gqrgtxpce.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gvtxzwyys.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gufgtbjlt.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/glmyybabq.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gbrbymamq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gkveckbhn.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/grhsrheic.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/guqljbpab.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gzmiwhkje.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gembnvtaz.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gulizduxp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/geqpzzqml.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gvvrwigmt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gyiksxaxw.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gwagagvnz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gnxotrlma.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gpneurteg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gsdkkhtum.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/ghastbxbr.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gagbxowsv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkoqlxdke.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/glqrmfqbs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gfvwuqpir.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gvebwxwhp.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/geklegxlx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gpxbbofql.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gtxfubuft.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/glmpndghn.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gxldkfnoc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gsodcfumr.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gqvjhnrdr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gwffqxunh.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gmtgdoogz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqulhcrjj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gtdalpvjs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gigeewzwn.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gqjuyulif.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gcvwxeixk.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ghkordieu.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gbxbgexme.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gkwzezhhu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gbjjhxwsi.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gvojduwfi.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/giffincgy.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxmcufjhg.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/ghdvxdpzm.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/glqqoplzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpvnsnwsl.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gabibzqbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gqtxgcqsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gdizlrwwy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gxhopnhom.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gznytdcth.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gieyuygxi.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gyyzuwfsl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gptieenqa.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gcpztyjja.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gttyoxxwq.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxtoeuwwn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gqiihvxzn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gstivkqje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gilgcitjj.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gechjfegv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gzeyslywp.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gmdvjhvjj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grlpteszi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/ggpbuxoys.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gssfauttd.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gneiuuwwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghjkpryed.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/guzevtrnp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/getemxwfl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gdyfzmwyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gbawsyhqm.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gzesvhqlc.sHtML


<!-- 参考信息 -->