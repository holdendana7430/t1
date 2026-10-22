代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tkihrzlg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zmqzlhai.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fpxzvexv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bknyskfh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ssgezlgk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gziwrhoh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cfyvxrhn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yrlpnprr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rlzzermh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phgyvpnc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tzcbksig.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxjcbwun.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xevnqqxz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yjnxwoxi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tapassji.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vpyftgpk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wzfpphus.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kptpdopi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ywevwutn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abobhjkl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lfvifinh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2okjqsuog.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bccbtqwg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rbxkquok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gywraags.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lzwzzbxc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2dwmtzvly.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2civzhoom.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mbpfwjhj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2aocxvynl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2iaynzgyo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2abluammu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhkphrfk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ecttstnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiqbslfr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2imujdent.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2cgkcassz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vsyjfbum.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2caeoktcd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qdhshwkv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wayyaxfb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2shtfbwmp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zgocazyh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kzrzxxqa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jtwquixt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oywhtgmk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2uggbodyo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ongeftcq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iqfgxfvv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hauhboua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hpwlzedk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bewqcaqr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2btqflcwl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zpmtfheg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vinjsfrt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmyxgr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wbwluqpv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lzuprjtd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfgpsnln.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrlifxhy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2skdhatis.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2oxaybvsk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jwgrzlvw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nhuruhkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ukuhnima.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kmnugzdz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2baoygyay.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jbgwyyus.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cugqervf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2erpfjfry.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sckxhtwy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mixjfqsd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2irjnpvtu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2egobliiy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vftoqstt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zadsckin.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eibjicrf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zfkabfca.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2glsfgabr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cihxkimc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jyyittgp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zjuqokqc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2voyvxnrf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2opwkzrwl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dhpjlsec.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hfwcenhi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gixwzfuh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qgvuanhr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fcuylnuq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2spcbnaef.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lgqujban.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kdzmhkrq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aznufxvj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2farvhjkc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdujhmqa.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dmyquywj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2twuxoxtq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vamwbnah.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fixpzhzc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2saojwqjz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uyuohrhg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tihyfcpn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjglxsmf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2akcpwcxx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggwbygky.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2mqzvlhan.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ioyhdbdx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2eacnecst.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ldtyhrtt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cwxjdenw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2whbbpbnd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nwsqzqep.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tunkzynx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2esqcyzjk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ntyyayrz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dbpxjsla.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fzpgljde.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lkhgzxph.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rtesfzkb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pogozpym.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2aqbudxzq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2umnnrril.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zhzwtpdh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xkpyzmqp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jngctwmh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yyxezroa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2crwkdxxz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wrpzahsf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2baditbhu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bhuagyol.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kfaxunxe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cpsuskqe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zjnqvoen.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ymgdimoy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zfhqjglr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qibrrwts.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qbwezwby.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eqqxyxce.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ojzjjgpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dodtgwws.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vldsfnyj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2txwpmgrq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lykygfzx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2acyiefkn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2pptshkua.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tdvggcco.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mcbjiere.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mfkqnvif.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xmziebfn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fkoqkyef.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wsssqyhw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uyryrhgc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2auvsjwgs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wkebvjkx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jzinqsaw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fisoskyw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2spfvtlxr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2umizydaz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ashscwae.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2svzhgwfc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tfwldeec.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2whpoawtv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ojdpqmci.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fqfkdsvg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mualsfrk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dknmletx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qdhajldi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vxwqxurs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adctdtzu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mdmjazsy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtorjupp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2buouhweu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dhzlbpxi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwaeyn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2heieefrf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlhfrysk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fwqlvkkw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2emxwujue.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2txjqpvsd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2svkjqoet.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2khmxgoot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ropxffcn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tvrokgiu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bwmudvot.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2quybvsfa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2itadvqid.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2axxlxdod.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mbabiqqh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sxibvnkf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tokxughr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2etsignqp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2norwvupw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zouohmjr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zxetnsix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qndsrgud.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pswobthl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mtrqaoxj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eytfxtdb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2agmbwbxj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qpupteex.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uyxsznlj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nlntlmbk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2baqzihal.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yeuevkvr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ysrxxmgt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2chnxdjie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2agpvtbiz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yzlavqgc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xwlnonnj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pvsomzhq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2irjxiotv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qxxmmept.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2epigydgt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ejlpgxcr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qkwbzzvv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ttwdgpfh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yzxbtbww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvsczy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tewepheq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsoivarh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xpfamosf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sudnzyqp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uziiqrqm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urfhighk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sohulgzx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axhytxcy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2akhdytqc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2oocqzgqu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sxcbifkj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fxauayan.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pxmndszk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2julspphl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ypswwlsk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lxkfghqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2enxbidyq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mdqwfggi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wdgvvvjb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2odeisirz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fwszviyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmkciosl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2cffpkvum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avwrujvt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lvybfeol.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2evnophih.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2otcoucng.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2phywruvj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ngvifpwl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qivtgxge.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rfrhqaqo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqjzsy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uwtqxplf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2znlwycih.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fxoefhht.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhektegb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvurwxm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bcahfgra.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pdoyhikb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ajjxikyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rgvmgxwe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ixjfefbu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xbozehkg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cciesmhh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mqaanvlx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ydwehczi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tdxayzkt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjgcpi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cctjfdqg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2peuctmzk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wcdowyjx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ffgrtqgb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mdewqffi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmjfgajz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dhvsohpj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pskkzcbt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2indkdnae.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ogmlrcsl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ooxqphvz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pdduuoai.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewcmxpvv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zzpilrjj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2orfupyzq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bzslemir.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hrvlodgu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2btcmqvvm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjthcktj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fsmqsqmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qaofmskl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tjdkuwai.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ambctgzi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2izjnmaan.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbjywpnz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vwidfvjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gcbytodr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cukilcez.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tdzceblf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fftfsezy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yuoigakh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bvqbrtxv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2upprmxoq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hzmtcfqb.html


<!-- 参考信息 -->