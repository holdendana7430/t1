代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mvaavtih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wueuxkkm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dklzwtxu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ripcvhpw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jbhzzzfx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kouqeawl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lqeqjbta.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fzqrfyjq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bfxrpjbd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pyybvdoa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fsyorsqe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hwgqypdg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qkzvsnqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ycqpvgkj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dtpefexh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fgaynrod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuhaztwr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yypgdbvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raosjukf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tbrdscnz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gkqumlen.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qhuupkdy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hayerrok.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kuisyrgs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3snndvcoy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xivejbvg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3yascverf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3arcpecsr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gnllodvk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qpogeswg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cliubkrv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rujmbigh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xkevziej.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3isylvnjc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ocxvvhzh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mviadjpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dgzjqgce.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vnlgalgp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ydaovsgb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yhcwlonv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pehgrmlx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3auktqnsv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbkskjxs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jmmeeguj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bltadmna.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3elsdlzyk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mcyaulzj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3fclcynvd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gippqgok.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zgeeadmb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3whoekgfz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zckygrmi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mlmebilo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jchteefs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ixxwlhja.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jnxnzkdw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qhgvuark.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mexnohud.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3arinotmh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cjqspbtq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acpgsmpy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dlryvxnp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdoaqykg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3merhuwji.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ievumdas.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ygjhejno.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wtdyxbyc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cwbwawjg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cautxgcg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ucvpvlta.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3baiycoyk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3semvjiml.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zljsnsny.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jxcwmecu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ztxcpjst.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wfzlrfqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3oimxnytk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ubmmkvps.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cccrtdpr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cemkynjz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bwuyvaar.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tpwdaghr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iasxblts.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mnjjspka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqvelaze.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gadbkmow.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dczxzuyz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mapsdwzw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npvuzxix.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wrunoted.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bjraaawl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yasjpnua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pqpzommv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3urrespdb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3drqtopxm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3stepdeny.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xdjpoovj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qzpqlvlt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3chtrygqo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jdbvxzyb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tpnsuueo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3etnntjzf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ftoxwgro.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dmhqqcrs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hskokvye.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bkzbsakc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jiruaotb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aaexgupn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xaxbsucs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ppqycixj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3itxvoamn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3znohccnq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mzpidurl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3iobfthgb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uzbkkujf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rxoadftw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fohwremq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pseaslam.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fpcylyfl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ochypeth.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxjult.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hxishimr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3pjpsgqjd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fedpmqpc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpxntncm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ryclubiu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nglcgbmv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hkdppvjs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nxytnfto.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nqtqxacc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyvrxoyz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3awuvkpmc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3conevyap.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tvwnytmr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dzloypky.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lmyqieja.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qvferwpt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gbzdsvmg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mpipnzdg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3trcijtna.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihgotmor.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rbqtvpws.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pthervdf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zjjbpfdz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hohisklq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3filsjczd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hkuxvomq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hvmmdmza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3evchsmeh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nfzjeyee.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hyttfboh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wiiydtwo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hccddmas.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bwrqzgqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xeovovaf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hjukwqbe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhwnsttn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xrwhjowx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3pddmewxv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtyhvzrn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3awulgidz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bprccpxv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hsaxmshv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lidnwqrh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kmouuonl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pimzsyqb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hmeeswph.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bfwkslbb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mmmcpqch.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hcgmxign.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3evvfmtmf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pbuqqhoi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ibjclqsv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wnzfsald.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oozqrpgl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxoiptlh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kiqccbos.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3awiroali.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nacyrmrs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3snwzziyg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwlrwak.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hjbkdxvn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3chnyayah.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ncjcjyra.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vljqiqgn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3orvlevnp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3avbkkjdd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3srxpxnea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fvrtkvrs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3psemxnmc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xyiicyul.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dbqsshmu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ygxfkfoy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dgzdhvmq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zjutoqqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3uzgnehhw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ptnjivnh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3oieshsgv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hawyndek.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3henzrzep.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sioezlvc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttaoinzm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yxpiuxeb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dydpvpcq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3fssjyvfq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3enkbbkmz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ksgchfwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbalorax.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pyabfbkk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fduympev.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gfovkgpq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nydltjpd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ojowmdxg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3klfzlfml.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3viidtqon.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kydrvjhw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3crmfqosw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tfikusta.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkhyqewr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qmzpirnp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zeswzxyg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gyvlqjsg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ynzitzkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndriwxzx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tegalwnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhwyfswf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hgnvazaa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ggshpdon.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3siohxcsi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3aellcobr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gjscrwqh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3aoffhnqh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xrbkwzso.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vpxmsxfe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dtzojulf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ewygfcmt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmavbuop.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dadgryuk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vqnmhbty.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mipycfqj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvdqkenb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ofttjoza.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nuzavuau.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfpctonb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3haodgfea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3osxsacvf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzmftq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gmeuvjan.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jfihwmhv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ijpdjdmt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jrmggyxr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3prqjrhhe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kzcjzcwb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nojxoejd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aufcohcy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mhqhtgmz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xarffmtm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3irmgobkv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3megedkdp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysibepyj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3syiurmjd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tvdzzlla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cxaqpfpp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gktkroth.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vhmxukkd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxswzr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jcneoahd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ikthedli.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tillwmbg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uvqamona.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ccmjyhqz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipjikgbx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lioibgnk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3opcksigf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ktlzamgb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fazlxtwh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fdgskehf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndahfmgr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3upmfrjtk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ddfadins.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnawezcy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tcglsxro.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pabwnlfn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3umcymbyg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3isppvzll.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xlxhyykb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dpkspqxj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kouyinqk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yfipujyq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oszxrfir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nvlmajvg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxsheppe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpovofi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dejahxxa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zuwglkar.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kuhbdstz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gtdnwnap.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3aqexorhy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nsklupua.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxeihy.html


<!-- 参考信息 -->