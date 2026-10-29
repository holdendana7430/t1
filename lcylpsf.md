代发 wailian999

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjnvmeqss.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gddfydaut.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grtkpphuq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gvorrfghf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gehqsyipy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gfizyliqk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/grvnkfyun.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gzgrpaojb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gebqvykgw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/goibxuekk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gpcaimgkg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkujqjsgw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gegmrmumu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gtxhoksom.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gfwconrjz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gvkindwki.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvpmwnwpt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gvxvrtigq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gesvihxdy.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gbnivrjod.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gavvvqpdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/govdqkylj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/ggdraspwi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ggkaturnw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gkhygcteu.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gtnfhxzla.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gwvuymmht.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gduscslis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gafjoqgnn.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkaggxjvq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gjofeurod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/giklxtoqg.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gnuqqwzvb.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gjzyebuly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gfmqoafut.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/ghggrsrla.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/guwcxypbf.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gopzzlrbp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gevwnjaem.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/giyynkvzb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gxmsjmwki.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gljthwlfv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gwkjeljjn.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/glbgagqgw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/grrxbncle.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gfrwwixtv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ghcuezvys.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gyxfpqddj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbiofhzza.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ghykklplb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gqhsscccv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjarbbnsb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gdneibntc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gphkmlagf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/glpbwoubn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gloepghmo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gwutirquv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gjovgdaaz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/goqdgkepo.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwzzjocuc.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggdmedbnl.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gfogemkni.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbyhwcclh.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/giwykajrr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmxfwtdlk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grofqeluq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gkwriodjg.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gqwmwmbwx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggarqmrnf.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gsasnoebu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gbfwludpw.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gyxdcyyxz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/ganuazygp.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gnvquxmox.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/ggxxdmdhc.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gusilxaxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gogeyueev.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gdpzxkoog.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcvtfjqvf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/grqbdkimy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gisyjmlcg.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gwqcqqfdg.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggqlahazq.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gxttinbpn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gqiwktaoh.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gfpbffprp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjtedamzc.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxvwfrodp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvcdlpggp.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gaefpvyow.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcyoykmqd.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gcrpzpnfj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/glmcubmjh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtuyoflbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/grritweky.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ghlounhoy.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gwhumlcib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gwogrzzet.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gkjbsbpqp.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gwqhmhehf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/grsnpelvc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmllkmhrf.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gqbbiltvo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gllagqqjt.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gsbduejag.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gdexdpbaz.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gwgpedszz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gzcbgxzcs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/ghjjkokgv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gacsjcgoy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gphwktotq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gdbyjerhj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gyjdrzboh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/ggtuzsbag.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gjqzhwvzi.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gzjmbsikj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdxovoc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gkncydbur.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxgqfahub.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gsnrqcqer.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gquoelhpq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gdxpnswjz.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/grpaikciq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvipzhxg.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/ghbdjkjyx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/grwkvtgra.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gcljmhctl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gkvszxzpi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/giukgufab.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gybflwubh.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gvvdhsifu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gtpicdnmi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gbvpomqiu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gaqkpqybx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gfepwkuvt.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gzgiobyru.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggacbmblq.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/ghwxifbzu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/glzfgxgxp.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gcvzrarhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqywxtrmf.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gnypgelzp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/galmmafos.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gwtjphrsf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gocphvrrv.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gsemrwlql.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gpwzspbas.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/grroimnsy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gpwzesinf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gsonoerat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gmggkgpbe.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gkznhfhck.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghryuqsig.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gbuzozmsi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gemeqduwk.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gdseqzcjz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyllrxuzp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gmivnrwhj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/grgmdqpld.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcjxqniqm.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gvchunibb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtjxgfuwn.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gxdyzqgtg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gfoejcuns.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gacvrxeuo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gteafmuiu.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gzsdswrlc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gpmtusxug.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gvqctkjij.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gqhzrovet.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gxvxyjpgi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gvblupkii.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/ggtgfzhno.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/goseknetv.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gynjkmvfy.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggufkkqgp.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gigsigqtt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/glvdozuca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gybqoyqop.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ggejkujyw.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gkxepongc.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gtwutnasc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/grmwrkymw.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/guohzzunf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyzuntoec.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/goifhtcuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gfsqiktpt.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gcumyreto.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gqdkqpdqh.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gttsnejqy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpsvqmuuc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gwltbrinb.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gtzymfkjb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gyjhhsynx.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/grjdlwqyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/guswypedj.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gocxhrcbz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gvxdfamjg.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gawcvbktj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gfpfmoarf.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/glxhkqjwy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gyxkrmxpa.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gdqqyfxcs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gifqnytni.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gnvcdmccu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcqxyfdkb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glbqpmoci.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzfimatke.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gwkyykvly.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsbmzqgsb.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gdrpxutzy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gewtlbhrp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gsbqzdreg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/ggfyddzhg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gasjmgekj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gulptbpqd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/ghtvzvzpg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/grazweswx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwkinynkc.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gjpuxaquy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/grorzhdrd.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gydwkqavc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gzsuimxtk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxrazoauk.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gzvjpwadx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gztamtaxg.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gfkjvftft.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gohbeseml.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gdumpcjia.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gxmbljhif.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gpnvjcltp.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gdrvnfect.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gajolzobi.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gbkyjvdel.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gpwnkugcr.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gtewxuavm.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/grfuqyerz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/ghvjopdmr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqdojuhn.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gqbhsybng.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/ghkbjmnie.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gutxzutck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gugjdnxer.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/giytbjfdn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gkujoipos.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/genjlrjpr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gssqjiutc.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/ghgyzvnra.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gcvsmlobd.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzmftruab.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gbjpvgaxq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gsueghkko.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gugjuucvm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gjzashexf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gibxiqdlk.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gvuviottw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtgumoays.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gsouzspob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gstanjhfg.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gezpiphbn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ggvnpsawl.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/grczvgxes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gvddnxtxk.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gvnufslnb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gajohlzjo.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/goaffrcla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gquzygrro.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gzhfqqhyc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gxruggzgr.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gsgdsfhmd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gcjyfydba.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/grzgqftry.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gjmnifsxy.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gijljbzaz.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gzgxqhzhi.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ghrihuqlz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gzefqsais.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gzikbgrlf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gbakkichq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gfjwwzgpb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gkhnqxtws.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gircxczwp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/grvpodyob.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gwmilbedx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gyzaoujoe.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gapijcyma.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gffrdfvff.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/grwakpqds.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gvjfydknb.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/guyjcwiln.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gfyrzguaw.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gmbozwzwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gkyhugpfk.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gokwfdzbx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gnhcvijmd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gkzwzukjd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/ghalqlftc.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/geulgpfxe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gtrszbryk.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gavdurxgt.sHtML


<!-- 参考信息 -->