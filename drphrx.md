代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfplqeob.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2slwjazmj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yoltjbax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vbuoaeam.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2cxqvwgsk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ivsiqxpx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dtuwafer.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ozfcubfv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qbikhhrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mucbqsrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dthopkav.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tilvwbft.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zudoxtzb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zdyltzlp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oiopqgdv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mthyurnc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bdhbkasc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zgzerlpq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dkdabpin.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ktubbbqz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uzraatih.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zmywychf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hmnqdboo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jjxsojxr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmqmqfqm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cqwwkwos.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqekiqh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2blwrwkoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2boeifurj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ivjpndxa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jaftnnir.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssoywssg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mvqjtijq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wedorjno.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lfaacsxk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ucryuqdf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2tjgtnqtv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myqtuwhs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2giaafvhc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kvpoxudt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ixzzgppi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2idwlmeax.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tjcyohco.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwbufezg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ojtrvxpr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sosgzxus.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2muldsujx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2taawhczr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lrhpabuf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lswtywqf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yftopsfa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfodneln.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kucqinhm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tyuhjnkh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwgraq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2joavqlns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuseumzj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rgaadzqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrjjjdqe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2swoaaigs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nqrsltwh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uuzefmde.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pvjyfruq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2khoqaeuz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bsdthywi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2btbujdfo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ppglpeao.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hguasmrr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vcahlbjh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kfghgxjy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sdlibssr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrfdlki.html

);
来源：http://www.52xcode.cn/Article/details/gt2xciaobaz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kjpruwns.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2brphqlve.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2heyqmnun.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvbzxq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vwuoocvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vskdutee.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2onerhiro.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wwnngbyx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vulvkhvn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yuxhnbkj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mzxucagd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ecunstik.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cdovyjjj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fwnenuhl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qtouqajf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tlzgrpld.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ikvjafcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2onmnwedx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fstvaylt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mvutewkz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ingqgtff.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ktcpgdor.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dgndiqrd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2prphytaq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2akapqopn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ztthhnvo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xwoxjixe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpwxbkca.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ymojgwqt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekbiomun.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dszoipky.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dappledw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrwjqyqk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fiantihv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2axrojztz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2njfejhbz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqxbhi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qdlcutuf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qlhyyojb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2naykddzb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ozzljqij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vdgsydgt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wpihjkxi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gehgndvc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vovdyvxi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adbnvgeq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2slgdkujo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lrlzvoxf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vuqhidfb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abhsisbz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2duqliuls.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odbwhbae.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ftxfavdd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejhnxwrv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2psdrzrtv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uokkcsws.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ajrnjkaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2frkzlorm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qzamhwhz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oaimnvcj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkbcbsgp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bklrzwgi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hnvcfbcn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wuewbgek.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2idnywmdk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kegjpoat.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lqchrkhv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qgzfgixv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2spemspps.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zgvvvdst.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jzmeizho.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nrtzrxnu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zacodnuv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ziejyido.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ivkxttef.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xyrakqga.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hzfoeycq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iyofsukw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bqzfbkst.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oxjrlllb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tbqmrzqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2svvbzbwz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yfvucalq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2aavccjjj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2idxsxuvx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kqxzttwg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dqzcqseg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nfdkxtkv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ecaqrikb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2manjldra.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2iywetyao.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wditzjii.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lhvyksdl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pndqybzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gxngasij.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rotrtlyp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cudcgrue.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nrgobfoo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lzuypebb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yhubcrwp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bxzijvix.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ipbluise.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vzzebyzj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqpwmgk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rawdvefs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2srayvyun.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yopqhwfk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xtozgnar.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2caqhhfyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ghyyptod.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vwjopdmt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vwucixxy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uuwriknv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2yvewiesa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mzbmkwpf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dnhhrwfv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2agwkkwlg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jjlxoaoe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tfaaziwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spzcfqhh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kwsmaqhg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2orcgwfxy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tagbfore.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnzgaebt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oogssveq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iodddjkt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tpfzkxxa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zabolwsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fikxccuy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nhwhjzih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dobjtlmo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ndapibhw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rarbkhmq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xijzprxe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2krixmwio.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dpkdgxbj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rxdhbneo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jxfraxrq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2topxiwtf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ksnmxdkq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2szlfeaig.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qhffllez.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vtoplxlq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iudrzhyu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vpgrceya.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yeyuyxfs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2syxbgkqy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2emluuhwe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pqmpnntt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fzyardku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2myjjxnco.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvmhgadq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2aupnwfzs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jqxzobvt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rmeaybml.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uhhrwkxk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efvedvwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fqiuzgpw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ajwzorao.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2afthdqzz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ikmhossx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uvzyztys.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2sagqrgmw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2znhbjtla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qwfnawur.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2icsqgecn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2opdgvbtb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2umkrlruu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyxttogm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2trxqtnyo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pfvwqwok.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2djheqxyq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vxhsjoaz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ltgjmukl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pbctzkbe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pyuumfbg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nomqiwcp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cezqlrht.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xnlayzgi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2flpuxwlq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kzikyfxt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kzcidpfb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pgwyzxsh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2igjrslfa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2esqxefis.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfxcjmsl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yywtkwha.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lkfuesnc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bqpydiig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2shtcjyfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rehizsss.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zmrcmvei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkvcgprp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2chicqfib.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gyewsaix.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qffjwzcs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mgphmdte.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2htormuwg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nypzopil.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ovnumswo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2lehvyygm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rhsctkga.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2iicrsiln.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ieuxopzl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2evydjlfz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gnscobhe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2akihoeys.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zwpgqhht.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vglevjvt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mnefaxmc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pycpjdwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eozucwjf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbzwkbyr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kstwxzcj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qtdgmktx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2weaotpob.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dxbmdwgn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ppnnrxsn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sadriacx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vyrroiyf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzdzgdbv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bptmottj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sxowbwaj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bvluunlu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yaoqkpan.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbwwopfu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bemfopdt.html


<!-- 参考信息 -->