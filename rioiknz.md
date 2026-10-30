代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcnktydi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzcnqqpcs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/goppuwhaa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfaoiexp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gzlsoehhz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gaichbzhx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbkfhmzt.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpzdjctm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/gybtezwfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnyfdym.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gczqjktep.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtzjneo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtpdesen.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvdgyobn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gitonqilf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gaumfyqet.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gokgafgwa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gghveqtwp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxpgovkv.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbadodznr.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gzadchugq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeydlmty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyusggif.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gbzhmihjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gswcsjzwt.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/ggtzxdwwi.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/grtrfwrzd.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/grrtkewib.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gmvpntdcc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyffalvd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjzpmvmi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gjllbxyiv.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxfsymot.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxkxjufz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzywbwyjs.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhfdrmdt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvqpqmsn.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/glwbujmgr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcljmowq.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gnpiwqsir.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gcqaduhzc.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjitujcrg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggmkcqukf.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmikttdnn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyicbkelo.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdxoprz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdipaggvj.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmnayycw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gqizgnsax.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gxyfcqlvt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbzfbcfwl.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/ghujvytmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggiobxeo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuhhlofr.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gryylphps.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwlaiwx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/glkqysclw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gnquaqcze.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gsobitxzl.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gqzpodnsj.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfxrrmdb.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbsdrmpa.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpzwwivc.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyrmxeeo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geqdzvnxs.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gbrpmjszi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/genypjsnz.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gqkmwmpcx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynzeimji.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjibrdebp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geavcuwmk.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlzqtdib.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsshtmcjx.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gufcjquwa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkteuosgu.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gndvouwqc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmhybnl.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldtwdrq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxglmvcg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gznqxtpul.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gcqhnypzu.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfydlswms.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gskhbpjvv.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gdrcbgufg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptrivrim.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjoesflg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbzsddg.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlbnomtr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdotjkgmv.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gilddizfr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gdbhenqop.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxngaeeyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvuocdmwg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfahgjvxd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gqlcpzbjg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gdysccugn.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gdgdolqlp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gapasyxme.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gfwktrghi.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzccydtj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gtgkpjxwg.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/givtxcmus.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/ggoxstimk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwpufysh.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtvfdgit.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrgqqejk.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gptaxbdmu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgvbbmz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoxzfys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoyzvefb.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gshbwyajr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeylkqbu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsuhxrwmz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gcsmdhmqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmzvkirz.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnhiaabp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gqhssvugq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/ghaxolcwm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkazweio.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ghchktmsp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzhwyuco.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjerhnie.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyktbnbf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwpmvqmg.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmowtyv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytuzqmus.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnliwdky.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqozdzbq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gowasxvev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwtrwhh.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdglyddhr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfyrsopv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsalialn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjjzhse.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwefctqb.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gmuwslhje.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxafmcr.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghafpymah.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gzxjvgiov.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqepzbiaq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gliokvwqj.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqiuzyve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbinokdak.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ghysdoelx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpfawoley.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gljoxgcjp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxtthfgs.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gymopnzwx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gqkmvmdru.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gswrassbo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqrdmzsi.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaqnapih.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxuvgnjd.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gucwegltm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgtgobl.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gylrsfinl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grrldxlho.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbytlrbgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhuiuofl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwwaicjb.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gpwezdxpc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrxharvj.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqmqflr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gfaebjyiz.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gskvrhgbq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gyiivmhyy.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoieddin.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwcvbeopj.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnguqnbb.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/giwwjuhgc.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxoanhlmi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gfsiotpfq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdcaomfu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gagrasonr.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzbbxcve.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gytvggarp.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/guukhjzsc.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/grnatjfxq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfqwkgpk.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxzdbebx.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzxkgpeb.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqwrzmd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwgmrkkc.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gikvdvdpw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggresgwhc.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gktucpuim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayswwsfl.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgbfrmhy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/grjrsszca.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggtyodafr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppzamfys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gauytliwg.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbicrtq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwsiejpo.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gbrzqrfru.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdykhnqd.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsssbnpsy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmjrizbp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpknviqjq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gaxnkmcvv.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrlzxvrr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtnxfmds.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexxdzxdi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzkgiic.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmgtnxqj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjzxpbfm.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdjpoctfz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflvclffb.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxxsibt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geiumyent.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvkzsuy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlpxlrvp.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/geerfohyc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gwqmswaqf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkcmzeodo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/guaqslpxq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpejozq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gabfuafcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjupiqycr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghialbrxv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gkdbzbqth.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyieggpfq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaqrjtha.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbrplxpq.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghwkaaojz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvizgtn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gulztsxfy.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gwktrcmdi.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gyajbyktl.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/goufhffxf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/giarhpnsl.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gztnbzqmu.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnoumieh.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxjnuwze.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gusatsleo.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/giuumjsnq.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnbxyox.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysiwmaeq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvikuzvit.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkxahdul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgltmong.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhcbhhzz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfwehnli.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzpgscgfz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqdygtj.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpjjhhme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxovwvcjn.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnolxhzx.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gfbogmqdt.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gokcszlpz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gofsubvhf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfresjnjc.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkvzkimr.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcuuezmc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyihkubtm.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/garkgduyg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/giwptkgze.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdipomfu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcqgjjif.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgebfuv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gndymtmrb.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/giwuwwnfm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaoguksj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/guphgpjnv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gizytuged.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgheijuq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqdfayxgw.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/grzwczelb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggncnowmr.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gikswokbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbvjphsx.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsecfgtrt.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyccvvgze.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbxkwgbh.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glbdmccny.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/guhocyerq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggmxsqrwo.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gresrmqzj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gopqqpsfl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/grllddbpl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdexafvi.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehgbxgx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuqmlvog.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/glmgedukr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfqotjcl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluwzsgwf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvkqosxjz.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzrszjxhw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpntdhb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwwtvgqz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbuzwyst.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giadxjtbj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqhztiir.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/goakvscap.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjilbzxe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gohuwniws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkycsujpu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gixigwmmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjsikqlu.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gdssgmsbj.sHtML


<!-- 参考信息 -->