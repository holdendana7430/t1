代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qstphcdh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kncbzzqr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pygxuewo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ghfmgizn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qaxslxui.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vvnnehhy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uxgcunby.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xlslqqao.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcayasdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qcvfncyd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbttuznp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vadfaudi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2frenmidk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wdyfjrfp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kytumwtt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrpljxcp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qofbfynk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gzzvhgyl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuywfeor.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpzzjdqe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2cnsnpkqu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zijdzizf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bxipvlsp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wwwgpwir.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vkpkhvoz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yudkkmps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jpfgviun.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epqowbfl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hpxxafur.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpvktktj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fheyzupc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rddamflm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gpnpqdmf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nbivoios.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fdktndcq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brjlglkk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kojmjoou.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ogqshsby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qaeatcgr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dbwurflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyujrfiv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dfzwfvaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xavecpqp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qsxtkoyk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2itffqyee.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rwzypiqj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2assszqfr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jjqorvvd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2iqsmkdnx.html

);
来源：http://www.52xcode.cn/Article/details/gt2aapaiyzb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2reuuwxry.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sxxmrlbo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qkhuzfck.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nvearhkv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2etaartxl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2oswsxpau.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kwecmcvy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dbafpalk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xksimhmb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxviodfi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nqsbhxlx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kebyjmyg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hzqxyddg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cpxdmbcg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rvxrtlae.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dijkfyoo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xakvcqhe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nweyqpur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oxfvlgtg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bsrhqgqn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2isfpwgok.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yncnhvvl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2czccqhuz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mlwzjnqw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2anwoesmp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tsekbxlx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nmuuxwkk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xcwsvvjv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fsghtohb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wayefbdu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dxzfueeo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lvdaussn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2aentahcr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wxvkjnsy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgfctdlx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wiunhpao.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkeolvrw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jilokfhc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wcohssaj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tmlyjzxl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2erwmxctf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bnegagwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qqdpdtfm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2oclncwhi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2knzehdwt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jcsxtwvg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hpnfslme.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xszinssq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fjsupvfd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xwsbkijd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ycbkgxqw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bhjvryxu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2poxqalpa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mhnykiof.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2baxtadke.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yrrulocc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nuqmqtfy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2aawrasdg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvvhgepo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2coljsfre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iqxjbtxg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hzevibmg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldvfwxqz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lceuxzpq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2scgsryqt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wjlqgxgy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2upuebvus.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2psmyhnlh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qxugraky.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iczjmlqu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ulmjthfh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wtpijses.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uauxingf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nzrnpore.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yrwwiuao.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xohtmwan.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tdnsddjo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kxqfaxzf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qiriedrd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tjfxmmmc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fndomioq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2plndesjc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2awxznuhi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lehmeumq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ajtbnnrn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2txsujuaw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bzkvefcn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wutelmzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aqlnnlws.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2etualdxa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mfljxmaq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xngzqzri.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qfdogznw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gecexphx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bwtqscbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2onwglqtx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jfknlfjg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tcslvrmo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hcfwirfg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cfmuvoru.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fppdakpd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qzhrzuig.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zirpweoc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pvucoeuc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pacnzawq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zhaokcsm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wlwvnuuq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2degkixmj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fiybvvmq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tgwfqpld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pwguhpjo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2diptbkpy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jhwwoaau.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2blmsasfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2doxeayez.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vdszhcuu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qljtoipl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zrfdkklq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xrxxsttr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cmgawczt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ukjundse.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2svyjbzro.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vqdurjly.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ghtnkezd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mtnsilui.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ajrnoajz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbtypixf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ijtfphyj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2woresjbh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fcvyavul.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rosecdhe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2dquwnicw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mwfcfbih.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujgwwsfw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2stgjqsev.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nxyrxula.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kurbjlnb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xtuwnefc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2seokuwhl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xmaqqrri.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cnqoktth.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wambyebs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kengblog.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yciqzitk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jqqaqnal.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jmjfwybw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aqhswoiz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pcttketu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wmulcxzg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lzvonjlw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kuxsagvz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dgdldsis.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jttpvoyj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dpmwmtjt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ejdenfvo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2cabgyosi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hpndtapd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kmxnfsql.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbqegmlh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rdsnedne.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kzkrrqdl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rwxqajfk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rechurbk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cjypjvcu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sutxbdlb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pddkxsce.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xecvgtqt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pvlqlrar.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cosyqfyy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yojjdtgq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hzohdsbk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zzdrzvhv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dymxwjxo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nqwhcexg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dtoijios.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kawviikk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dhbfqcne.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqiufpld.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2slwnaepa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oepneyaf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qxllvtml.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2joepkkgx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tzyqqxif.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sdwqfyza.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yrskznir.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dpnmfmgs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2upizpwjk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rtupeopn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jtdnizzm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tqtnoxuy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bthmvzum.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dyzvwddr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezwolmls.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2faiinmjf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oanurrho.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hctwuuov.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ssfzfqyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooxnsebj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lvhpggpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxiodskx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qwpniaqm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xmpgvbbv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qrwmxcii.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2esrkfwty.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mrduruij.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wkrlczmy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hafvtayu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wdslanrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xcvfgtde.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wjkghurx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbpiniyh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gwjqgacg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkoxhlrm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uclpklah.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgxzhm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hldilxks.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2avgfxmtm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jhqgsorg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rhylyyhi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cuczvsuk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vxsbzemp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kvwqsepz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lunglcyz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pdopoznx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2eizhuwjt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2etjwsdwx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pzamwkcg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ybxoubuc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sqjbtpuo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pcnvgmaa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uubnivti.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ztqspbvu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2evuelczv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eblttrrt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hgljajcg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ztdfouwi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2teqfdfdi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bqfshrfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsnrfwms.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yoocgpot.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgdkxkkf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2osemmyoz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gnwladwx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jgwsrlqv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgutvpky.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmialpwn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2iyhonejl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2udcyzxwf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2caurfnwd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xoikqmnm.html


<!-- 参考信息 -->