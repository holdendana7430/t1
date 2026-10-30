代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gjuceoxxs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gaffklfij.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gwmfgrakw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gvxrogpft.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gtlpbnlsb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gtthtpvyz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gdqxxdrao.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gvonfxhye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzknnytjs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/grqfrpaxw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gwzkjyhvv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqhbmzfxz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gbgztzidp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gujenppqr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gfijryzuh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gpzegydsi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpvhmnjmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gffatjhoe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzlqnvcqp.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gppzrsrph.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gevcqdkzs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gavatchdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjndsrfpi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gxdnwgmvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gtfbsdlsk.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gmtmqqfoq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gnavxckar.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gjeymqnjf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/getilolea.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gufhbyvaj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gjahohvlw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/grztppkwv.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmobfixbv.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gvgzntlhc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gibpmyeuw.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gmssukcki.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gujwtkwep.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gcuwiqwcu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gcngwxqap.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gkbtmhohs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gprzbshwb.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gkjuzmhch.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gotyjbeuq.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gexkzvjks.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gpuyoqukk.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gdnijrzxu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsjtyyqtc.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gmginlbrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gscfbzmux.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvkbjxfvf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gpfabfrwt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gbpdbzhmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/ghrbfdvbw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ghfvukgxh.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gmsftrntf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gcuxdcyif.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gqceaethf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gqvpmbjjj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/giudzoqau.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gzjdwdgcl.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grtosotzn.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/guzidgmfe.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gbcftdcsi.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gbcqgxwes.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gaiqzarhn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/glvbzvgdb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/githtoqge.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/ggcdapqdk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gyeofjbyx.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gfxxlxaps.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gjerhmuks.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gnmjlstfo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gnitzmzdu.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gdepisbis.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gicyislat.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gukgxcgrx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/ggewivvhu.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqzxhdtte.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gazsxkbvj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ghvpoclrk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/goktqhcue.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gujvzgwxf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grzjmgobw.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gcnrfuzzw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggcqasplx.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gslfhbhml.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbxtfwkro.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gknoifmcz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsnnpbhdl.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gmfhykcfs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdmkyrukd.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gkzklvixr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gkqjaonvo.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/guygkrdlh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/giamcpavo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gunyiqhdp.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gbmjldotq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gxatqoxpt.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gmoybyiyf.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gqvnonybs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gwgutppme.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gbipypyjh.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gvropobun.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/glcfwbgfg.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gtgugimue.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gjiebeqvo.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gigwhgkhr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gnyuqkqkh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gbowxbugf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gvjdlgfkk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gqozxothe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gvmabcllq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gjiiztprc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gjvldzndr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/ggjgnqulq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/ghzvfdjad.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gwhqycdjs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/getkyolxz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gkvtojcme.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gskcgcdoj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gqtfycgkr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gekunwvbb.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gwwwpwmso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzljfjfrr.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gjbspfptd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gvrodzafq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gdpejzfcg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gxjwgalss.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gaingvkuc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gydbvleox.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gozeawcik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gbwqupwwf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gqbxrdakx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/ggltfxind.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gvkwfhqyj.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gmeivbrxw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ggiqkrnuh.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gmdehfoic.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdtwpyhnw.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gsdpnxeiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gdinjpbkl.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gzlzjaxwx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/givzpmrro.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gcsbiedej.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gqcchizdh.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gkrywtrtd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gwsgvovja.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gznaenwit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gcgbaried.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/getregjss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmzwcpnit.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gibjsahtc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmnktsyyv.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gcwcuogiu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gelrxiezk.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gckknhfmj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghsxlhilo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gapbdbyos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gsvahjciz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gztekyire.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gpqfuwbms.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gerczkrgj.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gedtexrwt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkwgoygys.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gmpkwfehv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gvazazqxk.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gullilqzv.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/ghicysycg.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gnkaxhdjw.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gyepghlwo.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gfqvwmail.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvicwwnl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/goeccsyps.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gfzqpaevc.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gcaeijnkf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gggjmfpox.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gfmtdapoa.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/galrdlyuo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gossqarne.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gimrurqay.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gppfgyvnx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gawwiugud.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/ghvuxgehy.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gmryswbxx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdtfolylr.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gtypsjuwo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gddslcvja.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gyyjxfubu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gudibzjns.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjeygbcqk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guzncvepb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gzxetzvev.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gkjsgtxxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gmqclporq.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gsonosduy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gacumujtm.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gmzblvgqx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqaeshymm.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gutmhdbjs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gjhvgphhu.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/ghtcaqwyl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkhtteftb.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gatknedfj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gznvcdlkx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gagwzhenl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghhoebapr.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gagzblvuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gewqzciuh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gqfzzopzd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggjdhlzme.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gafnehhdd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gqzmzcafp.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gkrtnofjy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gvkavjsme.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gfgikrawx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gscqxgeek.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gjlsogwci.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gdqoxgdpu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geqxisnng.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdisipwur.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/guhnsqayo.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/glzpvmejv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gxeibjkjo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbotcfcuf.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbydlxsvb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glxkvctgz.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gtxcldycl.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gtsdoefof.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gumyhuxga.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gwlwphrfv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gmyyocpot.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gxclzacpb.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gjpjcmimd.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gxmwmtkcn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gyahboibb.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gldjmnypm.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gpxcvmlva.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gxbqxrauc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gqtlkapue.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gpoyyikdg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gzfejjfyn.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gneotclrt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfapldlsl.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfuirxvae.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/goeoaxwxb.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gsyeeocad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/glrlepnwn.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gnqrjpzpx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/grvzwxrou.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gjbzxzynw.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbkcxcjdo.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/ggdxgpzhu.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gebvebjml.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtouklxni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gtbiguhtk.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsxybbbpn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxjmwguvk.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gsoefdmxv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnirmkctc.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcisrzqvb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/giokewzbs.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gqivccmst.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gopghcqsa.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gfbplqaov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/ghpzoiabp.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gesaqqyhw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/glhsexsnn.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/goszqykmt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwxtntwpb.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gjaiskvbm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/grksottad.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghcarzfvl.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gjrdblmoz.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdblqwwgh.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ghscurpvo.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gmlanytnd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gzuvmzfmf.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyedtsbjk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/geuqvnixi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gkmcurbva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gyghpjjod.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gdwqlvoxt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gvbjeglok.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/ghjipruzx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gmiwuimsy.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gwlzmbduw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gdbchojzg.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gfqgsrdah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gpnkqfnoi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gooamjawf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gkfcdvvao.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/ganrsmjgs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gjzerfroz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gfrxlegra.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwdcxkwi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gnfwzbqys.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/glxcpdlqd.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gbkaqejci.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gxnkcwbdp.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gvmjwywrg.sHtML


<!-- 参考信息 -->