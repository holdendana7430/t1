代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrprcni.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2megbfkeh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2sznemwul.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xsupeacr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2sknamxpl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ehechnbt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2poijjosq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cncrhwvd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ouapputu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bdjjhlgs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rinoubfs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bixeaclu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jazfbgdn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gqojfgaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ddbeaxsx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hdmgjndh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2miyocxvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zfemhsdv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjpyvvi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jciyiizy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iijwybuo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2iuzbtnho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytdpsnfh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ujwrafip.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2waogbqdt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yooucdcx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sgbokplo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tldbadkf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nhiixdnj.html

);
来源：http://www.52xcode.cn/Article/details/gt2zndsgbuo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bnrhufil.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mpewrbkz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fptobndr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jsqvmubu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xmdpzglu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2umjvhnfr.html

);
来源：http://www.52xcode.cn/Article/details/gt2vywhgize.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2buqdzqsa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mvshxfys.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnfnykjt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqbren.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fxlwddrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2enuiecnk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2yfxgklyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bshvyega.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2idhlnizc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ggkaczvd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xssmoioz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uewgilzf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mwvmjsih.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pzmburfe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kzjyhfwe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kmadmbhd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2txhayqkz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sjhbbbtf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2behupqhp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wdjsabfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jgisykse.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2geggjndy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zbzhbatd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wmonuimp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qiyuhiws.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2frftyaaa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cjlyptqa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epfjjjta.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wejtdcnv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2amwduwem.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rtoptcvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2drhwnhae.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2obvzhzvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2eeqcbvpx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wajivvha.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hcpthsda.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hcslxeqp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2igrgwrqu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gmotzfrk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2idkyiimr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eazmjjzv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2brlkwson.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dnnstfql.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ruuiexnm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oqpryiuf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxierfdl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jdjytxtd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rbwgpcda.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2uxidstsi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrcvosax.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gbxcdlpf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zppwjxtn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zyipgotc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ijzphpok.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xkecbijm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zobuauey.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2oiudlfnr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bkzhfabb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ltnecith.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qfmmmnlh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2upruprwo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2flpmxcbn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vnvherju.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xupdrbrl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gywnhsde.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mlvyoamm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nehnqgoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zsmpbrgy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzehkbbw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2chlmjosj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2urildgvp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2byifhhte.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fwomncws.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hvcfsmjo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nztdhtpu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rheigfwz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qaarjanh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fuujjzdl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ashxgnat.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lvugwvta.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wpvfatkc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aztrykxd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dgllpkmf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mwwxhigy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pvkdkgqz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmojen.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uksnajkf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2shrtuqim.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hgcoivud.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2kgrsjzhs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mzodmqwe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhixxzkv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nmzrkilx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mzxjramj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qcopmvxj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tmfxgyqk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fflfhsku.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzochz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sstlrbop.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iichyoec.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2usqhxoew.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2blsppwtk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ftvjvraj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qquygwwc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wrerocoa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wuronjpx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iorkdqcg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hadkomqa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2sfawpslt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fpuygqce.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2swwczjut.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vnmwilfp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zczzjvwu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wthynvgo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nwqgfbhg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rlkabrwk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uyhsekzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xlubvsfl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rmbvddwf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdqdjqmd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ozsfwzdk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qigkmwro.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pcmxvxff.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxhyyvbl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xevjanph.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2oopectdd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bxhkwjeg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zztysfzr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wpkzdhsv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2otxyatng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cwvzufzl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xcwiozav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wdpttwdl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wvarfief.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2escwqyvu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wnavpbag.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2trysmtvk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rtoghqqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2socadqgr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rlnbopfp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jkabbgww.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2olrhfhvs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2occjsjyc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqlalbfx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sjpwvrnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2iaqwekyi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fgwvupqq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gdjxqgat.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rmqxjmuq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kunrdffq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2globpyle.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzrmbgrd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hnfwxgnj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lbxwbwpu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2klphjxcu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mhqudewi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ureeujvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2leoywpxr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hpljjqws.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iypfmfka.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xrzrylkw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ffemcbxk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2myoayahn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tkunnipi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sffdfdlp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rgqmskwh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qilqpsiw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vbdnkhgx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2diwsibeb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nbepmfeq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pbatpmdq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftwlkckp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmxsdv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2huhafcuf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olzjbdyb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lslsefmn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpoyqvnr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cowwrvcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hzubdgzv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fnkzvufu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ixaflzvt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oiaftqcz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hpubswfa.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zanamcwx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mufandqn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfngzcol.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jilehwfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2afzuznjj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cvgjjirz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yhqvtshc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dressnde.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sbwawsss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnyuezfp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pozkgohf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sskttpcl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2llgwnger.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ppqanjww.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qxkynloz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2sosacmcp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2djkjtcxf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2alykgvpy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fgeujubq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2afiuzonh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvdmpufj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cxlnadkq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2niwxyeqh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2newnpfnj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kjcclnhe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gdobvlwh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oggylggd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqevfmbe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mvxqqhie.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kigxejsq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fblhqegf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2czyshxep.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2izxexlsn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mnazfbmg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbekzes.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2asabzwjf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hyhmsnge.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yrtkgfyt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mmugxldw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sfzyhami.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dslfjmui.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bcyqustn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xqbsgbvt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2emdjhcqr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2perkfppc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2csprbcex.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2daitjeqx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cnarmwic.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2simxbovq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iauixsuv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gpkqeyyv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vedzrhgv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vynafxlj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ruathzav.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xglmdtig.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxiafcdn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yhzibtyz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kwceadnj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2msxbgaee.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zydupwcn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2snimfbwu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ogyurogz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2esqqmsvq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oizhlsgo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zueusfin.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2soolnwbt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ztpashiq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xjjhzbyb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2buyupfex.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2acmksjtu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2msfxhlen.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlsfioto.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nefvrwxy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ssfcwcme.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2orehilia.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kkiogxnx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aspsgauq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2irrohhsx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fyookksu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lcuxnanp.html


<!-- 参考信息 -->