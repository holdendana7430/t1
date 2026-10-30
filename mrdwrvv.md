代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqmgvrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnagexn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrbulozl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxpxoii.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkdtveq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gswiukfgu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmsgmmen.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxaafaijc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gkrkfrjtj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gmyktyirx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gghejvuyw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfzpfkoq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmexqiqu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gavdffgzy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gejejoowv.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvekptusf.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxmwjqkp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gyqwhqwxy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gdoemfhmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gxootgjmd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqzsyckt.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhzkauuk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gytvafsfk.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjtaariw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gdbybcgsk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghxfbzpr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneoutduy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmjbtsjr.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/giijmtria.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyjvopzp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamspezic.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbriohlfe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gdosjoyid.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gxpxdvfyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gttqidyan.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyqkiigy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoaxruhh.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfvjyebp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrwjmgna.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gxgegvrun.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfxyasvi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gsclaslth.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdsunsve.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnpoetn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmbjokml.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpkoxang.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbcfoatb.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmooqudt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gcxoeumqo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gonzcetmf.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gwitkfzlu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgehdbsu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gyvkxjkim.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrqnwwhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/grepdaicp.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvpxcevp.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmzropko.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkpjroep.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gimwrmmrd.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljjlvek.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiagfucj.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjvzmapi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/guxbrjhsd.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gidqgbblb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gckvrjyeg.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcebqmekm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggtwgjaym.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtutabdx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gkxqxxdbd.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvzojuheo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhgvixx.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijdrwxu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/ghuxhvxhm.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gotysrkvg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhicdbqd.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gqjciddmy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/ghatvpcko.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuewakpn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfxomrgh.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gkpqwyfnm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grollgikl.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gfnkjurvv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkusarsfe.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/glharnrgo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxbttukvf.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gkhovaijd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbwyywgk.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/guhfyltls.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumhinpgw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnglmuxwd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwiqikzt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gplhaqdeo.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gfmstjauu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqbytfyk.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gghacdrxg.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gicbzklwb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/grimjgbqh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswcrjgoz.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxgywzum.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gcxramivm.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gvutzggnt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvsvrkac.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtazoirfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/giihmwzsf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmyxilpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcceseskj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaejjhntz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gdwyshihk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grpoaavvr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsblmyjr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcudpybv.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjrrezsya.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkyoiqov.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/giakzalrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkegfnjca.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnrphiqm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gmlaihjyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gfbimeahn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxdquyh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwllbcmt.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupewobyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastykjbq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbeexkya.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxhbotax.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqzpaxqal.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/giydjqzxf.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/grojqhiwt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gaimxnbwq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gyyqwcpay.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gliqebsxs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfsrauvr.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzcawqoj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gagjsenyp.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaqnyhno.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdfbjxdd.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbioxamw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxedozbz.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqvhmha.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyafusakt.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrwdacss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gbyrspsvm.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiafgmtj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gazfouahi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gahfqqfwt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazlwckic.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gwdtzemrt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxqeevab.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gwvevsolw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehsqamt.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/guwecfpvh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcpvikai.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gvxtvmhkf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtedenlnd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gkfosmjke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakfbbnm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjssqdcfr.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gspkhhkkp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gekwbbmqd.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjusvawxc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyofrqzno.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxmnrqz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gczmqduze.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbydqmmhc.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gufzzhwsf.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmynpyxzq.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrrunruu.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzmymjmiq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gqkokxajy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gisusnpyf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeffrrbs.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiycpcko.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgubqmn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grakntrrt.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/grulbecld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gkkmwsamr.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gguqramyi.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfedtinpt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrwwwljt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqslnosk.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gjegmmnmy.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grpeelhtb.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gpllwiihc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhvhhwne.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvhrowjee.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeuyzuer.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiwdrawc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxahuaig.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpndpzbs.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/geqrpotpj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/glgmrlgae.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gxutlzchh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijkczpa.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gopukuxty.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzgtcxjl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkkfndv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxwrgcsk.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gdqdbgvns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhyqdayq.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvrhfbc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbuooumv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcilzncum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjtevyd.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxwrophf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginctqgcs.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gliukcbrn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpeyoavt.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfwtxhx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqyzwlnt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gwgdbzqcl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmauvybg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvjlciiai.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzphehqj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gojnsgaqr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gafqjxrdt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gednzbnzd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnribczh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbsspyqi.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/guksoemiq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvdtumnn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcrcwegxm.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnqvdys.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmmphwc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gzzxjuuhg.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gkxhadsuk.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/ghncdftlv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygdacmfg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmxzhhqh.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvicbiqpg.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzosnnoz.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxpmtrxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpenhakam.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gqynozuvu.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyycpfqp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgdpzibj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexvgbita.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/ginarklyy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gtzasbanv.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gikjxympj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqreffthz.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijxkosb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzqyzij.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gduarurli.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gptrhkrfo.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmxvmrmn.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gwmyaurku.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggwnjppxv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gindfjtgh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcsgjzsx.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgfebbpv.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxtnpwft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegnpjah.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnrtxhl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gudljtyne.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdcsoazv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grauqjout.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffmcqhmu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcbqkfmzw.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsvnrhzdh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsahdoih.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyebiiuri.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeblzqkz.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtakzpuyh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grntqhphc.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gofwjlqqy.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcdowtzvr.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gpjlbuuwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gopbuxyrx.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gysdvnqqn.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gycmxamhp.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdpbvuih.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxwsfwawx.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhgkkln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcsdwzgl.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gofyaryxu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzkpuzzds.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrnrebfw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujdlmmk.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrkxrxne.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/goiobofft.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gymqvwtmr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvuhozhl.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhfzqfsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gatumqxbx.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxchwkrwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxhranbzg.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gidasfker.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvdcxkrr.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbnsdgto.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyoxgxky.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtryqxlj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/geywoseac.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjbrbsmjg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gtfqgnwyd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gqtikwcna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpdhiwhj.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gmzqxsqoj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgmbweuh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsxjsxip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gnluagizy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnntfsmuz.sHtML


<!-- 参考信息 -->