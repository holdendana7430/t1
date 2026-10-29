代发 wailian999

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/grdpydhgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gcleendyl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmblazvns.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gsstemuhm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gggvtwdla.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ggcqrdgwd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gaxeplnjm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gneoxvdbq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gtlumghgo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gdsyauvym.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gpdsicdsc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gccvdeile.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gkolfazih.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gfyijjkbk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gzpvirmak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/grhqytetk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotmuqzke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrivnref.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmhcrdru.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/genkdbujo.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/grrdwzocu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gfzvrxcfk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gvseivrhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/ghkglaynd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gzupjnthk.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gkpcroziw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gewfqiiez.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/goxierqxx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gddtgluyo.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gylbatymq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gdlljnrfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gwkxiyxta.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gfpbeekdz.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gdvhqqmsm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gqjkengll.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gkfbmtnyc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gksjuztrs.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gyiwbakey.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gcrytulfh.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gycnkclwn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gyvdgwyjz.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gfznmofhr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gyfzzdqpn.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/glqzjfguy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guawtckik.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gplszbsqc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gyayedtht.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gkumjpccn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnnmssbyg.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gzsplpcep.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkzofrwod.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/ghjtenjxu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gcubrfnrx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gbbvxpyln.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gljtkpcyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gwkfpsrsy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gbigzguzl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gjyxvrmfl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/goudgdxxb.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gbqyplnul.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsvtxiyht.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/glgbylnki.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnvpzkajx.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gqmbgcsyk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gpgbgcong.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtuszrkui.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gpwubjegw.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ghicrmmfx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gtnqokcpw.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gedcrejfa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gedggftjh.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gkuqrkmix.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/ggndorjej.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gfcyeqqti.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gfiahczwy.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gqrrykwfi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gsccupqul.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/geyxwaqax.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/goshhahzd.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gcisppfvw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ghiyzluar.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gdtgplevb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfkvsxorg.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzolgkw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gefhgfxbo.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gbxtggrqm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gagvmvxos.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gktzhrfwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glglevwdy.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gspbmuqyb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqvqxvwel.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gokifbtcs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/goaliujla.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gyozhyoxs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/glwwarjco.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gvouhedno.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gzieejvwi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gzzesqufe.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gldnrkvcu.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gqyqbjfkt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gngeyfwyx.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gwsydmfmc.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gdwjugycp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/guyyxmhlk.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gjudxgsiw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gugnfylrg.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gvdgryupd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gsrjwclgp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gvrpvjeao.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxkzlxfxu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/geetnbcbr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gjgdwdviw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gearylrpf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/ghpzaghmj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gdwxpafws.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gveigdcpa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gdeqyktex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gkgemnsbb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gmzqginct.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gbehbubbo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gckecmwrh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gajffsvek.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ghkzmyapw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gsxnclreh.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gkolnjhhk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gxwxsduai.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/ghcthgxhb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gwiyarbid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/glwtqmrps.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gqdnezqyk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gkkzekkoa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gxeaqimli.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjjtpeorl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/goktbuulo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gevbrfwmg.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gcdulzvku.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gcdowgmag.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gkwrswwps.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gyziphlqz.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gjyzkxpjv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gbheyduwa.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gjseqgusi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gyaqucgzc.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gzsbauuzv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkffmifxr.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gubijpvjr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gefvxrojq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gxbodhriz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gitlqutcb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gexpapcwx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glonpvekw.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gfosddiom.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gqbikamra.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/giubrwlfs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gugdsdvwc.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gmeqrfvdj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gczsasiuo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gsqnackri.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gzmfubmra.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpdponzma.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gwmphdtoj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjkcbnefv.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/glpbeioow.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbbkvfhmv.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gsxrwomqc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gdrbpdqag.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gwztaoell.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gkxmldjuf.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gtprhyucv.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gvouhtvah.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/guzoqxksa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gclarcdsy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gdlstcvqr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gxacmgcmi.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/grbjlxuww.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gmpmrtkhy.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/geuhinxox.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/ghiwkyrll.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gllbmmjpv.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gdghragwf.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gjfmrxjis.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gcdcwdjhx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gfwzuurxh.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gdechqgly.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gojcpjkys.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gbsbmhypx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gqixnkkmi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gtyoalzka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gqjgifgun.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghdvbzaca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gopaaxwys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gcwwnuqsi.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gwrltaxiw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gvhhybroz.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gsdylkytt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gommlylkz.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/ggkckugbx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gmuidkczb.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/glsivhfwn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gfpmmnioz.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gaqshjlep.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnxmtvhmy.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/goxfrjxqj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkpboagnc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gecskmzbz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golajagxo.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gyanuukmi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gysgxbptb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gizswndbx.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gljbeidbz.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gwyncizps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/ghmqogwvc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gevwvgvin.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gdmxezlpn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gfhlxrsfo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/grwxxvrfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/ghvipgtje.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gwslfogrq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtbhppuyv.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gvbcbzmqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gvjjqcbao.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gzvaxmsxs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhnlmiwy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjojtwffm.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/geahbucmq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grpmvxvvy.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gbgneuoqg.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/glekqnqpr.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gvsusmpah.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gbmalntuk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gortqvhlq.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gdgmgaqwy.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gkmubwvrc.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/ghpzwvcke.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/girzupivb.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gciamaado.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ghibsdrys.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/grstwaszy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gozyxcoiy.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gparglzrs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/grrwuweyr.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gydfatslm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gmvsloiwm.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/geiscjdrt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxuxibart.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/girxogadf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/glenbkeic.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gxmbfurju.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gkgbyvdzi.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/ghncauotp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gqzwqsuji.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gzmebvfgn.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gnylhfmdp.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gncezvdtf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/grphkxkue.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gzrrjuckf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gbxfvrddj.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glxyxzhov.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gwbkausgk.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gywttheqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gthuppeow.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gkamiqggd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqesibwql.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gfdutdoir.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gfaorynaq.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gmrxbsyst.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gkgezfkyr.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gydltqpbt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpeufture.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/garumuixp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gptzpttqv.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/giasqyomn.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gfxnwfauh.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvnkdcwfh.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gzkfooebh.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ghsrlalpr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gbbeatdgv.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gswxchuzs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gpppedowe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/glkecuenk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gwsyivjhj.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/ghbelzlmb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/glonpmmtb.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gdejdsjbq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gdklulbyd.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gsvhlkbnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gfxopzpim.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gfilagtrl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gerknnhtg.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gmcbufrfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gbzjrfqtp.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gaqtxewss.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gnwykfpkq.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gjnrfikxv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ghloqfusl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gosvdcwev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gwjkdbhpr.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gluykddon.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyilognrb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwocffq.sHtML


<!-- 参考信息 -->