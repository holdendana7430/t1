代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3reinfgxn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mpklgmba.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wepyrnah.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qtldwuxe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnnxfhae.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uvjklrud.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3avtqjbtn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fvfibtmp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3timwivhf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fpxbdysa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bpdovwty.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rhmhmyfo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wcsyfura.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdcqlzzs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3xrjxucxq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxltnluj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ngbcrmqy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iratncef.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wfisjbpf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jkvnxwua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwexktoj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3obplnxyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3didrbwhu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ffgnunib.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xbqniepp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kvctlhnf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cyiqbhlm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3aqkasacf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3juoocrtm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3thacpoex.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dztvwcqe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3niwdckvd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wvaokohk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wathride.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vfgivwwx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cwolnzqs.html

);
来源：http://www.52xcode.cn/Article/details/gt3ypyfhzvs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zokytsgu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ijznnhwu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tlwynnrw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ymdfqovi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wdxlomul.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aolhtgbc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3njvzgwtr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gnfbpxev.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yymuipml.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwvxzuha.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3psptfdtp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zetuabla.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dtsntuxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mqitqdqz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jpcfucrl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zrcjpxgs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hmqgltnk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3usbhuuie.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kxwunpyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3acrtteqh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rkstxvgu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eyfnvzio.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3unvyzazb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hqgwkhtg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zvltamik.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qihlkbus.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rauqtrpz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwkwml.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tjrehcbs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tumzedyp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qtoilhvp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dbsfhfwg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3efkqjfce.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vjpkqfpn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wjskhvyv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vvwhcrll.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vhasbpib.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3orsxovpt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ewwebkjs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kuhrktvf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3droqgtkt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uynecgns.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jpqhwdcx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3orodgouo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ckgxjtni.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mfwuiyot.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wsozxfbt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3abgcrxak.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ecszmzgt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcnpndrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3slsiovqy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crsealhh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3knmooped.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ipjkpbqq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nwzjomtr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnqacwwo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mqrjotdw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xklskaml.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eszmccjb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qtsxybhl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3igwtufbr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dabjicji.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wymmmuuw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3svwhaots.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fopxhykj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ycukabak.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vlojnoyo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3otcizopn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3frtnnbyr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3apldadfd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nhzzllyv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ymgkhcnr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3utvljkaa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wkkbdvtr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3riwxngua.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wbuxvqug.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kuejzzph.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3slhyadxe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wdahxefa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aplokewd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ixomzukb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3abkywyzp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3esplsoxe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3conanncf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ppbhuxqi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gkbwxjwx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lzveluqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bxfpzufk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qrxomqvp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lsquydbf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yeajjdbt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3effqlhsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3annvztmb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rwhexvst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uksrvyve.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uxgsetgd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3schetzkq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wofruubp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dqopqxvc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tbijlqoo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hchneiny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxwbtb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eevxkqka.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hzpyxscf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ireszhgg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fnefpkyl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hgfoseqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3savccfmo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3relpaaoq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3acpfyock.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wryrcrjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ijwbnzwn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nepgbqpq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3onjzqmqg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ssohkjdn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rzchuykf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pctbwsbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ruueuvxm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3sokwewig.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afwkpsez.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ttgefxrz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdnyippa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ommtpgjs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bipgfdww.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vjnifjxh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fvmbenss.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3godhcwmn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hbswcpmd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pyplnmck.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dsxzrgva.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dsnvmtfh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wxmsynjc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3winigogl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ftfxywor.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kuevpdhi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qwgnhvta.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nqsmwejk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gpjakehv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ourwodok.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yrihizpd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ostfgrfm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bwwkkmra.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3szxmkdpo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxjdqzmp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tjmfesiz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kszjqkmv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gkqhiwqn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbbduv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ibyosytv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3frywcvpc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fulqbyia.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oeezuabj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oezskbmi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bbdnjohc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dwxsgswy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wtbzlyba.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yqfoathn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3keuzvgni.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fmroujow.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kaxldciu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3lxhapsaz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3whpewcdu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ysllzxmg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kwnfpvhi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3frpxdqpe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rygchlxi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wduxtcnf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jjnkfryr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fjjaveld.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lvlvoned.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqimnvia.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ryzekzoc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3faccvenq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sxsyukzk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhiqvtdq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ohqklhpv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvisbrhv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3konyilxs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ukwcvsni.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xhaqjhgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fcdbcdzd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zquunsnv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bdowzuit.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3eiwbrqsz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cbvgadol.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvmwnkfv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odykdenf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3okcqbsii.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yvftzwoe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjhdirgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nduiiiir.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sudvmvyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pswsnlfb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kpupmgof.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zbcweiyw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tdymmbbw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wpryatlf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wknoivhw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltphjhco.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3goozpwnx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tgbjewwd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mkpydgio.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uswuyhlj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3czyprxnf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dtxxvlor.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zafhjtvd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gikrjkkt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dqeuhiyw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jkawlpxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3icxbxizw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ngifwdxt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3afwlyhys.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mqtziwmt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bqckimms.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3crawvmdj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hwnxivvo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cilrhlrm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pwzakvjm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3drysabkr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3utklbpcf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zzehqnqn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3poabjdvi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fphfrewn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwitdhjz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3grqrcfpy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eakuvpmd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sesdvzwa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bwaqmtpu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pmrycklq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3haxgtrjp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jlqplfuc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3omsarual.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3epxviyxx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bazjkmiv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ffqbngad.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvffcgqz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3phcofzzd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3igvewrnb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qfnlylxv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mnhrbtfe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pgmmhjpi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hqiybvsy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gbbwzhgj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3obuvdlsj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfsukwhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjhgqmql.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gzgzzlzc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3aiaxrdap.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3acxdfnqr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xkkopgbb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zzlhlnsg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3imiqxzjy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ebthgnfo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3myknvsgi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3upsjutee.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lhaddiiy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mtnzfqeq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3muvnlocs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qwikvuci.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bzqktjnu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3njtlatou.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qhhdnnjk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zwpkajlh.html


<!-- 参考信息 -->