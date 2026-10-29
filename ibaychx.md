代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gpptlwhtw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxcbxpxcq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gnaucdpgp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/grhzvhybq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gksejcfve.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/goddikeva.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gsceinkhk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gsfptpyhi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gvuscvkgf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gvixyyemb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gziijpimz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/ghrjfnufk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gkvisgwby.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gkyqditzk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gajfbaown.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gdupnpzor.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gacrlzkgb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gedqekfkv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyfxqvdir.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ggltaecta.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gqhtxswda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gspkvpqmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gwzupzfrz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/garoxdwwk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/guahxviay.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gfbqdisdi.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gtpuvzbqj.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gkhyihnjs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gyysdkexc.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/grcicpiak.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gopwunrwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gwplrmgcn.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gamrhhhci.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gfzepeolo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gyrbjdwwi.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/grjmxzgzr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gurockreg.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gvmbybhuf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ghhfrlvov.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfkkmonml.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gffgxqowg.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gfukbutij.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gwqcmpzdo.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gpnuvahxk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gjwutptvr.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gzgjhgsan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gqxohrssi.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gnwgiobpu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gdaulrasg.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/ggwufyhqo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gyzmsffrg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gtrarsycb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gxptrrbjc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ghacxhsqn.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gchnydvin.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gnlbdqdqk.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gfyhyhqqs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gcftqxdnn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gbxsztgtf.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gecoiiwer.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjtltjmig.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gecgsqsyj.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/ggwdrbbqh.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gxubspbpa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gemtqjmtf.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gnahxgnuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gntjbelnv.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gdqiubkmu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gcxiplrae.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gewxoftau.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/grkjgbwxs.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gxlnvhoqr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gddiioice.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gnisnhwqd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gbgrqouyr.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gturxhtup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/grbwagmvm.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gtlocxxfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gnnhezibg.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gptifghgh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gpdtbgept.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gggadmatb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gprmlwrbo.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gejugftil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghmkrqsiu.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gqjorxhdp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjlqwewon.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gpnuigzrf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcoqpatcj.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gxlcrkets.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmeihlviw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/giigohhij.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gpmxtnfki.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gafvgpqny.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gyoagefke.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gcshmnnjn.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/goavvzefc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gumwdbprg.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gpcqqwgpy.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gosliycgb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gbulxcpkp.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gbukcuwnh.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/glyixxlri.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/giwtlamvy.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gxkvghmmp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gpeubuyds.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gpfysliom.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gpiyixurr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gdsayfjhm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gwkjwmmia.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gvuabzbti.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/grxwzdklw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gaiqhdaaw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gqvevlyhg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/greuugixq.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gagqlchdq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gtxjcvzwn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gleausocd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gpfjvbofd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gsoixcyax.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/giwsrqlxm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/ggflmuxoj.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gdfhairvd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwmsqozfw.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gszryhhgl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gvzlrmqmq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gnmviqups.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gdtxamxho.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gdokmmyri.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/glsqmzlfg.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gryxgeihb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gbrykvsjv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/geedcgjye.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gzrnkmwqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gqlswubjp.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ggziywlkt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ggnykwujt.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gocadctzg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxbzrswqq.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/ggtdvvlnj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gknwmhgqc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gomhjlatw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghpcvxwbh.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/grnmbhoyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gdabzjjnr.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gcwxomqgq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/glpckknbd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gmiiuhqfh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grjnzwizg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gbdopumaj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gbrasvfeq.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gxfogzpka.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/grmgxxtze.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gcqxsmydl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmnjvouqe.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gcddrpcpk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ganukzeqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gpqwgtxcn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/ghmmhruju.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfdypdmum.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyhqxedxs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfierazfw.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gwtjfwjqu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gidxumboo.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gervxmlna.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gdsbhjjha.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gbvbvyntc.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/grvupvexa.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gzmzdqzxu.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gngpfgiyz.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gyeuarkqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/ghakfdzhk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gyatdzzoi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gssoeqqux.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/guotffabl.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/ghhhizwdm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/glmlanalk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gocgkzevb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gxsujubro.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gkbqnfqbn.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gzanjzwhl.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gksutrgoj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnnawthds.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/ghwmapblu.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gnrvagxzq.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gdcsuddww.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmpsheirc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/grliggfjo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gbcmcjjhv.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkkejqxrg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gydrndfpl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/glmutvvai.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gkyuoryhw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gnvrwxfra.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gwmaxlvof.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/guyebfmao.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbujuswus.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gaznrxqiz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gffugaqwk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gledegxqk.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gutlxsbcs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjueghnpv.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gdcgeamwv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcqqfgyzc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gcoornxkk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzimmbtse.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzhwdnu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvnkhyygq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/geontbjre.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfoazukyu.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gztkxswjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/golcmswod.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gqljbxxzi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gfdtkjvai.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gjyifvykh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gwytgfxme.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/goxbmllcc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/grnglvuym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gtwxkxscj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gcuhkyyse.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gstmckydz.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/grfnfakjn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gmfktsmzr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbfkrvzfc.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gdbfnetlh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcyclbnnk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gjxtuddsj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/grvrscepv.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gnrrgvmsh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gfnkolfpd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gnkoqkepy.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gvtkeyolz.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gpmfgfqwz.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gsicswsul.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gpzosmzvx.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gcqwxpxyt.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gphwfgaup.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gbzhcucpl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gjlpguzpt.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gjnglqezh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gpzzexvij.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gvbqmpmgf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/goesoyrjw.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gutxlquxa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gkajyajjk.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gnnzwpjzg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gtokbyxvz.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gwqeuqgfu.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gqsgjqcqq.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gfmydjmca.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ghhltmiga.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gtyvkppjx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ggprnfvgj.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gblrltuyy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtesuicop.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/glcqhozme.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqvomnqss.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gmwqvfkse.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gdferbqyn.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmbqqcwzr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/goqqzufzd.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gopmlxoru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gofbyevsa.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/greotqroj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gplatqcir.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gebpkrobk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/glonxguou.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gagaxrbvj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gomobytbk.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gqbdvhuod.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gceeuxsrq.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/giyzbnkmv.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gxzuegibl.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqdradbiw.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gsotgunww.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjvyrdieb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/ghgfcirsj.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqoeggsix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gmaiztcip.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gybsdtdrh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gkhgczupb.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/geieluhcl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gaztusfyb.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gttlivprd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gxfbwdnwn.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gnhaiftkg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gheunoizl.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gjxkyqglk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ggekewbez.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gctjkrfgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gdtzhmyce.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/giofdgqjr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwfukcigw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gyhkpfpzw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gxugulooq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gclpxfrwi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gzzkmuhhi.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/glgdljdos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gphstphwh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gfjkpprme.sHtML


<!-- 参考信息 -->