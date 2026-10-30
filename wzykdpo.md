代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gehlmkvjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gzpeiskcg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gvmgpvpls.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gbwrgqvof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/guhencmtn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/glqhugfde.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/glplbfswm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gkudnaenf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzpjieczy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gvxylaqfq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giehxhnts.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gujycvbxw.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gxsytwuac.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/guxonfzfr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gvpnlderh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gocwmilnv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gfavqdefb.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gmygjpzmy.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gitrrnjiq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/ghfmutywg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gwyytvose.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gipapfyex.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/ggrcuzbqn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gvebopbge.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gfudkxmpp.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gjvjebzgy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gyuelaywn.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ggrvncjfe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/giggaavup.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwhlgddfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/grjdncdlm.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gddfwzawg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gwikrigvw.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gypnxlcsf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gpsvxiwoy.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gogyigcxa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gughdolba.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/ggevrbtsr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gnquueffm.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/grugygeke.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gtjzarmvq.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gtzcaswjd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdrtvzxbi.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gcftuwtxj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ggsytayat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gvqineurk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gcdywbvko.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gebgipdai.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gqbualoju.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/ghyccljsd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gtzdfbtfk.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gwyxjicbu.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gbeklokbk.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gwjfegima.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbcqyanga.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/geodmjmkm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvffmlzj.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gkqzbehgo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gvrsbbkjt.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gfmtsmriw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/ghadkdrpl.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gwjzphcjd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/glldaviwi.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/ggtiknqqu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ganttxvrd.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gbkkyhxfo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gyybvcecl.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gixheifvt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gtvcpmmjf.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghcfvrtfi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcjakilbp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gzetmmpxy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gtvcchfqe.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gdwlbuggr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqrvduuyb.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gocgkprse.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvajbfwi.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gznybaqcr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gewrvfivy.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/ggjfqtzss.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbszrhsmu.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/geqmeqxuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gyqiamnss.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyvseagdt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfxhwjfdj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/golcszjbq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghdpumxwh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gzgxkyzvz.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gtklaocka.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gndwktvqu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gmpublvsx.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gyukosupm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gzymacblw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfwjypsje.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gduvzrrnk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmiyontyj.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/glyvtekto.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gkginnqxu.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gefyahgfd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gawkopfcw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gwfxbkmlw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gqcxeqhux.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gwhumdqeb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/galjjxraw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gcnxshfox.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gmtkouifm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gompuncdu.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfiburavr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gqbtvnwga.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gapcgtghc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gmhfbnnju.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gvzfryppz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gzpgzmenr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gsqbyqlri.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/ggkrnvusc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gdzdtutts.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/ghrfcpyqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gmkjvsubl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gcxrwuqdd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ghptauiaq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gsjjpwlth.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gpofsjluq.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gekyhanzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gydwqepbx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/ggayfjntv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gldgzzocg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gptgokybk.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/giwdujoju.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ggufiwcvh.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/glqgyacof.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gnfqneopn.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gmbmyjijs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gchyqccms.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gejhpiyrm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gwnodxqti.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gvxngsgyr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gbzoiwsen.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gwltzbqgz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gtanmutsn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/goojvyuxp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gjzvbtcpq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gtqmuyosa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gjazloeem.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/grkqsypft.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grulxzaok.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gpxtshzdv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfxicxfhm.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grpqnhtvu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmxzodtux.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gbivsekzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gjvfugemm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gshcecubg.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gwsplaufh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxdltoufj.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gvluqcked.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gaozeytft.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/ghmwpmyoq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gyjipcdyd.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/geyynxzkw.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gswhxetzj.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/grcccmyqq.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gcllcerro.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gnhjnfhui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ggoosurpl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gigfihrfy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gvfrsdxay.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/genwhqubn.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/ghvqtevds.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/garbtausr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gtpvytwth.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gljotzqgo.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/ghoijozho.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gtgaxdgtz.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gnxckojcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gfjpgzsqj.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gmurthlyg.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gzcelmpwu.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gttgiosgs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gkpzdylds.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gftunxpio.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/grcvjlilb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gaaprzjjt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpqodcjtg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gjagdvdel.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gezmejuae.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gydefzgsl.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gczcwwvqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gokamvmbq.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gnklxytzc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gobzirjno.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtifujfka.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gprjquepw.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gbqwtsutv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmomypapq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gzwnpuscd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqxgtojmo.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gdnspfjiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdabynzpw.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghjukgman.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjucuybju.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gnwxaxdqg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gluidhclt.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gccjicrhv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gdobsidjl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gdbsdlviv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/grpmchnfi.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gxhbmyyqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glkeigmtq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gzvxivzce.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gehjmmsgc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvhdmetiq.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gohzjrzxo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/givfzbste.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ggdzwmmws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gqjtextqu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhneoqra.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gjoweawmf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsyajikse.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gujzbdlpd.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gcciemrud.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gszvutvqq.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gnziwpema.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gqgfohoxp.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gzjiqzhav.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gvnkzywtj.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gchebqynu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gskxtyurd.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gvcvfjiov.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gkfclkzia.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzkdeuyql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gwezcjxdk.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpqxrvtqx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gjmdpugsj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gnvezsyjg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/ggkvquzpp.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gzdhljmxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gusyvxddd.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gatxscprm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gpdamljsl.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/goggabwht.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gfbpeebby.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gzopclxmb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gtrypbclh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxjwfsaxb.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gcsonmucn.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/guzxdfihf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gtlkdpdfs.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gtfttwkwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grzwekujx.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gzrhcjqnl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grarguesl.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwiieeiqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gacbdsyol.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gorxhyuhh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gezjnxreo.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gmsfzzzsr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gmldamcde.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gjdhibrnn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gstkukkyz.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gescnwxtm.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gxjiogadk.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gupbxscmd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gakworggi.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gqqavqron.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/ggcmgixiz.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gcvlmedqu.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gsxibxsvh.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvgkiedpu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gqsxzowxp.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ghjdhguyg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gifzsqems.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gcshmonuo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gqvhrslyk.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gnhwdryxb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gasdhsfhy.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gqqstdoqr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gquzptqra.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gnsvprvxl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gqklnwgdo.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gdkpeviwf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ghwcazbhf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gsihtftir.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ghxufuxwz.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gdegpskyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gngvkovas.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gpgkdtyus.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gaguqdgum.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gqebrpmbh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gsnansqcr.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gwjzjtjjr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gyortoext.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gdcucwlat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gfbphqjdf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gfzoizjpy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjigazmci.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gndckuvhq.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gvejefqzw.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gciepgltc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/ghhgjwtui.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gwkiergln.sHtML


<!-- 参考信息 -->