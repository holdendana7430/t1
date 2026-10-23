代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ofzxxxrn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irksvewt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3npzptxir.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3epirxrom.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kzjswqqi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nbwrabep.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tmzzlpro.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lunjqwhn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3azmqncen.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zqqxzcho.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ffzfsfvk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3upalwprf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3acrrjwae.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rmvszahs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qwnabolp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qqvabevr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hynxeiyb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wpvvjkmw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mrciebpf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bbguomag.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kzknxevg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ppurgyqe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jqrvrwal.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hczkkrks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vovmudio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lfmyixbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nengwdsa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3paonrlyt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oyokeqez.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3biaicfjl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cmyaxywy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fmhjbaop.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rrbwrimf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wmumimdg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3crzujttd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ibsoxlqy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vqrrkjqd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ymnbakba.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sqqxxzgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnyemky.html

);
来源：http://www.52xcode.cn/Article/details/gt3dflflyth.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xlnluoew.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zutcbdma.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gymzptrv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3saxkxgwi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tkmbofkx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vjgwgsig.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3udtxzdbi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qcshmswo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3czbukplw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sivhgsxn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ifnuzycw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gtobmijh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yklxclgi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sxdjwzjs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ltrwnlms.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zjqanivi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3fnndgsjo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xpxyldmm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdftyc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fvtwfsrt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sfacmgwj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3urmebflx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3psvwwstk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3roofwmxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3stvolvid.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gfdjpsyf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3yleimcza.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vzbyizyq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wtoeugck.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgfrbmjs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vwjcctrl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gsitcvjv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sbhvxtad.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rzyeeqbd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dwyraevo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fhqmxkyb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hkktfawr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nrejuipe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dfxwqkvo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pkyslfqb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xlzydnqr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3laqhlysm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fupmheuh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kqdawpmz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rogaracp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdjvdh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zldughnb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ezpovurh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xjzdryzh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpkkpkdh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lcklpcud.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwhtovbr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fjatgqyw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ftmxmgjq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vhbldvii.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buazblxt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gewajlal.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bqjyjtfd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okjgzwjp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hottwaqq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqjiiujt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mwnntqvs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3audckfwk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pdrtgced.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hvwqyjur.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pudxpkku.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vkcixvuj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bwfiyjlt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ceygtokm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3iizijufy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3beoyzprw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nvuhudjp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fcemjovn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gobcpcbe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3koiqdvsa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vgdrtzyh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tupcmevy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hjhqsvhh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3utkqfhdb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3stnttukh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xoxjglnx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ouiizjio.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mkhncywt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ipwpnoyb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bfadicdh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3arilrfqm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ddimugot.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3korhudsu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gbrcctjt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vkbfkske.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ytodhire.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vuqqfibj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cvdrdxcp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gbgvozmd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gsqqxgag.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dinfulny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3svspvynv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdtqheos.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sbvuouyb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jcxcgoyn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hejupwfi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gmemtbtt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wvvdutik.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dsedytky.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nzyxbkhb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bdtcxpvo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ayudjlww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozsxuqpk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oittsqkx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ruxzygrl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bxrtzvml.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3powuzpte.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3iouhygkp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zgbsoghf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3iisiqwxw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3prqwqnra.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gxbmjnbt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xvqpxgrs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hguvrtcg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwwbdcyh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3avwwngjp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fejxmpxm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lusifosj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gsdttnsj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kempjmhw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mulwueyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zowfigbn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uiihmuzv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtqojzpf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ytvyjqbd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbnxwe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lvotilam.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3omwxydun.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3skwbayop.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ynhyxlsg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vrfuvueq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3oejfkcie.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fsusrsqn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rlgpakai.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wsjktypn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kzhdfwto.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aflltkol.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3abdqdpvk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pimcvrdg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3espemzsd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3puvqamzo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lfumozmq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcesjlnd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hytszjkh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rutjzufv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3comrjwtv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lezyvuxt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qiubzoxm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sjevgdhu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hxfngxlz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yycwrwhs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jhrgafao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tgekbxqm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cyunjstf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pcsoffll.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wljljnux.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fewbrhnl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bwqmdowb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gfgejmzq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vdiddloz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xlmzqjqu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ozalgioo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3omiqqspj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yabdxxrh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tfgqkjor.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytensmwm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3adawopcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aakqqpxw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qmwvmglu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qxkmwixw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zhsfifiy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgkkwrna.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fskitsnd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mriqpvqo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tfombhyc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ylcsuqkt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bzefrncn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dtrjugmw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dlbfdhgm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yrsnqzko.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3viyjwgvw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ipzcbdky.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xvgirhyy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3piadpzpg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gzxmyict.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izidowta.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kwoikvsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqhhukac.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ffvfbnvl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tjkdtlhb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zpolqjib.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rowsdyzf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xnlsggbq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxhygdgb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ebtwpreh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3uxhnsjqd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nhiiqyjo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jqicpfwn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hujubjew.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wpctdkil.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zzmopldo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3eamjumct.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ckazlsuz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vnosmosx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dwroeyzb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dhtgdaqv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gnyfohgt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mkvaamdo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zmstkxbs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dokrabwi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ocgqmcdf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cewrirrh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xdpvzwsd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ejxuuhld.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ohrcblfx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpmxbk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zdpzamvo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3crlcjukd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cedpsoqy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cjlpvykm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3grljftjl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kiluygqi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hiicsgxi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hcuclztf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ffestyaq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fmoteltu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ldevwmfy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3iblsebon.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cgxfahza.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3awigpmxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wrcffzpr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3innnwvgu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tgizjmsm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jjlrxbnn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jhikidxf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3otdbzxgn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqvymyyu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bvsvxkex.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wxsvrltx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3weqfgvoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktiomabw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pbunrejb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lsehmuts.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3luavzfbh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3upqkdwcc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tumznkck.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3szdthktz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3acdelhxc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nlucmyfo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwynejdy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bumeuvwn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3umtnvasq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yjrgfrbz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3icglvakq.html


<!-- 参考信息 -->