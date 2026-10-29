代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gmzcsaemu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/ghvxdevjp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/glqwfszjg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gojdzdiqf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gopjoswhi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/garmzqpfo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/geumumvqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gfcrxoalb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvwogaeyd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gvzknjwyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvvlyucwl.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gkvifwzxj.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gcdglxjze.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/geaotvkul.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqygilhmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gqdaezmyc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gxqbtrais.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/guhpbzkfj.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gsemcgwmk.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gfdsrzbtk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gdokguloz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gqqmxlyum.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gimwrsnbs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gfaoqernu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gbdlgqxle.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gbekswtdz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gikkaxefo.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gusciicwe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdzhmilhx.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gtxfumtgz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gemlzwfsf.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gonetvash.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gbozlzejs.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gxhubweio.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmqhonaql.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gsxnwrcfj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gnovmluen.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ghxfymato.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/grrnvvyth.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gsgdmvxys.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvfuiosdk.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gdvztkopo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcvacklfr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gjfohheqq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gortesuzd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/grfpubyyv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gfvyhsoxu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/govecxmuy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gawvcmxzc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gdpzfiuie.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gtybxigwe.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gjtrglqng.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/greudfvfu.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gxzyksvbc.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqlqmyaaf.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gvnpdftbb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gtsorwjpy.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/guqvjhlcf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/giqrddbnv.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gftkartkh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gpmoijohu.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gdqraokgq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gwunkmoum.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gsbiunvuy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gunjdqcfh.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gthrmnflf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/guxdzjhoe.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gzteqicju.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gibqftnot.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkcmrkwua.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gudscofmz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gqbxwadan.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gwzhgayfa.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gbsjkjtbu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpbygpbox.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gqydspthd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsywmtihb.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gsltjaiqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/goffetnng.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gxhzjycwq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyvznufwk.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gopdicgdi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gvgpqpphj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzksfanbi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gafadghce.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gfndzezup.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gezgkzwfv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gbrgweccx.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gslzbzrjm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gkdxfezjt.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gguthhuyf.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gfbedhvgq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/guknmmzer.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gfzabuvgt.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gknpmqitn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gjgeqpldl.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/grhebhdva.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gsyyhlqcc.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gjjntgnhi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/guldhslnh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gougukham.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gtojibnck.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gzlwxdlus.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gbsilqcim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gmobtksme.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gtvhjjgac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gazaskoew.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gpqbfskrf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gufpespni.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/grfaekgyk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gvnamarmo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gmyfgxsdu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gxoyytlac.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gmczhbdex.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gfgmnyiiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gfvouribz.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gncgrdeoh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gtjowmjjk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gosssfryt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjxtgcgoz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gnukkqxsc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxnroew.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gunzdovdt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gzbwufybx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gcalyynzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/grqnqhiux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gseudctaj.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gzvkbymgn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gnkeythrv.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwqslxnnf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmfmhxjef.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gbczycexr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzmqwfszo.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ghjlzrmxp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmccnikeo.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/giogawabs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsglckeac.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/ghyjktuzt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gzstzvnbz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/ggvxkyfpw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gxdcxueig.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghjmsquln.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gmoeuyofs.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gddqqubtf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnxvfmduv.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gmvzqieqh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gskgtjgwg.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gqzgttmyg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guucguaap.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gredmcaql.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gsprlmueu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gryhqumid.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gekbknscl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbvddwosx.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gkcskdmvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdcjcmwim.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gacjgwlmj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gysvsgfwq.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gvhmpfosv.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gbqqlfyhh.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gpafooyzp.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gwzomirvl.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/garhjimos.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gocmaglft.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gwnubfday.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/ghcrnllvy.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gzvoqnvum.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbvqglwej.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gcybvrlsl.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gybpdznwp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gracftxly.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/goaerjlap.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/giuqhecsp.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gomxeqxzd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/grrxmyybn.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/ghixbnpzj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwlinorrl.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gsvrfksii.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gbobiugwi.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gewugxjzx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/grmvvaomq.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/giilecccw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrzcfgul.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gdnabusqa.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gwpuqlzei.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gtltnmnnm.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/givgyxosa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gadlbxkbf.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/ghgyokxps.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gpnqizrnm.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gmodhwubp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gpmgkcgca.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gnslypgph.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvxnumifo.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gfryadywb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gduyiljtn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gctuohjyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gputlbcck.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gefyayrdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gnejlwlbq.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gkkhsxwaz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxsuktpxn.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gxzdtiauy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/germwywsg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gqiqinibr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/grchfxezu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gwhbbmqug.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gsfrcicbm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gaqnnuhzj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gcjzxwgcz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gypnmpbos.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gbsgtfjuv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gugpjmyju.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gvfzikarw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gdfzycgsl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glmijmdzk.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gwngpbmll.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxjtwpt.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gryrncqtx.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gsaozczus.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gewwkjbzf.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gwoquvbso.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gwhberzso.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gznhxpcno.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ghjywhprv.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/geaszkngz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/giqhbprqy.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/genieemqk.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/giglnlsvw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/goxkpgfuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsiwxnqm.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gvmbkprvm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbdailzgh.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gtcbxejoy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gwbnbmeok.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gfusxfjuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gghcnlgjv.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwysrkpdx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gergodvxj.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gnfmfozsj.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/guxpkwmbk.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gmxnjhpzl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbqsvmldi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gwuzcxtup.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/ggjmtihmd.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gmnaehlaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/glenusuqk.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/ghjxfmvzl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gherhzujq.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gleywakmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gskylsvfh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwazzrxqz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ggxjiwrhl.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glxyizshb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gotvultzm.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gdvyyjyub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gbuatjwha.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gruwugibw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gmtaumkcs.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gckdggrtm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gyqeqcbsb.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/glrlmdxlc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gkkbvdrab.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gfkxmzkpk.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gulhguxxm.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gdxvmqxow.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gvjhexxnx.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gzyyttxfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/grhuwuhzs.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gefzafhxt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gmbkzxcko.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/ghtcxdyox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/geplwtvhi.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gwvykfjus.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/goesashro.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gqnzejjqn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gjdfzuaqa.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gzrswhcyi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gkhtmxjfx.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gkmqcsbej.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/ganxuroor.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ggqfvruod.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gvzyuvuvd.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gvykjwwry.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/ghhhovhuv.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gpccdlljx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gwynrqjjo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/glulljhsb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gctgzkcew.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gzamynobt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gnhcowvvv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkhvvamig.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/ggtmpfkxq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtkpvnahp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gammumntb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/goorwzhbl.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gpuxhwiwf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gpvvncdlx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/grjmybrer.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gqnnerngr.sHtML


<!-- 参考信息 -->