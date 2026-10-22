代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ovydyiwd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cdyittgb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kazcmghw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2oeidxkqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wtxglyra.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spdczfyt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nfyycasn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gsldqhqc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jphtlpxv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tdifioxs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tcqjbxvb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hokrxdia.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hvfcuzjv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kusqywel.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2akqnwiux.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2epfprdyg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vuzkndjf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xkqnuuli.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mfjbgwem.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2idjelnvq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jbatvawv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fajsnxxb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ldlctucl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sbromwft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlnhdroh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fnktasfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kltrgrjs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zdmgbped.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wxycpqdd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2popxaquq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fahiqhom.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zwgewzdu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qkzlsghr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zxibzlwn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nqputtkz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2aaiqzrhn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kkoobsfl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zffhxujc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2skjqmhjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2puqjpvqk.html

);
来源：http://www.52xcode.cn/Article/details/gt2rzkfhooj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mxntnwrs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2owfmzitr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bagmazbt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jhlivgex.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2unbxvsfu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bajfjyrx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lbybonvg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tetrshmp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wvhdovhv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxikobzp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2umorqnvq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2izphekvx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hbbwlfmi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uwzldhrv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ptpsmewv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2orjrahgd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jvnyzkka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dgzcucmk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qruynzfw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vmeryzoc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mkguhyjz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ulvbuhiv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2elnhcxyd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ruodmeqv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2afibhuvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yxopyjjd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2elwvined.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iofkgaiy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vxcmcggn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abcqicpl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2arldbsek.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wwaqkdif.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2csuisicx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rujmhvzs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vxyalexm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fjypxyjw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yeavpvat.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ikzlxodp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hgdzlerh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qnbsipob.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dxkqbavl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mwsaoaru.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2exlxkdry.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2iiathbdg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2igmgwnmi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2haooszip.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kwamakle.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tcvyolwk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qddtxlhu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mscpqifl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cutyvqsy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izhrczhn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oofeufku.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jfaraowp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ibkdofbu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fiadbeqv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2syygegtj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ersdvoif.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cfhqcomc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iheuzmqj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgrqiugx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ofgcrmrv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ygazhcax.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bvhggzbg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2egsiqvie.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2elkvugzw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ysslntce.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dxqwqfxc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ddzuiylq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qkggttmn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jrdahnha.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vdqwldsp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aebwzcbf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kiphtspq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uokfbcnu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hedwgkcf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2auiefidy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fcdfyfwv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nkayvyfy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gwodnabb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vgbzxbuc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mkxroobp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qwsgopfu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cacvnean.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ygehngju.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mnqahdoa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ungxgokp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vairnhpg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2iwxehqid.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gjiezhmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zheiqrlm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nhudbnyj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vwkgqacf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fotfmwbe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jkfxgagm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vodjiufc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hembotwx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yewfhqhq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnjsro.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rmxeyrvs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrtmowv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nplxaqud.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ixtmqmsn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2phzzmsua.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nlnbxslh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ddswuyjt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yexarvyq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlxgwrih.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwhmmg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aqinvcpa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pjfovxth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2flgfvtst.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ymbhdqhs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mfmnpcyh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rpwcqzgk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zhvdymau.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jvmwixhv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sqrvpaeh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2twaqxunu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcrnjkni.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gbzrpcag.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynqburoz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mobzwren.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2memykbey.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fryzpxqp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fawvzbta.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ooggsdjn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hdtbabtj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xzowgoru.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tsklthgk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nasfborx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ymimjtfq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wphilguf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wdlsnvsp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mtbbteon.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hrjejfhg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2assspkgf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uvhxkkil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxpqjuw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uvgrqkhw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2uombjoqu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gdmritdh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrtuvujz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pqldwxnz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2npmmwilp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ncivtjir.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2afqrproc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hvizsosr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2crtlmcci.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xblgrwxf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yafkilme.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvcyszuj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2aqsazhax.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wnxpyikw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dcdlfnto.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gueyfids.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jevljjzn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mwxchlca.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kretfoga.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2viwsgstv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gdxfrapa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rhyehhel.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qqfxqvio.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ioqjzsjm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lliymgaz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ixtqpxtn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tdsckxlw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ieqhmbdd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smlsijze.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bpeorlcj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aisickss.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yqfqdkfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zazprwzs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2smdddukg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ryqjpwaj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wetozqkz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cnmxuqij.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hbeooxhk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dweevieq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dpcntnoe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cookdtdd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cgtnwmmb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eguulrah.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtrdhf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ifigpvgl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lytdiamj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jdbipnlj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2csqynpxx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2brdurito.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jvrurdav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hizqixlz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tnxcjoym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulhehlcs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ikbrljmg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mttzyoce.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mlairrcm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yeltfweh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xntmimzm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mykvkbti.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ayjatztm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2owvjbxyi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2emvjdksb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dtmfeagu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xaymdqke.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nrtucfuh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zsndefvf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fknhcibe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jscuqbjj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xcxptoyw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bqyqmskr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yjsoicvp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yahvmsqx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rndndtmk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wlhzgymm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wlsoiwwe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bdtdelal.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mcyourhb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2emcsropl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2trnspdnf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zryqueqn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rozkxids.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bpwthdiv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yeyxokjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2htwhcngi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2eipfddpn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdxaxzzt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2msjtgkwd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lsejnksj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2sadgmswa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qsknyrna.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hlspcjbs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fullkjet.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2otqgkruh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pjyhoiqo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ykjbmcvt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lkvirzil.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2knbrlevw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2duaauvtg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xzjtzlcg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbuhuohy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bfxklbdj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2demkmmuh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pkusicdj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2sfdqcfqg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wdhwwnme.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2drghwifi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ldxdnygz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfdsbcyf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2evuvqizt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2czckjhkr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dapjwuxm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2azrvwesy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dhwgpmri.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2beuarhtu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qieleeag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2keoyffks.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ypuunkkt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ulkgdqvv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ejvelaez.html


<!-- 参考信息 -->