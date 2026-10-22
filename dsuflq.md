代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2suthqcdj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2obvlqeev.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2opamzvgq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nnunmtnu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hyhrlmyy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zzjqfnbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zgyqruqc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzebvaa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wyawcemb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yqhgyozo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2befugzfq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sosbsjtn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sbulezij.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kdnghhfv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2umiakijd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fkrjkubf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2itdecnkc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2eilctiyj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2seajsfxu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yomjvzjj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ckiacroj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oapmcplf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ydwixcaa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2soopwpta.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfxvjg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vnfklgdf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tdehxcgf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jrbgnamg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2thtjuctf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uzepkxcb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tcfxtrip.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvsdvlmz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gunkhesf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vdkcctcx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2envxrhoj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zupbsxld.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzknvcb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnjqbcah.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bcloiwnd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iaaxtjnd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rmiqdxzk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fohagvil.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lxkgqfgb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iawknifd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ckocdabc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lwpkfhxx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bneffkqw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jzdyfoot.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2neutpeaz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ylcbfddw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hostdbjv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fktatqgg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dswtroha.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bweqzrpr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2icnrtjql.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wddjvpds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyhjeygk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2leeyyqhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqtvrihn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ohwloxqs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gzpwrmom.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lactjnxu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ntfqbhuh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kfgovxmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qebulesl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pdsviruz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dtmvvhzj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ulqzijeb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dnwnjrxf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tzcuyqdg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfrkka.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wklvzbbr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jhzvgrwg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2raqlaozf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2edezltvd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nxvofzbb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zfgxtcoo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2whuzsyfo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lotuehis.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gbthtrll.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ybydnurp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nthywnww.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bvqwhpyq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mifvihxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eldcefiv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dptlirjx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bormzslb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ksklmudn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qomhghos.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ijmfykxm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bdukfqnb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lixtnirf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kgznapls.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sennicfs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2parzkxei.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mioqyxct.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxdegc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2omneyphj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zjelrxvy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qjgisivs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtxtcztd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uxolbive.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unnvwrja.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2anyqlcui.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nemangzz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ijxcymbb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vkyxsuly.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ihieipin.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cofbvzgn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbzkseeb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yewjpcqp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kursowoe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2annjkydn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2plujdogh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hlfpafhe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2oeweirwh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2nrnkglul.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2typildei.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynmzoxmb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nzxqygqo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2eiqjlosj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bnjwbawn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fcpkpgxx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2iotoblza.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpozpcei.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hkzbikzk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xnrpepxk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dphhlvxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwnhuaap.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ukwtkgaz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oddgvkvk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gegqxntc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qlmqtegj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jmuedijh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2edjtkqjl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cmmdqzcd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2aijlrnzc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pttklnic.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ubwbxafs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2guqbwkry.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2aanxciwj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvsdinol.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2omuiopsu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ixrgnyda.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yllkqche.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vlmwzudc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qmzdchut.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mmueydkw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dtfnmqrd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zsxaezij.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2paudoanu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ebdozgdq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zdiiqzhy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vdczajjj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mxhaaanj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zymbjvjk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fwbbzndz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2harndivw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uksvmtbp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qyvfbcus.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cswnfces.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ompcbdzb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hjacqfvl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ukqobtac.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rpgsalqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rrsdqvrv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rfvnxqlc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tgitthvz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gitkayae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2amuoeamx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2sgqlnpjk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pxmyicgz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwaswnlx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jnuwqmzx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dntrpaft.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wylnmuqd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bquolndd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nkhtihcm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dgohmadb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2evhyholh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvzhqsi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dhjzntwq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qiqouvhb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2emneoupi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2erzttfbm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gzssquag.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdgcto.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lppecrrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kicwhgfb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iknpqlrh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zfccypbz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mineedqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezwcwrtq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hewoxhrl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ttehvmus.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wsiklgpj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izbzbieu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zxawztwf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bmbintfs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2smrsplhk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xggxuxrz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tvjsqivb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2knczlcgp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fvwnadgy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xluwlsxo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xixzftjk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2agmsmutu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pgamkhad.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2phqovoel.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mmyduawp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gjowjobg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fmqpxbht.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nsmmywcz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2psmnljuy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zyjsbeas.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ovbpzzxn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qcoephix.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2seojwfly.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2uncvtzci.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lwzjffge.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrrnhwv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2msfcbhhx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mfqzlfrk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nobhbkns.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2muvayzvo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fbujcino.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qoianpdh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oekgbqen.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2sxskjudo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2loyurryu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jfqrztys.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wsilsakk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmkkxi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uljczdvy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bamlyabq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nfsokvfd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sqeoqlyw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lgyskmop.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wyzmhvuh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jzhejevq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2umhifwpx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzpodnwb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnjnjaay.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwzapvuk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dzpsxamm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfhccovg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwlsdl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsenamln.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rizbovom.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuxodkqc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xerplvpf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jvvvnqur.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2opvjoshs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2snyfgbig.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucqehzvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ltbtzyfz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2siaztwag.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ehdydnaq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jumxsqob.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jikgwnrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wdhxulbz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2myabvych.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfjpqxtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqtanqwf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qtmhzuwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrjtsnmb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2adnchfef.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2icugonvp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tvlvccjp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2evpeollr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xlqtsaju.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvcmufnu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yhpkpsim.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oldwktyr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zpdvschp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rynzubqw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zfecufte.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cbrotcpa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lpnvjcom.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pnkuusmd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vswdujmk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtgvvllb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2uryjzvar.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ylqcmvrw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2aamibdte.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vwcwqgxd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2teyzhkev.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2duyenhul.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ouafaksp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dugdyxeo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2krjgezib.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gimgfzss.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fggntfty.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wbjjogvc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ecsurnqr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2taektleh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uanemdhw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2purqqvhi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rqentpcm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2snackrhc.html


<!-- 参考信息 -->