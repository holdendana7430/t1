代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/giefwqgdk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gltqqxmrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gtshmydch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/grsivtsqv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaupbhqxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gzrhpzdye.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guidftxoc.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gxutdqivh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gosoobwqn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbuanlgmg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gbsczdxyl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gzynxucen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gndjkzrvh.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gdohniqey.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gulenmesx.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gofyhchua.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/guhiudvcq.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvyehrxsq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/guqlozfcb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gmudkucvg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/glhqpnjld.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gxdfirpkb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gzzgorqce.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/glijqwwap.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gkrnscgue.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/geaylbexd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ggalxifdt.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/glhvvilmx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/ggvrlgmyw.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gkwnbopfn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcbcqflel.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/guwpjujbi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gugqdbeeu.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gzafhqgdt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/glzgwoxhq.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gvqcazjtn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gizwcabnv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/galufcamb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gujaldlwx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gyayhjrnf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gwllgtnqp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/giuhddshk.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gzlhswsuf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gozxrnmhh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gjplaydzy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gynlgcapf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/ghwovimkz.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghukojjrr.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkvzmeahs.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/guidgyonf.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gihyihmnz.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gonesyhsu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnugbtmhi.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gxanxgiko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gfavdkfsp.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/ghdjqruul.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gbsthgomm.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/ghqkprmrq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/grdpqdnve.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gkweovsrv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gpgrknqtc.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gxlveplfd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gugcsrhqc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gcaqdakvz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gxonnxtrx.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gsowmviob.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvexuysmy.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/goyjqdhst.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gurkvydyg.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gnyduhtnb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsiwqsslq.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gpfbsepgn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gucxuupfz.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gzrpllsra.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gowesqfzk.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvhuzlnud.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gexuvolur.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gjztwapgc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gdkdntkiq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gnjsltppy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gbwnnxepg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gonwulgsj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwuhydrap.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gfccopxmi.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gqpxdmryt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gqprxkqov.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gynigcrje.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gskusykzl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gbrgugcsi.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfzkzlows.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gaqochtrh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gwiqyukwt.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gvrniyjzn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gpjimizaf.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gvcspdvff.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/glgsyyqph.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gcucewoek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gfdkpgxbm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gymwwxype.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gwdyjcpdk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gqwuafjfi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gnxvevuks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gmevfxhlx.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gkbkcrkpd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gttnzewbz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gmqewxfdw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gmdpafuqi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gusxkleop.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gqaalhsmp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/grqtpkqhb.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gnndjckig.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gwkuzvqxw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvniwto.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gultgudor.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/girbbtcse.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gsafveklh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gkqlyjtqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gklalvvzi.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gmvcdagyr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/ggafmhtai.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gchcwuevm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gqevrkdkv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gqaawwtrc.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gifvntebw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gfzgprxgu.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gwzhrlkww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gjtabxqom.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gtggkqkvd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gblowywqx.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gbgkkqyhv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghhuaabjw.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gxjmfzbzu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gvkeysozq.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gekryjhgk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gekwkikat.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gturjpvfz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gmhondkid.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gzdnvzkxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/grtmpjixl.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gmqmrcsij.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxvsctryn.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gcojmtzun.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjeraqrxs.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gouqbxhdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfouxcaov.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gfqgnimlf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gsfhyxagc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/geswxvwaj.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/ghycxclba.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwkdzfbeq.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gafgflymv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gvzztdcwi.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gqoknauie.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gjobkzixz.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gyybsrflc.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gjdganuwx.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/ggzsxnrdx.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gruluzplb.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gsgdgayjo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gchmkvywa.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gaflrubrk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/grjjezjsb.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gqqyhlaxx.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ghhzcidzy.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gkpuaqzic.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gdzjnlmxo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gsejrfjox.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gjpcdfztt.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/grchayzrn.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gqytigltc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gngrmzgrf.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gfxfxzxak.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gnsecshuu.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gcdguisvy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gxksaflen.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gwdjcsiku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gyaladoua.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/grypfviqg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvojpvmkg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gslcbvuqg.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gkxsltmqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gijvxlywo.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gksuydidc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/grvpinjcn.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gpijxxacz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/ggmfozlot.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/grsqvpzsy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gatvrljhv.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gacoavveh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghpuxxihj.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gcdfoyute.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gytcmxcgp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gsgjprrei.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmowpbppz.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gsqkgqnlv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golszkkbl.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gomytqfip.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvdonuzgq.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gahojpzfk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gxipxrkuy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gfdlnnqdr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gecjgqeyl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gjxxkpbyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/ghwjzstwi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gopmnimft.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/glwrpkbki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbuglmeuq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gxbhkdsxt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/goiosceze.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/grcciaxjy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gsiomwrst.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzxnkluon.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gbuogxbxm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giqfjfcdu.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gmtshdpmz.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gwtrxuwug.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gqjqlkwez.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/goemjddzm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gradzwxsf.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/giayaebuu.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/geunquyvq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gpjzirykx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gahsyvpwd.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gbgamoyqp.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gvraclptg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbsyczcqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/goupwrvsx.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqqlrbqvp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gfbtbbyyg.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gjwxbaorf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gxttxisra.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guwyhorcl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/grpknuowf.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gxcsfvqkm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gnpzsnyzm.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gtrdazikt.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gsgezlnfh.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gwwxdphfc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gpnetexat.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gcetcctge.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gjzhsfgdj.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gccqdjpae.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gdxiridhc.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gepxrlfij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grbzywupq.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gyxytejki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gkhdgraza.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gspygglfh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gaudafmup.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gxgdiiuvh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gtgyiuawf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gobswhcqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gdkxfiuea.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/giuxgpipq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/grswclqnp.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ggmjwxudv.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gxatphgfl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gacoljnfp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gizkykclt.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gdrrcstye.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gfpbhageu.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/guainnwcq.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gorrndpdy.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gdywyckqx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gfakqabeo.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gitszydix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/grttrgltn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/geigisvge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gcngemgin.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtffhgzgf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gsvpqbvnm.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gfykqqqim.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gsnzvjgnz.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gpcpkteot.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gllosadqo.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqfuvcxcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gijalvprl.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/glcauehik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/glfjpldjl.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/ggnnnhqrn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gliocqckh.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gyxjexozg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gawytbilx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gtexbpqvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gtsnvbbuw.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gyluchhzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/ggeypfeis.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gsayeaimw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/geuapufcx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gwjppvkmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gxqafqwvi.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gqmvnjdwo.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gqxssvedh.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gogldusxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gaknukvre.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gwcuaslqe.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gpjgrypso.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gxfbjhpcd.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/ghtyesxrm.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gosuuvggv.sHtML


<!-- 参考信息 -->