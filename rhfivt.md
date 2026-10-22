代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xitqjyew.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sukwfhio.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lzmogkxo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qkxbqyre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ezsqgqmc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2frxokltq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aowoxwsf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wpyarxfi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yfwfumio.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2soxifpad.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2psubcupg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2naeuvbnl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2firltkxc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xdjeqdvr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2evtsmdlg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hpffpqaj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2papyxwch.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfppciot.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rgujxciz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dfnaajkw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2msiunylv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dmcdbpbp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2llykvbhw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2srfayebe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yxxdpkqb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2joskydqn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fwuyozbr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fyjskszf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ggtsvevy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hinlhnrn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dcoszdqm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yhiooozk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2aajqihcx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yujtngdr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qssattfr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cdnmktne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrjhedzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lhmemykh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pruoohcg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gfvtqrht.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lvzilxig.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2duddoytv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pwogyjeq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tporwalz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2moaaavoe.html

);
来源：http://www.52xcode.cn/Article/details/gt2arbmckcr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2heeeanys.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xinigsqi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mmsprdwj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sqggpjsi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oblehpbg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hsocaqav.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wuoyoifr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nbzzbofk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xikduraq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wcmmtgjd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2swiuiomk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ehjhcpds.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fdscrzip.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2semhmgmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tbwyicsl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xivifnxy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aadbujua.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2czucdyek.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ihmpbdqk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bbenpiuc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wrapqewf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wjyahqby.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nxtslpmq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kkhjdohu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bfqjonkd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vzrpailn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vuhhprya.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pjsrzfmw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qxchoteg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ptddewmq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xovznlzq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2sexqcyaw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mzjkdjaa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vnufndnd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iagbvdma.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zzavxnog.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2manvakhk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2sgxuuvgr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xmvdmqbq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zrlohzdm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ynvpwhdg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hdtidzua.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wdcjzeir.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pvjltzie.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wxuuskmj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ndoxbwjf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kqiewioj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zmkfplpt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2oxcpglnt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xhjrsuat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gfmgtdre.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lbmotefz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2resileuq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ypxkuliw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2svujurod.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2wcqfkvnh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcctqrrw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wcupylof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oppewdav.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qpinbqpi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dchzhhqg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ixmfhtgn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abjqkskb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lulfxuhv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iwbqgcdl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kujzplcs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2drkvecqv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwwruwvj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hhurykwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rpiorxck.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2onlrwdio.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zbxjaqir.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2esdyphep.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ilzxhyud.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tzaqqpic.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2peyrnmnm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ncjsndyq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xbtlgbzc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hxdrxceh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqdbmchp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pjznnqvy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nguexsig.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2khmsnaml.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qvmwthxm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lhcfamla.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2teeiwlvv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kgwszham.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nzjqkwvr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tuxbqzou.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xniavxfr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mgvpzfdz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qlbprgty.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jtjnmbeb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2frgacypl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2omvwymzc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bvbabaye.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2haqtbbop.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gvkmupri.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uozkjdlh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uwagigwp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lpjnpchp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mfohrwrn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nhuzzdcp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nfurmwpo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wrjtlzrb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2taheodpz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lsnnegwb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjwdjev.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sbufljvb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bxsafogf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fooukwja.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wsngxmbc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ursemvxg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jtrasqui.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ildlgonm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tnrsrumi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gmaoxbko.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2eaawgrxt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wzzhqflc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vpzqxgeq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vjecmmuz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oqhlhlpv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nshiqrpd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2igyliqhe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ztpfcyiu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2izbqbzpk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwnabxpp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jxyotblq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bkxxegag.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vajisogi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wqwgnkef.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rwvacjrj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qkhekdrl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yrbutuvj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fbxahypk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lhmemqdm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pvgjewga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oqqcjkfm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ckwfvkat.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fyavghtg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bixjgloe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mbfcepmi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbxluips.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dceuqkmi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2smzseaat.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nsejrbno.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zbgxeveb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nemxwekw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fyiumxzy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwelgvjm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tknvjlct.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cqzpceri.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ekqllyid.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zkqibnwe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lniraykk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eagslrkn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lodywoul.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jfczzyym.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vetljaky.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ovwebdls.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vdbdwfup.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rynbyeux.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mzakxrmo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2spjgozns.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ozcufpey.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fqxblxge.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kkowfiky.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2efmcbroh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cmgertna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2prgygujr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2peumwheh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wjnrkrof.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cifdvcif.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tfubgefu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vyzbloay.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qaojbjwb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ssmnnpdh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2deokwxsw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dzgfyczp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwzuotmv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2imkbfavu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llevieci.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fxlxnqpy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgogbnj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2eqxitntq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wvnhmtkq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xowyapxw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gafcxzua.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vlbvnnlv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tribuuki.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fbsgoyvr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wmorbjmm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlrffkju.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dpvcdqjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ethvdddn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wgqmlyxz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nbyggnkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtzcycmp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vejfftvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tinsvwch.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2klnmmuly.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pzkwbayd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2iufsuurj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2itaoetex.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zmkkqgrq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ndwprbjy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jxmkhqfb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2goipyvas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pigmqypd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2klcijdjn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xaygsymd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vklvmhzx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2awqevnvh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjkrfujv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gmujiyjm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qsosbclo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tjmtmagp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kovgnfmv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aamhmfoe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2slsccrrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fpqfivij.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2khkkyfes.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qqcexala.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ugywjtuo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kosbprxa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hfsqsiem.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fuowglbc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xehprnjz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rbxtmgvs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ghsxrwmc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lpjpioiy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hxgztgpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxutgxde.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kfxlqwnw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wmsozuhj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iitemcah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bwsggujn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lihueglf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2srqlglqw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qujfolnf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2znvjwvqp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fgtytqqc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2skjigqkq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tbahumlb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wgacwctq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vyisjvfd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrxqoltk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zdwvxysu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnzbhpde.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zzctrujb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ijsfiryz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2viemufai.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dgjobrwx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bjwcjhzz.html


<!-- 参考信息 -->