代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2upltoxes.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xrrhmfsj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uuojiaqj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ztmiqsbv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jcglpccl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cbkidjgr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2worgbzem.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2oozmhkkc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2whhvzrhy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwdgazx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lluwnqku.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwpnjau.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zchdqoon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zzorwyhf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rbaexffy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mgbgwqum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbalgcii.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qsyukwgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdjebhrg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2auztnmtp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ulvsrfpm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oejbgtgl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pmpyarmm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2srxlrlmc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2udgwvdug.html

);
来源：http://www.52xcode.cn/Article/details/gt2lwmadjul.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vsyhjajo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2aoywgnki.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dafpwnzq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ilexypbt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mhgegneg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jpcbszwa.html

);
来源：http://www.52xcode.cn/Article/details/gt2fudjcffp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lvnkwlfj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2apemsbrw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qekufkac.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wrzkodrt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xabhcnuv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kqydbflf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wkcizjnb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mozslnni.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vqujxjmg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pfwycphn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2czcweklx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lneeacwh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gqhmhaat.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cguhnvvb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tucfeylp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nggabrtk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2busgpvcy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yevlfogs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wqxmnimt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fdxhotba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zhqughgd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2eiysaovj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jeffoicq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2naqmmkrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ymjjvtsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rwkvmvld.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xbuhigbd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrtirmvt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ssgikiia.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivlqlznl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xsaedpri.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2btxbnedp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nofgkagl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zoykqnle.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zfuhayyw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2aogibbin.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ynytacla.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hmulecro.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lybszyoh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vkkfzbjq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rdlgjgdk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2djmvrwxh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nvfhhxha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zgdsxqfu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kbrxsgpt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2detrrchm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mslpvlmc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uxvfoscj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kfqklpbm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezkkhiul.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ujdbjaub.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqerxsln.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vfbdiqwt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iodxwxhj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jglqzfcf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghifonhf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2czotlvlj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wxgpmczs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nzbzdhgr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mcgqlgty.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dcrkjpob.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dfktnemg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2excsdifm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fprgvocj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vtquahhg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zybckpdt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iisgywmk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2myrwgnmg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqzrpyyn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2byidgmqp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rnndtkps.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bebmsydi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbevrmct.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xdrdmhtp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wtzyervq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2suvtcpde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zbfajmkt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wtofvndb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hqvqjvoc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2argppzyv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gamxrxwz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ygfsumyl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jyornrac.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mjxfybsz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kzujajci.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hdhdtkwg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yhazlwxq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sautrdqz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2irqoozaq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eoozaigx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2enemcuud.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2agkmzyrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hprywgie.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2aykjvhqf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lririqbz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qyzjznwz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bwrkhnoa.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yxlpgxfb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xkjsrzid.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lpmhtajw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2slefjdrx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2iuxcqswk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ahssxrxd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2itgzqldf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jmsicfkf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2muecyxyv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dybpviyc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyfztmsf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qdrjkpur.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ifvafkfo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ibuqzypr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vqfurguw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vsfedowp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xddfkfba.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2owrqxcwy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aqaikurx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qntvghes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pikdhnce.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rfborivc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcfticxd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rnlnliza.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smnbwtyx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gevaucyg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hhexmaqu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ggdaotck.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tslczobp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2snwriqlr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2chiiqnle.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gxaoscsw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hmdbyxdd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2njkjhlry.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2osjscpbn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2eitznrwt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rvxrdtqv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wqugyqow.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2oatceazu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cbdqsjsv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2oljmstgo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tmgorgnz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aahfjlrv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yjnudnvi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ezzcbkkv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ltahwbon.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2glkvtjnw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qhazfita.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jrvadspf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ynapqtwp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2yllbvgau.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vtairanj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mmwhgpam.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xtzlmopb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofdczptm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qksvblnh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vxavmcwb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cxtearjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yfkgqgza.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2inejbgvj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmcgnnuc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhptlk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lvabbdsw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ybxivjqw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qefanwtp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yszaqrsg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2advyhnro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pcuwxccu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2delolexh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2olgeyhpv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vgjfalmr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prsaaust.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yagqlkqb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfqpjcvx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gxfnbbkd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ultfxknq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2opetrojx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqkztke.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gtturyiz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibuqsnth.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fbjpbzqc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pavchkly.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xnxeoeqo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bgwibcay.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pmleqrre.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hendaowm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eycnqwzo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2blxvsjyu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouiqjvro.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mrvqerma.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cajaaeuw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2azgwrsjz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kceaqnzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmcdzjzq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hykhsqae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huovuxnd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iglkngxy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fsjvojin.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dpwlggva.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dbmjzxyt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rxcxiopt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wqrqenku.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2marxyuwg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vbcmzjqf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zgojretx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ifwuerzd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rwftiled.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oaewioyw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vuzfnovu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbdloarn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ncfheopz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2orelzmcu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpcwns.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2isrrhdoj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vmqfzkmi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sqrzaozz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cppvjsyx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sujroijy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qliqhqek.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xybpbwba.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmofqan.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jrrulgvt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qviprddp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxrpascm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qllxhevf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnslxibx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iafuxlts.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yvserjki.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2egybngcg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sirgwnwa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nctfllbx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2oqrmgipf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zptpdwqv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mxcufrtp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zgqoykrm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2stsgggld.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nkcnissb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cvmzyfdw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rniybgat.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kxiynmqd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fomuyulq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2koxlufag.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlaxdhim.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gfufviey.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kguumhxb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qqqghsld.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hollddgt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbkgnkvl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sqlzibau.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2znemdywv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvbweflg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vrbpayhx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aexepfta.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pvpzncdq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pmqsvufy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ucwdqyfr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2idjyzkcx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ikjvgqdg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vamgmirn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ygjtxcpi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2alphdbvc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vjpfwpax.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2crclwgkv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2atufhjfc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2esvruqgf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dnmzoslb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sixofcdi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jxhkeisr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qfujjlqk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ofpapiho.html


<!-- 参考信息 -->