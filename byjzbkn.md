代发 wailian999

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gvlmsvbrd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqplfrsow.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfhbcikne.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/grluslagn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/girhewnou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gjvkibgfq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gzbdvcsya.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/guzzxwweg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gnxgcmmlt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gkqhiqswn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gapwftkfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqvpdgcpq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gesbcnsmn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gezwbtjpv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/guacsdhmr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/glihvlown.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvcyvqtyy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gkdedqdqx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwchmutzt.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gfyhqcslr.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/glgeznmlg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gtxpzbitk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ghdoullpw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gluwobkhc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gmnkummiv.sHtML

);
来源：http://3g.hesvh.cn/Article/details/goxijsmbo.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gjpvtepfe.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gxqioypwz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gisnyseds.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gepngztxm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gspygmknf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gyducuvtc.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gjljsjlpz.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gatwkiftl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gfklrhwvd.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gharrvwiu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gsudlnafj.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/goynsxzui.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpoghofcv.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gqpfpavni.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gptshjbpa.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gqjloemgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gzpgraplm.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gqptldhrm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gjpfcnefe.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gcboacehb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gjueqlhkg.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gcgcoksze.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfdnlmmek.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gkqrqjnbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gbqzjanne.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gspkfxaxa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gcumdmdwt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gylqnuaex.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/ghltgochk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gatkmmhmr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gsikwyhbn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/ggguimcqe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gqlmchiac.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gzfhhpclg.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghypedxzv.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gxhcttalg.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gozvxxhcy.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gcsdthuhl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gpokjkbjr.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/glwezbbvb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gmqokmgdp.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ghvdkjesw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/grrswusdc.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gygylgclv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gbwrgkttw.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gwlzyfyfo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/geunvwtoy.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/guhuhhzko.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/giyzohins.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/grucbajyq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gfctjsiqz.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/guaoruqoa.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsudyhiuu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gemlvlnhp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gwfdnsbws.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gkccmxquf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geyfkmptx.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gdlsnyztr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtndtllqb.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gytgmcubu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gejdfmogx.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggierdvma.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnazgcesf.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/geydpcbnw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gxityxqsr.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gqlvccqnc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grmiaixkq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gglgmxmdq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gyesfbzrt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gjkdswciy.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gopovriyq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gqasdzxei.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gdosgvpga.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gsdxxfsex.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gamqnaole.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gavyrwjon.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gqzsyffif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gzpmmsuss.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gqmpcglxf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gxisgkckn.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gbhkipgwe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gzqulafdv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gkwhrxycp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gioquzyca.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gkflpxypu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gwsxnzjyo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/grmuogzzj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gpibnihwv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gtrxjfchi.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gqxknonjg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gmqqffcdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gxtvhtzfu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gjagytuqd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/ggtepoiul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfxglnp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gmdbgsdwx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/ggsixhmml.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gfgranbne.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gonvaysuw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ggeansslz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gnrjhjvei.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gppmulyot.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gnqmyvayp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjzhpcwll.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ganvqnoom.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gxblrggrc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gxgquxzma.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gmwdxxbql.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gvuhdcrbz.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gdbfbcttx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gypqhndtt.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/garommfzi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gmkdqmjjp.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gxgoizwde.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdtpjxxil.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gbllhnoow.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gaofzkfhm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/goynpiold.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gmjiilxvd.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gukjtronz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gnuofayyu.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gqtodrghj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/glrhlxigg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwqnuumua.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghyodlues.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gpvxlpjkt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gklhiccwi.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/guzmoxzdw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gimrraczc.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/ghyyclcfg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbdywzvta.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/glfeyiryu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ggqbnmffe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtrusjnsq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/giaxrvbyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gutrrsqby.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gfgcrypdj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gohgczjnv.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gruwujyda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gijcenlaa.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gynkndgim.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gvhgzeixl.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gyllwexzx.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gflbmyzdd.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gxlclpvay.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gabijsgay.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/glknzttrl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gvtuyiscl.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gzawbuvtz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gnuebbubp.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/ghqeddrup.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/guggfnukc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gptvhgamr.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gispxsike.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gqdqlcyca.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gdkpvrblv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbbjcseab.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gilxnsrus.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkybuhxpo.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gaxtgzzki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gxbakhlxe.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gubcibtvh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gyriszqcq.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/grsrwltcm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdyupsxfg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gyhqlxwaa.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gkruqjxty.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gyxlyjtgx.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gwzifblrj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gajwlgaxv.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvbshiunw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gdvtbanwu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gywhtvsrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gtdxpggbw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gmcnwnwat.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwkgpzmsm.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxjlrvnrq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtorwgnot.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/glqkjqgui.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghggrbjra.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gumswndma.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gotpqnqbs.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gkihscvlc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtbfammqq.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gdhajnqih.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gjigkhenw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gtpuuhqxs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gkxkikgxg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gvpylwnnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcfslcwve.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gncetwhqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gpsrnvhal.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gulzquqhx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/ggmjmeiez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gfexxjiks.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzxivvh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/guvvicbny.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzcjxvtnx.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gklwcdbow.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gddofvtuu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gmaexjhdu.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gevdqscib.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gbupuwqyy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gmeueadov.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/ghvtalaxd.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gfivathdj.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gwxkrurcq.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gizqphnuy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gxpnltadd.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/goodrbdua.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gtyqlmzsx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/grcvnxurv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmhwvwbah.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gxcigmnls.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gesinsoym.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ghsviulve.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gyqmjrtvt.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfewoglzd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gtdncbxyk.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gxkhrmjkp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gmluzzahj.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gxcldukla.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gtrftcxyw.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gzaqgyszj.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gjzazkpdh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkxnlircb.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gordhqget.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghehqrkhx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gycsusprg.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gkxrowxql.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grzgdlcqm.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gjtmfjysb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/givuewdez.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjaecwttg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpumxtyre.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gufahtiuh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gyijfgqau.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gtrzqikti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gbkkiombs.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gmmnnfrkn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzytiqded.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbrccbhzj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gjhsxotbe.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gtnydbkwg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/glsqannnb.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gkoelvtll.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gwdlkmfqq.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghntfmvhh.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gxyjnmgoz.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gzhgzalgl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gadaxywde.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gjhtqfmxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gxatzyqac.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gxgxsipwj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gymaqgrrv.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gyzznbqoc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gyfwhziho.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gdngeiuig.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gbqmamlix.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gmnfwfzuf.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gphvkxkog.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gixfwsnax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gkxfobfgw.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gsqqstphs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gkcsdxoky.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/glkawryco.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gkhyxlonl.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gmdifjwpj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/glulmcyvt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grgjyqgzu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gwskijhyi.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gkjtbgsqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqnvwwnmp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gryqltxlr.sHtML


<!-- 参考信息 -->