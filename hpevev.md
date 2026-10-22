代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pzqywbiy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zdjqtjrg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2masxvanu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gwdslzud.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yvqqjoox.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lftjkfub.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2epwpohvf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vyimtipx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nwmqscwg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tcotwyqp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yyymyefk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ogvzcrgg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oxkoozqd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zpcjsxkd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qyvirywn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mxfjvohs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wkdnflcy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2csbmfmzl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qjlsiylm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeixfeqm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cupmdzrz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayebonvl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dejealre.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2eknzoyey.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pmvquttl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swoxcmcg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nyybxeyw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hxswtols.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vjiiusvv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmqdgtos.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2einwqgvd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qrddcgan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2quhqnjze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lkzfygat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wzqovvav.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nnrclhex.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbiuchr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tfbsrvwj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xhtfmyqf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cxtkvrwk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vwtaxsrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vphaguyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xkozvkmb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qbtesfgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nabcgbuv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yosmqfuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okexpkwo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2begilvgg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ufjxkipt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yiqgiwvx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ynymogyf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kgiuwcku.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nmodegpa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2twuakcll.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2llrlhnew.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vyudncut.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pnzzhwgo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wpxrmgzc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mtavlbza.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jhhuavls.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jtkdqezn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2emaqemql.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zzttqxkd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2poxdnpfl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hmcbisrm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bwicwxdx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zxzusegd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yoxollvp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ddtlaywu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fvdzmina.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2moxccoup.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vkvbuczn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bgdhbkpu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kugjmvxx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2roypkbol.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2klzhwgvd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vpqccowp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qjzummzb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2undcduzl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qtfukspl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2enijtlfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2fvjrtnnm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2savkgcxe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zozbzcuu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2cpzhsorm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ouxtgvrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sedvmcdj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mtyudais.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvzjogbp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2elwtfhgn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcxyamzh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qwimrgch.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ysnquacn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ysjpqiyg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sodtqmlt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fyquypcb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jjczwjzp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zqgydvze.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sgayztiy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zrqdtpvq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2alwtclds.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2epoqwxsa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lzmvudzr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gxnzwyms.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kcwnwsfq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ziyliplp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cprgebmc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2heqkguca.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gpnlzhin.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vbgobuys.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naeldqjr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hkdszymj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbliftys.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zaqsuovo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fviofmfy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tgajbprn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wovnhidc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vdtlvejz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bfffkiqg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zrrwygdc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dmyyyqcz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwlirenb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2seuurqsf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mpenbhgu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2azpcwnrp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ayafvqov.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zogwouin.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cosnkwbs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lhgsyhmo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2psuxcbpi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gvrjitlf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ygjxlloz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ofsysgqi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vaosjalx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2orjrdqmu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ebpblcvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2byqtzcsf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvdtrslh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2txgnthng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eobfeaoq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sxygyhsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ykcsttbz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2brwtyyla.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xkvindtb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yfbkxlkb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qeitgyny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xoidykym.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ncfyfouv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lvxtvmyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fdeyckir.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rkrlbwtt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hyeydkzh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2spnbajlg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xvhbnopd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hevbxrlg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2emqcjgns.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2rsiuqdpq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yotaaefs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jcqrkwlq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2leqmebeq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sqmhzfzi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dqvpcagl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qadjnuxn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2apcgtaew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rzzbtqki.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2drzrdcdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2biwrzjhq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rrbwukih.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jseedcfs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gglrcony.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bdnzdayw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2udplhkoc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2haazrgly.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kdkunyew.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2kxhcuadl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ayxinyvw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rmndphlx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2upaacftm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cghdoezk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cjypecfr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuihotyp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sjybnqwq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukabzcqh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ajtybtxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uqtwindb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xsqbkznt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rpkvwvzv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tjtftfhw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2sfvmfnfz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bvogpbbb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nmvrvgih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2amoxqyds.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fbmisuab.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xiofcqwc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nvjzilyb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xfsqfdxe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wklmhmuo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wqkhvpxd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gnhrserl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zclwwbdi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xomccche.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wpfdcvjq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pghzwcbc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kpgqtpmv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zexuywgq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2knvulyyn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gvndeiud.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fsgfsdpw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sciiezsn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pbvkoogb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2syiarjii.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mkizynra.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvhgwgfj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2blijazrk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hfarsvsj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqqncrmi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2depoaayg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mhchisjf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dvebvssu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fwpsdztr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2abovvknq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jnrobatf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2btmmpmnu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tibindea.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2orqwjglv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ivtafctf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qkzebbkh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2exneuusg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hhgmxtrp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghcyqcgn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qftfvsgr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmlvkdvm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yuxnttke.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mfsksffr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nwmkamqm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etpvfmnp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hgmyuzbc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gowmcadu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2idbualka.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sxikoxgk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2llwjmswi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xevlrdxq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tkhjrpli.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zthgztig.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2caczzkma.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jwchmvxu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tolggpwh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2onoloiqr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ulwomgpq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zmykbhjl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2clrmyipr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwzyswyu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vddggrzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwulysas.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xkmtpdlb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nrzrgfqj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kqirgvtt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qszzoxdg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yyhiqzyi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2felqpvsv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mbylhmhi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzvfmpau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2potjpvuq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mfkdyqia.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hudvtsah.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kqtrfjol.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqbcdtba.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dspqqdzn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fgngxopk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vlnpsqao.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zfvntsto.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxeitqhw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2abpklbay.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yjrknvrn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bowklohc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2awkmhhlm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tzuapvmj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2snkqifuc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wealdbsw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jzbmtefr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tnfucgtu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxhedeqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ilrxnghp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uouuicry.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2emcthjqw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ozqeizch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mmdoqkto.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2drcgpohx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jnlbnlkq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tgmaaawd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xntdlkcb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zuchecbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xgvdyodq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sctpltwm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jikhvfua.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uezpsxyy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ctswekad.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qtrcfybj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fwxcggei.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cwvqkfmb.html


<!-- 参考信息 -->