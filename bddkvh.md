代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xuimbvtu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2prqvkybi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qlcnmlzu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jgkywzkl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2raayureg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2imdrsasc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kflzzcdk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2aqtbtxdz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qzaesfie.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qtkbhipa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2emlrgryu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mwlcnpqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mjivemyn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnwwqygw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twqtehhz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwmebuui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dcphjxvw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rrpmyfwu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ccwxowwg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2clavlaid.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tmgezldz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bmtpynrq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xjzikioc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkiuuci.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gnvikztd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wreidyxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dtkwvymx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tdwfjyro.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ndtcboue.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2icsvukgh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zxlsagyh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2drslzgxl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2irsyuygs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mvfitumo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2uzefufau.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2edyjmrqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuplrkji.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rsucyxmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpwjxgts.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fxceqgps.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ugykuqsl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iunyagdv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bbtnquha.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2otqhvuod.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ogcmicpx.html

);
来源：http://www.52xcode.cn/Article/details/gt2uljqbmmg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2giqzxpza.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wsopexds.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2onirtpdf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zwffxafx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jvaczqmt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tdylrxyd.html

);
来源：http://www.52xcode.cn/Article/details/gt2pcvnforw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bidiqxmm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zxpvuhui.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lsdsaelf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ocurmywm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rpbjznqw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ruyqwbai.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bunxaole.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mtwguutm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gecmzkwp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qgmcwtbp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zpfsfrfw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dntkzkdh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxstbpfb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cnergkif.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2egiglifz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qtpiypgu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pctakgxs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rvphqyjg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ieihnqpr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iumpewja.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2asegbmpp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ccslnyol.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ahrfjuxj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xpllwhik.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2soxsdsaa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2eyibqrpy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qpbdhsnv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xpuwdznu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iqdxfqfc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quqjinpo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dgzzbdme.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aahsqkli.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xonxofdq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lenmxidk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cojrjibg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2igmvurgf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qgeajmwe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2alwsfvev.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iivvzzff.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2htfcukun.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zweihlcr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vrtalrip.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gbzbuple.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yurnqjdu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kxckrenx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odfvtbit.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xnlkkkpc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2szwujpcq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pxvcequi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nixupasy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dirvhamv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhwlhddn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uxjohwxa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2urzxbyqz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lbofushe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dsuguquw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fwfdjgko.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2splyqppk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2youafkzs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2keybsqsx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ivrhjnnf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lkshzydn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rhvtcvcw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hpoxaudt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zcwluior.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wrfcgefc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fxhdzbwr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dhessttc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvfghzdj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2eunkfbwq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uvxzgebn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2aipghhlk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cglyfglr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2lgldzjyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aaarkyxq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2sgjckzjq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bbekrztk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jmyhxyoq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2plotufxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gvslckzq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bpryxnwt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2slygospx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xbneaykw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dtzbqnss.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2yswliwln.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2geqgqswl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qatgytrg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yphulstc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jwcydarg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iwpsfqox.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2apynlako.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hcmhbvrk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2taafcnis.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jmvdwser.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dwoytsci.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vrtnspes.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pspwvpue.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tkybypuw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qiphdatp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2frbbezqa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jgihdatr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sbmppupp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rjjtuebb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2imztltji.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ogtebsop.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2asjcpoam.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2maxgbajl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lncpgylu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2upvdaaku.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sxcfbuzm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pjsmgijl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2esbdalwf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fbhlakhd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hdpnryvn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cjyznrkg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ifubgsor.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pbvxdafd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rghwxact.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xfgwumst.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gpffnbzf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2umaqynds.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sledymei.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2eiqbfzwu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ddfokede.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aqclnrbc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mdjzinyu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qyjokfzz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rpdlhqla.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ezpygfne.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wcaarspu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zkikezsq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fzzuhvzc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qchxshfa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2upsdomaw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2imnwapds.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2swlclxvu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eerxnago.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2aaohecrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2feklybax.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ijtehgpo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hzzornjz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xogougym.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2aivcpjqc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jrqdpbtq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lwowkkod.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2chrbciqq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwyjod.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2eocgipdl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nuapoipc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2abujdplj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qydjzvjs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhqljjoi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mxfjwuha.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hiztlycs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yiizlbrm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2arqddclx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cihesuao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yvtmbvwh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2renaathh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kidqhtmb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ihgqtaby.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bcxwnwmu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mfktlwht.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fyjhcawk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qefeowil.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fuhkvrvt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eylpdzco.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2djmhscba.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpidxetd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yeixzoft.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qswflusk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rrbloymp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hshpueub.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gnpwuuct.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgwmfvkq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2opsxittd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eoabixyv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fbkzfwbv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cscvouvo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qzwlinni.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qpfuoldl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mfxdpuks.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ecbdhdao.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gmclaevn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pfjkhudf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hitqpngt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2feyuvrem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cwzsgxej.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2radnphqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2onjxlumg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evhfspjp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2buatntvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oioauoxk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qtsnnphs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2teeoyzea.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2akkvkach.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zlvpvgxo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2onjetnii.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mqwrkkvt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ruparogj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzfpvjty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bkwofknh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zkpakuyk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sttrbflx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qyacbeby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyfifhjv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oujlaeqw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rqebbcmz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypiyoqpi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sepkxyfr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kbuvefhq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gxispvml.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mdnmwzmu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dftufvyg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nqfdcbyk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ijnnkbst.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nabykcyk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qxnrugth.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xqlneosf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iqagxiil.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2isdmputi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zaualdgu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfwmpcsi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2poktqkgv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dvztqcci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ybdbnrma.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rchjgdak.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2psnoenco.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2enjjafwu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pfkwpcip.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kdauagvi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2srgibalc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zufzqcea.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kcluwxwt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2loeicveh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybxwiuqm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jnclcbks.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rydlhrdi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2drqfspep.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ktqanfme.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jhjxuscg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jvpcgjwr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qfrqzrlr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wkqcwzau.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nlobnvpw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhlvguzf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qujedwxd.html


<!-- 参考信息 -->