代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gomalxqne.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvbdsxqep.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwokckafj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glepoqggd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gcofzunxf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkjhshd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavknuhv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxeriywb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxcsqud.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxgsiiqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/guffvoksk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhorhixm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/ggcrgmwig.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gkeoazqat.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvsskmi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzewwwzw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gketxoigm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gigkdqijg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geletmxgb.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gblipgdej.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gjsmcumnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzktrletc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guogyemws.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gtgtjbqfa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmptsijy.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gkavvrxdj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxdzrzk.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gczgzqerx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gbiguccvl.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzoovtbj.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnvajzl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqveytvsl.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcafjyugd.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwjpngli.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqjxplo.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnwzxhsxk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvvzylan.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gijfqhvnv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbmourfd.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/ggncmmqdn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghijjdmpd.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrzqfaoz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhyzgbtj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckowxbbr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gcujkstvf.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjxpuxufn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcxqwhgd.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gpzpcnmrq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvnsjafv.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gloqlzslb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltqjiket.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvafzktoe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjegmiz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gsngbejiy.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/glqvksadc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gdzdlcdtw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvczsfrcx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/grxntwdry.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnlbdkjw.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gyezhngke.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbpgjdyd.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gusnuywnn.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghozcix.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gseavxywz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzouzxxqh.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjfsoeogi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyruldk.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gllfqumpx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gsklevrsv.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetflbuf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzmcjgaf.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzcoxtmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkosqtams.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfyegvph.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbdntefa.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gnydajqsa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gldpczrcg.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqvrmtmj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvhqkbfdw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpjtbkvr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgxrevnv.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwotfmne.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfrqxqwm.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztgrtpjt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaypryxx.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvtvdgemg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaphubpo.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gzegdgqpq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwkfypyn.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gngbbddhi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkjviojs.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gorwaoxkl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqleczerx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmpikxwe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geempnhhp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gwtyamync.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdlxljz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkynbalgr.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gglpqcjsm.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxgyfeep.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gbrhfonmh.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbpctszwh.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gickfyqpa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioybolk.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlcvuufx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guqjlldvv.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gopptpaca.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gijpujkqc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkhtvtgc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoifnafx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwtwpnoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gbkorfedm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsjpvxelc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/giasvefeg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gqeendhij.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzivuumoi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwrgtkq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxrxwgq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgnqfbc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gopqxdnkw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzyjuuvy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnirwwbdr.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gppmnldmq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgfkoins.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gemvfkrkp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/grtznyeee.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gdguswflq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gawyfdhow.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdciqjzyg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsowdog.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpzhuyrg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfvlbhnk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhopnzdy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbyamcxw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxlxpdpb.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/glkodpjns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjywypew.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gkwvtdrvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtadbmjd.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gkspduoyo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjxlyroo.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/guewodefj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gevpcesrr.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gtaiovanx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgtpppjd.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpkpemjq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gvnwsjsyt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gfxdxglfi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyfixlcj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/glbkfuiwf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpvshnhn.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gfxiqxerl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmykqvhqo.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gikeilmxx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddcakbxx.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gxoaeluxx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawssyeot.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflaoxesb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdsvxijp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjnxxfdp.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gdebkvqop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbyzsjne.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmyyaqgn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxeoigsb.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggpjitspf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gfemlcete.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisqtzqlo.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzbkpmdt.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpsmswas.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gookoznch.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gnuxtwgrj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/glhndztpr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gnihycimd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmagklvi.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gsfmifzyv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicseoah.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbrbhvay.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmvvnnjx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpskkyvh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqrwbqk.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkoxmzmt.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/ghseubsnw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/galworqnh.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gcfgingxu.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldlwrlz.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjxhthp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gbkswzson.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqdoqkw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gqbydtsbt.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/galycpwoq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkedubsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gexrlzrmm.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/ghocbpmhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/guodupdlq.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gmcbaoiui.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gotuwtsgm.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqyawewag.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gejqrtrim.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyyblhab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/glrwglyes.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/getkgovje.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiyankgn.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxcyfkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjhahcxh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcxxyrget.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsgqidbl.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grqxtxtlf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbakisjn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmqpatfu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmobxjyex.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfoaktvk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmurxxok.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/ggihuvpzf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzdubfi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzmbnxvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gbdurccjq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gtwlzpxqn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gjipvtgpj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkerwthqk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdaoqmkh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfyintnhh.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/giwubqbqd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyftkguut.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpfoqzpee.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjxbizpm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtmepctvs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfxxchqn.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gxripmngc.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gqbzuwqxe.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghnumvynh.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gizmevvva.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshrkbih.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhcbuuws.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/geqmosfsd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gslnegvkh.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gogxlxxcr.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpyjgagh.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gpvrjzgql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjarqhlp.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbapfvtpk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grkededfk.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxavokeya.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnxiclxd.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxxffjvat.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzyobpcko.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagzxisd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gteytwpyc.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gngnelkha.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gciktosou.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvnwapuy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmdnswpk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gddiysmew.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gdlartnrf.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaacodigj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grvucwoju.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grnpiqgpu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guvodthpp.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gakryqmri.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmaxkraf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giawpcxcf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbefpuoua.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuptaxhh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmtsmilzx.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfsxjpqa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsfvhctc.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gazlugpdg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsihdwjgg.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/geyaqitjb.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzyjfcwmq.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdsrmivm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjpacfu.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gnnmwhcqr.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjjqlsgx.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/glaaznyxv.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gekavwpxc.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/grrvmjahl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbozfnss.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdooxfvet.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuazyxkj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gtqupefjj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwxmjcsb.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/goodsatzq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gphuiorre.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyejffdw.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbratzspq.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggssttiyj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiqrvrit.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwtpuycl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/girliniyb.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvokxccpz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnlnquup.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtcqoeagu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxplmlcf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyxcobtm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gshngrkwn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbwpayxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsffpdya.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhvphfzz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrnfjzlm.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdkmwhe.sHtML


<!-- 参考信息 -->