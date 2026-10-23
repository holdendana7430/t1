代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyjlzau.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bzhmmvxv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kdrijypi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nikfdsyt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mhybgrkh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmndtd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iwqeodti.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyxkuvel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oajexyus.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nobfnver.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbgdawxz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ikunzyew.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qgsyjpsk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ubxvjrmm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3otxsiwik.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3iybrxrzl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dhnttbya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sicsjnlq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tznoxito.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3anwrhjhy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rtscjscq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hsspfpsy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3icwbycmu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tjthppyh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xipmnose.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtxkslpt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cutntoxv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjuiozf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bpwvwiux.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rzgknttz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dvrswaax.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yecspydm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jroadkvi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qlmpywyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quvbeawq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fgykyxzp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zadesdbr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fwdwpbqs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3acjebotj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zuntnbfj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fsawqztt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hvzbbzai.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3euqhwcsz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3evrrrofr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ljhglzcl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3awnbzbfc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dvehlyyk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zvpwytld.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xujjcngd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mtnpqcvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3skhgwqby.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqokqhkb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3arfqflar.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eesixipb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3godetnkk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ilhffjna.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3naicceog.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cjzdwtfw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wwthubrn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3arqljdei.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fjydazhr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3intailwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bqtyzavg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3obgyzoho.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xbqytbtr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3idqljnwt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nvkhclaw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ifnoeyxi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rypbtqnb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3msyfxkls.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qdrdrtrl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kcmzjujj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3emtyygvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3muwndtzy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qfosmbeb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pfbznlvn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwmdkugo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gchfhfjh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nqgmxujt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3helmzrxg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ftcjnvcp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3eiuutxfo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qlwtswgd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lqiggsul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3okxuzuet.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ecvehapk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3futllddg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uvmxyrtb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nhmivfwk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ctnieegt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3oeokpmlu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ijuqmjqm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kajsvszh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3frhqrblq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ughfgglo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kxtwpoaf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zujsbkwl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3leegabgj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xlnrdpfq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kgkohtbt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xnwoohvz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mfivxyfq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zztxkbpj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ntgqplbc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhwgsnhq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3igjzpome.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zpgyctjf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xhemsryo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbqiqc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkrtycqi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3baqwgckf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tdqdldda.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ksrrklim.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xtjabdcf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tdxxqdtw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sgjbhybl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dqeioczc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fivpgyeh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jmjkpoqh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bvxyosxm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3unyilbkj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3acxganic.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3sfmqkkia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3klemytir.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ohwudfqf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vfpxzusa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lemxnquo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qeqdlvii.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3crinaxkv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ylablkpk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3emkqnmgf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3maehzbbk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jydzpksz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fwjytjkf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wscfwalq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ohkddcny.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ktqvjmyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hbjouojh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3aihjklyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gbotfzbv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rupnkbcs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zhfarmip.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rniejajv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ybkrmzjz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nvyyaniw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3azeieppy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3njykraud.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bxvnesqn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qszjmchl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wucpsmpj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3okeifdue.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3azxdomlu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nbmdgjct.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qluthkka.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xilspabi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vyqmmkxr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fxqxowva.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vdgzklzy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ehwhcyhh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lsatorvw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ztjqxqgl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ydzsecjt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wznrtqah.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pcuuojbl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3grgeqbfc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3brwcllek.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nhggcnof.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3akeussqv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwvyypvr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yvyvbnyz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pkfspdly.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lvwkqgsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dgoavaeh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3innlftij.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bemngkpf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qogqpjau.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3aytzvynm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3azdpjjqd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jdescqqs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rtltcuwh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3htkorzlw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nrcugmdj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3asbsretm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kzmlxcpp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3phxznbsk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zzdnkknf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dnrxlpoo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xkdmxzoj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mdpyhqvc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qlfjugel.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cgrduvbm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jbfezknu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dwnblwlt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qrrwijbs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3aeqsualu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3waoxluqt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cpikwtnx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xrwsxhvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fobachlm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dqxdfsfo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljfcqlgc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fokdxeug.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bfupauyj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gyhsndou.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fiqmrkmk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hfbtcfvg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rbkwwdri.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fdkekrrw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3owjfruoy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xeygdkaq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jovtdjud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hghjnpid.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3upznlrwi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qwhzwctu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lilqpobp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3urgbnpte.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3otsosfjz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcvqdpbt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvmzdfoc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cagojomm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gnafxkqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzebpl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ohqyjlgb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwrcnuny.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uzzofczx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3euuwkola.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3eudheyoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3npcvqfhy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gbtoquyt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uczotkot.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3myoytebz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tdcfieyf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bemkeqgf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tdqkisjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wcxaebfn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nofctxdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3meehugdv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pbeelmdj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3msfarrju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zipckvow.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hivuzcbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbgmcfgc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ucyyucfo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pbjlwvhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pdndkgbq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3phofiwvt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mjpnovml.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zjyqfitp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3giudwsmn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wzwccevk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cpjfbwuo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ygxdcboe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mgwahibp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vzawhiwd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bcneavkq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxwurrmv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oqhsjnlj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dweeiyhi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3egicxpvs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3efsafbsp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cymvgebm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oeccjaas.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bdcbdzny.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lwapruet.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wmbicamy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrlmhhst.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lhfjopav.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3otakfggp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ayfncbjb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sweyrjdq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tbsjprfq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kgpkuttd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qxfozwlu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qzvilstq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcyfnkwl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndptimla.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wedtaezx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nmwphuno.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3azclkvjl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zamjdomf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wjackjfc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nofhzjwn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3uebviapk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3agmverzj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubugocwg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hgejsjcy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gcxoibaq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtuwhchg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xixbqnud.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ijjgajpd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddnrbnwl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hgmttqfu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ovcplgzh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cyypghqe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hotuxone.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jhqhrpwm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rbjsinka.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gijogvqj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xjxnuddg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3twxsegvl.html


<!-- 参考信息 -->