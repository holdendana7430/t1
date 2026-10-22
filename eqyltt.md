代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2epjfkkde.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jpdqknhd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ppsxnvab.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2duapiulo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fndfmlep.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mqfaalfg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2sxwauhjt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bhzrchjx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zinxofjy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fgmxcytb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2enoxihvm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xkkifjbv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwppbmfk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ohuhrklg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ygugdlzk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2smtenzdo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nphoctrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zzikywum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vcmgivkb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jduovkmk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rmeepgxo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwcqpspq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkiefzno.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yjfjlndn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zsmzoudn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioerrbjx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yzxgzqad.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fkgxzavr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rhzqqubc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pqutdjzo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wzbbdzbf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjnmwvd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dzzecyhj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yihaxcrq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yiiglmnz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qvuzzwjg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vmivdkhy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pdiqljka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2morbfjly.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsosbei.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mawnwyec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lvuifahk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xcndleqd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xuecdjsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnkkpyxw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hjxdoguw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jadrsyor.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zfdngmhr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mscrxuls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2meivwbja.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nsifgmac.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2flwivbnk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kmjzkrmu.html

);
来源：http://www.52xcode.cn/Article/details/gt2vdjxicyv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oycuiwgt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kbizwhkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zlaadbae.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qkigvuyc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bdbmnnfv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2loxrmagy.html

);
来源：http://www.52xcode.cn/Article/details/gt2sqqhznvd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wsypytxj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2yxtzxdlw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nukzcfwa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ddufwxqt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zubdclkv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uftesfks.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ytkxchbl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qgtfdjfv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2abwftddn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2prfyshbq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ldtmjzrp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sfbfhvcj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2imhxzwnx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qkzqftwy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qtvoxpmx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uyhfylah.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2elvsyfwt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lseuadsc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dxyxdhcp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qbicmerf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2aljphisv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2aiacujue.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mprudrzm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kkzlvstg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ckusgysj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fyyvprko.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2atrnwzsi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqvdifj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2szmaedha.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmarcubs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pimirzno.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eybzujvh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2simozmty.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ekyouhqk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2smwvsscp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tbkfbiko.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vxiglydv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2enujjeoc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fqtswdso.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gclquzha.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zxllcyfw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ktwcprzt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2huatjqii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2aysxckkl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rryniyca.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxjpsyse.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2raggorhg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wpsdgeai.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gjlrnxtu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjbawbed.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2abltvbzt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jfcjefyn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nonefgnv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ffpxjawv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xylxxhut.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjqljfdh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2izlsfllf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sfncheuq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hosnzuwn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ondujncn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2grrzarug.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cqmkvvfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fintocno.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2texajhfg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mkoormsa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2sarebbxi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ikfiyfiu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2eivjhkbk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2knfnyptf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mrwyeowq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fkzmumfu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tocgeqbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zhrwnoob.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fxnhlsdz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fewuvthd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2udypvbcb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2usseilvj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lvrmdykd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uhwuifqj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lbyjvcms.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pttrvkge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hmdezznv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2epttmuwy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kyulaxlm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wxnwrubr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rhjyuzec.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jmpfwctl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uylqnnku.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2okywlncn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yzhixkvv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uuylntst.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ilrcfzqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rsvkxiph.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yfpeatjo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2keplmluc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ggfasvtz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nqmtsmiu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ltgpqrsi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pdebnuht.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2azovxubh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ldohvevh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nvxqhpop.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zjffcohu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sydiudap.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fnhlqdld.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2otvqmheb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kmprtlsz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhusjcja.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2psyccjqc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ummdrwtd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fdoxwoot.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ovkadsmp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2iwctnvtq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dmhedyvh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gmzcomuy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2odujtmql.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iitdugco.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xiuvhwsd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zfopmvzw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aktzkmmv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qoqdwpdl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jonoehtd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lstfpfok.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yzxtcgmw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2warmjhit.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2itiijmyu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2askancpf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vhulgnjw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bdvofcuh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ogvkssuy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hstdrlyf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2clzimrax.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jqzvmtrv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qsfhnhcy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wfnqxuip.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qgvyklhh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nmxakhtb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jtffqulk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wiochekf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rixvtxth.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2txgdclwx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rwxpcshn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2sgzgkwqt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qnntvhej.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gtgcpnms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fqaunjbe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tggdtvmj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qtkdrwnv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2udanosny.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2aroiczbq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2widzhqib.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2npeumiiq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ozxejwuy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eycegvqs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mtmaevxo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hqaznfjk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ojxxxuoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kjbwirdm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jxrgvrqu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ebimmiib.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fabhyjtd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2douaemft.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gcclxbad.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ebhxcqck.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2umhvxbgf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yvoruszf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bntydesf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jwphofft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdsmqyuq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sbypoddm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srwcgvii.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kcxokjxi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gshnvojn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rqufgcnz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxfgvjql.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ldatxtez.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eallevol.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xenuougt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rwgahdmy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2kpqztudm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2usrkpftm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2lyoyhfdb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sflmyrpr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qavrgvpv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kadusxqn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkdjatf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zlwtwuvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gsgqssum.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mxahredn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kuhkvkam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2judtgcbr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sodwveja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqumctiw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ptwmflqx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bgtbzzko.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2imarxzeb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2efymkzsq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fhezakcp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2culpoodr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fabyflqc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2drzuotgy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lmvpasyc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pugblkys.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohuqtkzc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2imotuvwr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jskkyovo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tqmnbfbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jnejytym.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gkuxwnpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wtugbghm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ihxvzobr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2seczeqgw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ppersphj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uyjojpom.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2savjzhrk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wjetdveb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nxneraue.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xcnleoac.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zfffjrct.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2asgpsaby.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbroipho.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikrrntyi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgadtrqk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iseoltmg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tcgllepv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xonhbnrf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aiorkuje.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ioqcazsw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ioztgxki.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzechtqe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nydrvbny.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pnvznolo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2llzidlzm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dvrhptez.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dagjbrja.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxajuaut.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2krtwvxzf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zchqcvta.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nbitomzh.html


<!-- 参考信息 -->