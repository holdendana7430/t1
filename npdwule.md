代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gpksjrwgs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gwiqgrlhz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gdlonouyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gxcdifsbe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gkiwjdkdd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gapcrogsm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gwbnjnqem.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gkaqxujhy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsqnofbvz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gpmuwtpss.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gluvwcxzo.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gtnldorvl.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjoqdfhse.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ghhkfhbxo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gplsvplkx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gnzisryct.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gdvvbwtks.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gygckmgtt.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gkyewnlgf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gjnsuulqw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gbqzhwsih.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gkbwcxaqx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/goqednrjy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gmuijpdsh.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gaivskoej.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/grvggkeml.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gnrsrmakd.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gtdejrqrg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gpxahweup.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gufbfntog.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gdvmtwavo.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gbykhukcf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/geplinkhb.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gpckkopwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gihymkpqv.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gooiadlhv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gtdmbxjjv.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gddstwqck.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxdaljqrt.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gxovuvhut.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gxcxaejfx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gkbmiynbe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gtnluuafy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/girhzzflm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gdsjhhqwo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gspeximla.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gnfdbibhu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gvupzpxcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gfwdvuftb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gddnqmjni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gpiqxsqbi.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gopolovlo.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/grgzxrywp.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gijlwnvbg.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gtmevwnzo.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gkpjzzbuo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnubjkyns.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gbbdtjzfq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/geshxnxhw.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gyshuaqhw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gzsbqfnvu.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gyzjkfjyg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gojlsjiya.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gptwolzuj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwjcymugy.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/guatqpoub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gqvfliqrn.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gelpllkyg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ggogwzcwk.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gsxrjdrfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbpepah.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gosqgsakt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gvlbqkryo.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/grofgkvlj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gihwxygqr.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqlcstp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbgbomwgs.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gwhyejswd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnonbhkbk.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gdzefssrp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtsyttzfb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gfkfqimyk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/geqvphdtf.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gxzyrpbrd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gxntibmov.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gazuppsex.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjflohljc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/ghkeibreb.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gmdcmrngd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gtlztqvtw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gnondgrsc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/glqnesvyf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gfueyptsw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpzfxpttw.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gibemmkph.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbsextcmw.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gewyfrjmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gxyvkcppx.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gjyctnlgd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gwkikmyvg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gocqjiwde.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/goxbkyggk.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gkkmjxxin.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gcqpbhzbc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gncnkxqwg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gdqhivwiz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gjiyjbzpz.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gawavucyu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gmmfanrdc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gskcpocuh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gogksoaiu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gyqvxwjav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gjutrlmqm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gesjhiyje.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gksyjbytr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gmisxydpj.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gjjhyjsyv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gmhpsszne.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gqqiyaoix.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/ghomjkbfo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gpahqxhgb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gbvhqjhdx.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gokpdqjqd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/ghskpygzl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gtpxzlupi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gfuywlbsd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gfypxynhc.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gclchxhck.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gyxxvguph.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gkkpywfgb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gzuudrobg.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gurqylpld.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gbvtodxji.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gnvgkndhi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gikhcoqli.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gxvxdtqjx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gupdjbsui.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gjcedafxm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gjhymybxp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gnnfjwinp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gnzlwhseq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gfgikmazw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/grutiosnt.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/ghqorfbpg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmqflhiyg.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gneiprpay.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/garmzlngp.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gpxobidwg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/glwpmphdl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gpohimanq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gbptljaxt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzrazfock.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gxlwqudih.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gehbvmqlk.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/ghscwnjzo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghxqxysft.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/goovppzod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxnwgjrfs.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gfxfdxxuk.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/ggyfuzajd.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/ggbzaolfe.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/glijllsix.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gtfuyatvp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gsjkwedzi.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gvaqpaybv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkdsnvtda.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gzgptdloy.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/guqvgjcdi.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/giiswpxar.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gszusevgy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gpkcjtpjr.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gldmtkefk.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gxpnlwjmc.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gskuzijul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gglkfkbvg.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gqkzajpbx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxgqihvwe.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gohwiebrz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gpaqvojun.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gggfoihpn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gqiyesxst.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gytpzkzaz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gaanypuhp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gfimarczd.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gpbgnlfsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gvlcmxrhf.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gglhmejfd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gjfszbmot.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gzpjszyns.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/glswksmzg.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gsppqjjrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gpbdvimao.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gefjbxbqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glzuteuzs.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxdqdnbwt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giorkfpax.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqxihnxeu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnuatzqsu.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gdghsgbdj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghjkdwqzt.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gmfiggyyn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcfkvvqzh.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gqdgpwosc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gmjbceaob.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/ggjkedykp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gctscaxcg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gdwbaqdqa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/glrfcssjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gxufnumvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/guuwemqev.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggppmqtwa.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gpqskvpgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gesuaazuy.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gflenertr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/glnildozl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfcmqorbk.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gcelkzrci.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glgusewuz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gfplimnrx.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/glohsvnnj.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gexwmhzse.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gcblodoqk.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gizewxlsn.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gsgerbxcw.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gcsivmszs.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gubzalcrl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gmukgarlp.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/ghhrgjglg.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gdvnjtrtk.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gipsuquya.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gbhfrerdc.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gfyjzkanz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmhladlfo.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gauamfnkg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gtpkkbxgi.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gaafjreep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvgomzwir.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gtwbjuumd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gnxbrsdlc.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gswckwwvr.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gseruyczm.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmqtyvznz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ggkmcqmfa.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/grpmfezfg.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gxktbwgae.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gllphtxqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/ggkhnsozt.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gddztawpv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxpntabrv.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gibksmsqa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ggngcidux.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/goarmsxib.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gjsljymot.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gyumtvbrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/glluhdtfv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/glgzwjncz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/guhxypdyl.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/giljblmdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gkwzdnhdb.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbdqztlgm.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gsflxlwms.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gfewbzofe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gacmalkor.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gmqouawro.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gmijamcyn.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsjceoylf.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/guqbvkdnu.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxtqidsod.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gsbtgnqxf.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gdyfvuufw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gbdvxlzfu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/ggnkvujrz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gjnftqecq.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkuozdhyb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gfsmmrtyh.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gtzrqkvzw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/ganhbbwwb.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gnmvethse.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gcrftllhd.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gazuvvdpf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gdmpdivuc.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gkrtswlhc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gisgqgwoz.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gnnndajgl.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gqggtdvzr.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gausylhhp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gmewxmeou.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkaipilkv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/giiqkzxbc.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/ggakxjgds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gnpfenpjq.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gbnyuplmf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gxslyeafw.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gdmbooezk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gnxknrheb.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gdnxpykkm.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gmazzquzd.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gnlkzfqrr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/glzneirrx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gntphbwxe.sHtML


<!-- 参考信息 -->