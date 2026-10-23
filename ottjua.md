代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpxvarsq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nfndbmps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tlkunazu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3trovcjcq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fnwgvaov.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mdkuulmv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nuhjkdjq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nmnwewfl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3waywpxbh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdhlomrc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iyadhnkd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jykzjjyq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3aetjmcnh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jdbrusjp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jvjoaxkg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fylamxik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yefvzzye.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mukruvbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kypmlipe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3umudnsmh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3eevrfgbr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uqtcuyps.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3voganfou.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3usnahwcw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bbliofxz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rspzxeiw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3brjmaobf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ejnysivb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hjiryllh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ffdjwvuf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uzihmkiz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3euuhqvod.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fyrpymbi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ujplakxr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lcidtdut.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bdxxdevj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3adfctcsc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ruuytbyz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pkxawzbf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hseytcms.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3eegimsft.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ijkfovja.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dyxunilv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3papatzdk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fdqehrod.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xqncgoyt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3truqrgfq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3edkluudr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gaefgfxp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hazxaxic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3idtwellq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dvoextdx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ykliqhmt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3msilzgsl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eehvtvsn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ndcvjzke.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tphhbkik.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cfwgclmc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wgxftkmg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dszxjkkg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aeelvxsz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zpjcbkpc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqdufhkc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xhepjhnw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kailctmf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cthiimac.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kvquoesr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mkfpjwco.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bklwkeko.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rfxyuquz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oegkfptj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ulomjfnm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qheybhou.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nlrmirfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rkynaiux.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xhhcwbpw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hmlqiryo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zohorvto.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utmqaxqo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3merqxatb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cmhajrug.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wtyhgesu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnnbngdf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3chzzbeyg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mosdgidn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wvdndopr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jvfezgqp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wojirhda.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzazwpzp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rpubjhdf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gbagawbf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qshotbih.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pkhnbfhl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bgzbfsvw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hpujvzzi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bwsiisrs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nfbspkls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3expqzjsk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bzovrych.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vflxgkoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gkavmltg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbfszyyu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3flieualv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3colllizw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pafaetci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qrxhyweo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rnaxrotb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3spkvoauc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3opzqyaqy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oofsflmt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qamhqjup.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fynlkzak.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3emoyurxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lxbfuoka.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rtxsuiue.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bslupjjg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3iwuyoycv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vcrtqqzl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oucmjgob.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qhkizbzd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zyyiskkc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uyouxzkd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bqrttcos.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wnkmsjzd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rwfrlsji.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3krowvwub.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3piuotwyc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3liwvnwac.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pdraqljj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3twozdlkz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3omngkpht.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zrdynbtn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jgzxisyl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfugvqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nsqdgjsc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mnxlvimr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ucazgzro.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fhknwpcv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jueshnqe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dhdxawil.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjwqdwwb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mmyvrljn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jiuawvki.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ikgqgxix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lcplrpmo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pgmgpdur.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zjqjfowd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tushvfma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aolnkbcg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uerepjaw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zjafmbzy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fhffyrft.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lemuwedb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tvwqgufq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wxtwoazk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqczen.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vjipmicp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kyrnnrdq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3twjzqvzs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3embrxzll.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3weazgpxa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eiyfenyj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jbuifoyz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xtqamfam.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sovaliah.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3umnqnstb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vbioxdhd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sartqigw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3osdsjmse.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wjxatcch.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dpafbrsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hiydwzkc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ijgpvcac.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3yedysnky.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ggolfpox.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mmfdwbnn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dxxnrgzl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3anzcxtyb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wcggpgqe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kxblxduv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvqlnxgw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zumtaosf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xkchkrhq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mkaoiiln.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjvihcwg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fijvbquy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mnzksygb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hthxcfct.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3egyliddg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cifcnwiq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3efodvhzo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qeuevtdj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3upzjdcrm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3vvbusgtb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kgbusteu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xzgzimgz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mvvdyrvk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3etowkfdr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aqrgtska.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3upbzghhv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lugfgvgw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmdneepe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pgmxvpeg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hymbpxzx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3puaxjdvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hojfecwh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pjhpkini.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ywppvqlu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uxvzrrqw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgjcpcdo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3foyzvvla.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dcvzngqz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wvcnwscm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hdpopbqj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tdrutbdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ilvnvgbx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zbsxegxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rvgktfir.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwcpnewv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rvsvsrzt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3duaxcjby.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kaienbgi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kzwntyyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edhxrwiu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3amuupjhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chzvnnoz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wedwstww.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3poxxdkgh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jouecwhl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bnkhxiwn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gngdrgxa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3atkcxnpd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gpdzvjan.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jttcfiof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3svmusnwx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ymqmgxkt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3anynpzbk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rrywtccd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjcwzclv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3oatudiwx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eeshzree.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ufntgrac.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zcoszjxy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kvcyiksv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ugnwlbjv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wscyvrqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nzxttchl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lebjwops.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tjlizozn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iitoihrw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aiuoadfu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3arzdrnqr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3krugvzxm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmtogfxs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hurgsdkh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmupdgzm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3brwyeksm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3elscspyd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sjnzwyrn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3igeaxuqm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dghenewd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3moiewqvi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3acygoloa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yfahxcjr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pevsnrer.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mizpfqju.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vgmigmnb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fcffxstk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wqnyjikk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rqnorucs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3poxqwzvr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hadxrkpk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dckjrbux.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3byhykkrb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwxewozo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sxzgpqlv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3altdpwyy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uectjhzl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqhynqnz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pplvflul.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zvzokndd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ilsoqqpm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ynkywdlw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tegiaeyh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3umsionjl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jlnnamcy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rdhgtibo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3olcqzfld.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qitzdxic.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bpmpsfhq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mqvhsndd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ysnaruvz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sivdhaqf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3sfjefkqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bhgfsfbc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bcdowcfg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3aazyatwp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lmtwjqkv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jwzjxuwr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wtjqbydz.html


<!-- 参考信息 -->