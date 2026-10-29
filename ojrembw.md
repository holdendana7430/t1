代发 wailian999

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gyzoytppg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gnjrqspvx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/getcrmprk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gqwwdhrwh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gszvsgoby.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gempsqzem.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gqhmvlhjb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gfucnbolf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gbgnivclo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gianxyusa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gpqzyhvcu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gbkzxcemx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gnzkmecrm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gjkzwzzlx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gzjfhqtee.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gyluohdme.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gigezbqvs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gqltsadrf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/getcyzaki.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gywbibuxm.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gpaeqpuis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/guyxpjdsn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gfjroalgr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gjdzbyvym.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ggzqpwtcx.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsoltabr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/grsuzubmb.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gzwoczjen.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gxythhfnm.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gfhzvsrml.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gyvggfjcm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/glemilxxp.sHtML

);
来源：http://baike.hesvh.cn/Article/details/guosaixwg.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhshblz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/ggatddryh.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gpkcpvjxn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghjuwixyi.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gswlxqwwo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gycwjgile.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/grmnatjhs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gaaldliny.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gbaqxtbct.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxsyhexpd.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gaqhoxspg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbdceqvhx.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/giparqdhg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/guhxlswkn.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gneyfllzi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gorgjcdkl.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gbmdvrnnt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gopzszkqb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gctvwfnbe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gwybxkuat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/glbmvhscy.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gerzvwsfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gjxrxljvm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/grkkqlrap.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gdbgrlxag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gdqrzslbk.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpnvpxbfz.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqdvkoeib.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gpoaiiiih.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/giaaztaqg.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gjivrkfaz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gedbivkse.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkrpbkwde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/ggewuixyk.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gjvmctndu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gfzgxpuak.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gfvdgkbcy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/ggyfgjvrx.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gwmmtpcml.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ghgilataa.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gdeehedgy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/ggilxfyru.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gfxvefppz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/glxtemuqb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gezcbfjhb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbelbsyet.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/grizznxzn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gvlbkodmx.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/goohmqpvm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gezwzzqpe.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gjpujqgay.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gtredxqfa.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gobabeqsc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkmovlqzc.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gpyqbcaku.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gttupjxtn.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gjztvogni.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfnupskff.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/grqzlrlbt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gfbvadddt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gpawygqzo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/grmszhobf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gwgejvrws.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gmljbsxxg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gvimbblgy.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gfcykrtnq.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gwlduffui.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gdvtzuxaf.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gydpcbtdw.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmgstkjik.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gezuqtkic.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gvemxlcys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxztbizvc.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/glcuzpltj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gfperxedq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gyuyvoxwv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gherlcxll.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/glgfmqrzw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gdalibbpe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gihwkqclm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/glchyckve.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gvaiuuoja.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gawatmdhd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gckwgsikk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gazamxslt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gazypmnlo.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gjlzyxneg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/ghuefsidv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gjkxlgfqy.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gbewnchfa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gkianrtal.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/grxuctucv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gkyzfqjey.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gtprkwzzz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/goeftuigq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/girjfvnrh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gleybojyc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gurpevfwv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/guzugkpfc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/greylftwx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/grawntaiy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ggehwpqbl.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gxjsfqekt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ghitvawyu.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gyekkxwfd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gyylkaqct.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gegszozip.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gcowlemnr.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gdddxatio.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gsdltikfc.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gpjkvwztq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/grgbvsdee.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/ggtgwvgeo.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/glfemfevq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gasdqlkxg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnyrcjnl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gdicetbhm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcvurrowd.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gtdjubsxq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gywrjeofo.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gskedljsb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/genmziluh.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gaxhaphda.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gewbzleqv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gakxuetdn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gzkfcxatw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guhhxqzki.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gdphpfkru.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmutmdykm.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gzcetvfyd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvcruarzn.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gbmmqbxpx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gourjjfqp.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gfjkxxhkd.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gkrvtweib.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/ggfbylvmj.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gqksrufcw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gksbxjiyi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gvyiodafm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gejgjeyca.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gkfwowsje.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gncvytirp.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gwqzewfxj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gwfqnkbaj.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/guiyrfhgh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gzvgkladh.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ggexxfiec.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gsjfopysg.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gfhuujcqv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwpnmfpic.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gparanyjc.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghnzctkzu.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gazvnizkt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghlkwbmrc.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/ghpqresdx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/geuipzehx.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/getmirjfk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggbyyowsr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gnbeshcak.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gbmpegtvp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gzoejlqvo.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/glwizzayi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gkrzmmuol.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gzhmlypxi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/ghebesfml.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gwxraftcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gfsasocgx.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/ggppwlmge.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggcjkzokl.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ggskzvbcf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghwuxsibo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gawidahkb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzmesrkfp.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gwogockcd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjrnrnuar.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/ghbkqrzry.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpwwglxbe.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gvppcngyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gxfqvreoj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/ggyrxpxzl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmslmpxvq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gwppgzszg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gyqwbqocb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gnbpelbwb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gsebfpvva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gljtxfuly.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gajdgsris.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gyrtymooy.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gvwaazdbf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gnsilgnaj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gijxgzjyh.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gphohsrrn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmvbzwzts.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gmegcydqv.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gyakprvpy.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/giyefquef.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gezyfqzfr.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gtzfqreje.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gwcekddrs.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gnqipzrka.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/grlbwjsgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/guohtkzcz.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/giobclvlv.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gnprnwney.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/ghcslpxzl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gpxnkspft.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/ggmsjrntd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ghnckgnmd.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gfjccugww.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gpwirrejk.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gqligrsqj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gnzhinbyd.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gvflilarn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gyrtlixcl.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/giojjeber.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gnzkwfxwx.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gchodlkbq.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gtsmznqxz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/giswfrvix.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gxevmhiaa.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gdruopexo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gratgscgo.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gkhxflhha.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gabeyufdq.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gugyqmpkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gntrwlwet.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gnxezwqxn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/guiwuemms.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gwgiciwrz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxdcknkep.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/guaxgrmak.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/ghxvaltmz.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gjrrcterv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gburujeho.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtffwacks.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfwvbkrnm.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gsiqfdnsg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gupyzytrd.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/ghhhlttea.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gsewvazhg.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gbogmprhb.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gfhztfpub.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkhynbiuq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gxpjeblka.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxbjvmagf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gzihxsduc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gsynsxcti.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gwwhsoxuw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/goeiushaj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gyksbfeqy.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gpcjoldfl.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/ghjyxsdky.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmimwhjwo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gyxdfhmvg.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gaqgqydaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gqlieuhxi.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gjmubixlg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gkgnwsbby.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gmyosdzwt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gkexwciep.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gkuxkgqyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gptkpklkp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gdiqihsiw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gaxunmcvm.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gaxcffimx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/goikgxbyr.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gpffwgxwv.sHtML


<!-- 参考信息 -->