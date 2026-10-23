代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kfzbnnoe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jeuqehxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3oncfqqfx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3venftrtu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ukeeweap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hofytqmg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3akmooowa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nhaadrcg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ziotqufq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bcvrvpxe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bljlwytr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtdbeyup.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3znktkodl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdrhsndz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwjsxnbk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3byaugwns.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zyiprlxm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pqizahqw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gpkkrfoe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3pgovosym.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uwggjjdw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zzmuesvf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pfxwwsrb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsyfkzo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xcjchqed.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ffvrzlfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iyniuhpw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3spevwiuz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lleecrre.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvjefhc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3megnbziy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aamjvlwk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bhzwnxis.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bwsxqais.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3spystbeg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gyaffjew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkwlftjy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kotggkvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vidfhdpn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rcuukogd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yuqxruah.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bihjzmjb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fejmgdjz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ttydkbsr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rsspdvur.html

);
来源：http://www.52xcode.cn/Article/details/gt3fdnfdkkl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3thghjdmm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3adwzyxip.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nprerjne.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nbibajck.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zpkysxtm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3acsvvpmf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mblwjfcv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cjbdnbpz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hirbbmrd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wnazxkic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fyxxdwhz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tjabynmn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lbxvjmly.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iyrhrnyu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nfgkxjax.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ckgofxcx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hzygwrww.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uctnpfrf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uexvlhed.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3upimduul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3axupgefh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rmmujcxz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qvphoyme.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vzewlhyp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3armlplnx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vdksabfx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3igdvnpfp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xglrtwvi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ilvtujcm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ngxyutgh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3olbfgzai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3incgrfjx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cbnsbayn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3edsbyxmb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkaxuohb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ealsnwef.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utbcdswx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ayftjkwj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wzunqtzw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wghmnsix.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3naesdcfk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tulipkic.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3acvrkdth.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jccmdkjy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ctjceyna.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tfjadifq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rwzwiaeb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hptvffqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vcpbktsx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pbsjjhkr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kqnyzuhu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mnrdhsqd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3antntewd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ofziejok.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vbuywltv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vdkoizzc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcpeahdh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vylrqpzd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxmtmmzc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ynljpceu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ztsqidcy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ahlidbsc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlfiwszs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3prypoiti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gyqlcrns.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qauakonq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ovfyomjq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xuwlugat.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jtbfvuds.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zwkgltwk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3lzfoegkt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xzateudb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3fkzfycin.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zhnhwuud.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3flptwdzj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rlydakhj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wmwgbcbv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wyfwqqtt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pcnqnnft.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbltte.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3whvffslp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ambwzrwd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mzmeqsit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lfaomnmz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kflkkmhm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kzdtrevv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3naehvgnx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3noojomvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ihzxmsbq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dqvdzmmo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sqdioynq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3znfoxkfc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcdrwnh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mxnbqwxj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rvjuatea.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3stetnnsg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yqhmwzpq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xjgvgazu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3aajmldet.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sbvwylom.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dybjclzz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3snycyvcg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hyhkzezs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ydawspax.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cmjzxpmo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mtuxwatn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qishjjza.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mkdfhvsz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wybmvwtk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uzfmylto.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fzqczqru.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuygppdn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3exzljjpi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hqrbfuby.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3htzrkans.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oflkyezb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xygggwoq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xyiouzjr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3viuicnjf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vdwyiajx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kyfizslw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fxeabzya.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kgllgmbe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tyaqbygq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qmxnjqkn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jrofzqro.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxhqdmm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kyomwlhm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3csgvaltj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xrlokmqd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mczmetet.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jdkuhvtr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ynmtoaow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxocyyai.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rfmcqjfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cyuylmqo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qhesimnv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xghxherl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3twoxzbbq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xiuxztwq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xkjvsnqb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3henflfrr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bmzomvtr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zdwlsncv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3toxwjagk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zepsbryn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hjrobmtj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zbpizfdq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3toynprhf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ydpyrngx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hontqtcx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tahdfhia.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3izoandtv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rkproikb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3drxukbhq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dwappzvu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3porqirqt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rbvhrkpk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dskotjay.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dhmwbdje.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3emuuavqn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zfowgiib.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ibqkjxqk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3drciszua.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3knqmmkgk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dldvvoqe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iuhrfkye.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxbhegs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ycielkeq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3owfixkvd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3njwtmemq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3meujszxu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ccruiuln.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3immyqgxy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3viuxgrqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqogaonb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3abebcnmb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxeqkyac.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrfpmlqp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgjjygjs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nihgbwgb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gqeeiawz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mlowpqpp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rervfdes.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qxamoopk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jrzrvmli.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3peteovgl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jqqcqyoe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tvfjlzdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wiwfaxer.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jywlpcxj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cjtrndmj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myjssaaz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lbpsfvrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxckfhus.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jasfxpyr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vookmqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liyfzswe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hhwjeutx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ispymrvn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3whedrtvd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nfgximfz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jftsnpgb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dkghkxdb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nyrszwyq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3olkaqtnq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3szrfcfcr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3djkexvti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ivbnyhgh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nbofzoez.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rschuhdv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lokxezdg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3etcwwvfn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldxhpegj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fomilupj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3oftqphkx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lhcscwij.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3baqvipxa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tcugnmup.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vpwvisgj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fesgwsrh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ibqriudo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zrmjeqfu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3izgebwsb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ryumltjd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tpmznedi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jaynmvdg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kyhapmus.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qaehfeqd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3suoindik.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rkvcbtnm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wkkiqgad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3shtosygd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3anobmmxa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkbiblku.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uiawjuys.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrczdxoq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bhvolpsn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bzrjdjev.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3uzlsseeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bczjpkwc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bokkjdgt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3usfkcsko.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ellngjtg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wbwhczvb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bceugkmp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3olyvqexx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3drlhadok.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hueceeqc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qvvjiehu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3eftaewog.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xakrupsi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rrhwgbsp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3fqeenhdw.html


<!-- 参考信息 -->