代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mogffcel.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fvrvlzkv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ioybilff.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mdtagkuh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gihisaqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zuobxpcp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dwubivtz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbsjsbij.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qvsrgvqi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcjexbxo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2masugjkz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aboypots.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dsgufjgk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eruicrlz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qtqmntll.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ossnmmxy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmborabf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yrtayclk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tbzgswcw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dfpmoehv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2sfxtjope.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2peorzhgn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ozuwjvwc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wvusuggh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yfclhipn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dguuhigr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hyqcfzno.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2byzxngkm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fftgxtke.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bmeetaca.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ezltgevh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ibbfqswr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uluazfdg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rcobjbqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmalmzhx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uhddmmko.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2arfoeiqx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tctbvjqt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jrgxmias.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qsfprtuu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uoszxtge.html

);
来源：http://www.52xcode.cn/Article/details/gt2resnjmey.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qpmybgtw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hixhfiou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mmxxtscm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ppodrtin.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ymwadtna.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xlmnstve.html

);
来源：http://www.52xcode.cn/Article/details/gt2ntymqjjm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fhpgbcih.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jwgfiunu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cnbtilps.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wxbfduks.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2apjsacym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohmovoaz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lsnmaiil.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oralbpay.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wiiehbnw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hfanczrj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hnstaqis.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2brdoahox.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nmwxvful.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2quvhvpsb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hpdkijhy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ojcvtabk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mpzircph.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mkzgczmc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vtibjtry.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bzoilwdr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vhiirncd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rhiajppw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qtmanfkm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hcxlxepg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2czktgeyx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lddtgqpp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ibvcvyjm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqhtoar.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yhzylldl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iuvtldkz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kqjrogse.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kcndqkns.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dhqlzjfx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eslwcypq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwbghrxe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtwyhg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qzrhunww.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2aowixptl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjcpzj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2znrayzbv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eyegvlwr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ejhitgpl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2arsedqjv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gbciyfsv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hhxooauk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybsfnrmi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kfvmnjfi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2oblqgjjf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wtjxdaws.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfzbifjy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sdvpdaol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgccsple.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qvkhkwin.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jnxmnxvb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2elfjriig.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwkxcbza.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2duakncbf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wwdrewqn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jieqtmdl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mabtuqyk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmlufewz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bxscnpdg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lwyljwgq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hvlwhunu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rcwswhck.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nphmidmt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mkktosha.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdrtxs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhzaeqlx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hmssgdyb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ritehvov.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmlgyr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bctkbaea.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bnqqhntb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zqqsakep.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gbmdszid.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qincdczz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mkihtraz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xdlcuvrp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pxwqlgtw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zkujpnlc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eqzfwkol.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vvalilbm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2oewxrsxv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lnzfacdg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yduzrbin.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zkmzipvo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pnkcibfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2epyytjba.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jwvqrvyt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gjuhwcmn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zuerakgq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wnrhspqn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pnjkzgpy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sqteqjiy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpyohmar.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bnedrekb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2romjcwpp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2trxqsaop.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2knoncsct.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ullzxdml.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jjvkxtkn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fjivdfbf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ijprocvy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wokpszkp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tvhqioac.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2brhjhtun.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngtxggmh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nyvkfhbc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xgxdhoch.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jgmjbtew.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dzsmnttr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gyxfylav.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2txxmlati.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2glzofhbt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oefqagck.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kspzgfvd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2huoggyaq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rsemqqup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlfimitp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bkfdcyqh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qzmixwya.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kowmgcqi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2upryuhme.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ddbcimrk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xonsoita.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wshprrcv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hjvxeqkj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fishrhox.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2udmimvje.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mzfltaap.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yjcjdpcx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mebjuftw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tybejqnd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zbtmpqfz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vhjyfioy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lbfatkkb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2emeulxog.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mkehgvua.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zrgwawtl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pakmctbf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gnklgzmb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2klczhpar.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eakjxrkc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fqlkqxfu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hnjymgzo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vsjbdlov.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ilmvdlhp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pmaufdyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dthhhvqo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wondknjt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgfqhytp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2brjhtzon.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2uytkrivt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2femnyaso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kkiwbciu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cuniwvtu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gjybgqdx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ybyxlvwj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dozgsabq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yblvfysn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2srqsznbr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tunvfpwi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2htkoiatm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jogjcvyu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2awueufpr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fbrlttni.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wzxcchga.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtmwetzg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ldtuiygp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gaczwmms.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybofsxjn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qojobdbx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wgjfmajk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqospich.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cjhzziec.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2glmsusbj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rainqrbc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zzjjldpi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jppesuhj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tfdrrtae.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2razdkcvy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aizxzfaq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kcjrefcg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mtqjdrmf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xbrwlbbx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zurtppfi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2trjxcrvn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gipsxxwj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vauaubpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cscgfeev.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dzuwmnjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djxxbxuj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kxhtchxv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bmrtphwq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zefoakha.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2phrljmgh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2soxunfln.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjvhvdee.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2efzpwgdh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ltqhpwze.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2weswktic.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xtocitpc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2thgqoezz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gcfigswu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqzvsaat.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfvguddg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wyhzxawj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bpzsxpkf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ikogxduo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jollpwdy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cplaqjta.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vscnlfns.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qpeevycp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lbulskzk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jusxnlwn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vhpgstcd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dqeewjdo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqcqrc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2edqsgghb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vqfgyzka.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zxrlhkbp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fppflmdb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aizccsdj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2urlmyvwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eoqbevke.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aaczzqqw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2acyuopcp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lfsqutkr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlskiyhc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gbyfzxvp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjpvyr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aefyhsja.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2loloihgk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qolurhbq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bnpsxjnc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cugpziwt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zlccvzxx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jghgiihc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xlkaopqo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2upiyzlvu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2clkvsjqt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oxqnavxe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2isoajlzd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2olvcauzn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vavuzuxv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nerimxnl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2loowsome.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iddsfeat.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2drmvkfrr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qgzcxgub.html


<!-- 参考信息 -->