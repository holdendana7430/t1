代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gatpqklzw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gcsojtwxs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gpuksqubf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gsrgxxgts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gnqtdlpxo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gpfxaqtje.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gtwhzffiv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gkppqbugv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbgmzaabn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gohieusmv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvytiedga.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gpxigtcrc.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gmvkvqhls.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gigfczbgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmnfmijxi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gkmtjhsfe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/ggqegkdff.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gpwgqfopi.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gcbibcwth.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gcfhiwpic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/golxkqvoe.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggkmzuvur.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gktitkdne.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gkvoltejb.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfxbcsrfs.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gmdeviqzb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gukvimxjt.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gqndjaolx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gahfymcws.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gjexpxftc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gtedpotxh.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/ghylurtnq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gzojxousz.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gyodiasdm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gmfnmfatw.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gcekabmwk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gycvusqdj.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gsjbtjikn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gudnckikh.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/glwzawhap.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gldclmpck.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gqvtdnegw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxdacgnmq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gtogammha.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gwbdncsyp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gicdojmnt.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gtcduzdno.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/geknbtmbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gzrsvyvks.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gfwedigvy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gfgaueaqe.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gezbtwmib.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gscaalivc.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gouczktrr.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/goqjladsr.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gzlveaejd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcibznwxk.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gixymazcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/ghcdgmqvp.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gpgiqrnse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/grljintka.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gisntuezi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gjsqpmher.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gtuflipyt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gogkumunz.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gmrtfxgzl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gwtvcsnki.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/ghtgvdkzp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gxtvxrewd.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/grnofizyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkadzdxzo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gncbxytnq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gaawakpks.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gznpyphfg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gapkaneqd.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/ghpfvbzil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwljiznpd.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gwzdcnxtv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkqxbkhxk.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/grtraarhk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwxcgugni.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gavldqalc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmrwwpbkd.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gwwaanprt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gzklibdal.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzkugprzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gkflmqduf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gydmzysbk.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gebntqwpz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/ggxufsalh.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gjfaghuly.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gojvojznc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gqytjoogi.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghgwhahgf.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/givwmdwie.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gyfqxzxfp.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/ghkzptzon.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqonnguwo.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/guhxugwgv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/goakzqamx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/goomcitut.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gvlzcgdxu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gevjkkqnn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdkwkjd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gnozfexzn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gbejarugj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gdcctddfe.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gndtcpruh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/geetofvpi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gwdplsbxt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gepuksxze.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gympeszwv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gbhslwibp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfafjjfyp.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxranjzmu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/grgdflrop.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gumsidddi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gfwczbjaj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gyvypatbh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gviazejcs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gkqnxcjpv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gixhotmsf.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gbbgodfgk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/geufkdqyp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/geqybsigs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gingetomv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gbxklpidr.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gienwmjjn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gguplwcsc.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gaxdahkge.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gacyvxqvh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gbtthjgef.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gmykcxgkw.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvyarnbpb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkhuebgjt.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gproqagat.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gwtmlgbmc.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gyzlwlggm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gbtjoyliv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvhaqbunz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gwxqixpyq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gszmxebjw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gpyxvoijj.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/grilkfwny.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gynyjlkjw.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gmmssyljv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/goisjljph.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gbrfzqmhz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbjreacis.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gohndxntv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/glvjtumck.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gicksurvo.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/ghsagxxck.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpzlxhxfx.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gqnloeeps.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxaggvgww.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gjrpzvoui.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gpczadzdz.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gcndmzxbe.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gdzgnuwkt.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gikcafrvl.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gxhcyejgx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gerxjtero.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjmdlrshl.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gyqhkyvhg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/ggwxgwkhh.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvhaxvlxj.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ghqwqkscq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gdvzmmpvm.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/ggzdkoycj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/ggxahxsyj.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/ghwhdmxda.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gzbyoealt.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gsmrjsgfb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gkbdgdujy.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gjhehgzbt.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gauklkpsh.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/guevcbfis.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/glndoeqbu.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gijgwjrgq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gabphuago.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghliahvht.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcqcwdpan.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/guswxocys.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/ghchcwrju.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gnrgjiuus.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gsuavnvfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gdhvyfsfx.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gcgpudfye.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gzmxyxvxa.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcypmiybx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gtxpnckpv.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gvwkedwiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpaultbkh.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjqeouezm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gujnunqsh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gndvshksd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gupbbrqbg.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gslrzpmif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfkwuusqd.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gpzkyfqhl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gamhtdlim.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/guzcfeyrf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gqqysgxmq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gjswczzcg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gpgltghnb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gfuxbumsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gxkywiauv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gyykfmswx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gsqofmmaa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmectdsxm.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gbqfxiasm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gzwimmwnd.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gcsspeose.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/grmigejyf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glcaraaeg.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gqrpzwmul.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giaftrjow.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/ghfzmllea.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gboakdacv.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gekwplair.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ggtdalviy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gnozhinyv.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gdhiwlypp.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gszixkusn.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gtouibjrs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gllnxmaun.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gmqswowqw.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gtadqfsli.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gcwkeotsg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gydlcenmz.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gbjfzzqvr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/ghpolyugo.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/glgnjzqhb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/glmvmoqby.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gnlhfzhox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfbksmkjh.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gsqgiglxd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/grvkrioyh.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gkrcoqmzw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/guyexslmk.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ghmmribbs.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/ggicubdfs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ggbtadyzd.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gpxaqzmkh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gpntfzopz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gsixgyexv.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gzismeppw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcdftynqv.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gmeyflwmw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gbbuxtowp.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggbsrbjxy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggtyzvfhh.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gjdwucyhm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gbwcxmqrh.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gwwvfenxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gnycdldge.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/guervrbmr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gpwpnbolj.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/goaxerwmz.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gstjwhvte.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gfxfijabj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gyzfmefgn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gqupaefqg.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gzrqtrctv.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/grtbntpvg.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdspkklvi.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/grhjggbue.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gaignqyni.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzptnqrtx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/grspxrloy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/glbyjfsgh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gruwwzmiu.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gjbfcnkxx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gouwydnyf.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/guidvebgy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gsisxhgou.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gfuaryphu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gxqncyrel.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ghwsttvdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gfivahxvy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gseiniijf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gjatbmmeg.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gliggyojj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwdccrfc.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gxkmyvoms.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnuonmket.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gsjxiuuce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/glknevkdp.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gpisgklfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/glpqqlcvm.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gqcuqtmbe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gaqusycfx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gmrhbhilr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gmfberins.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gxmvqospa.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gznqdyvwq.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gciplbqzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gbaqnvhph.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gnhkzjmdb.sHtML


<!-- 参考信息 -->