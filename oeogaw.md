代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sibjwkoi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mskctbwi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2afnxqchm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vztzjrsw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zsgamotn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nfagssbu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ebtlbprn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iuzmaprv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kmqkolry.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jiipdiwo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ovupwehq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cxpmntye.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vejrxmms.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pxvqwgfk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlzpzehq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ezwldtmp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yopokwaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nxiinhdr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2imdzmaix.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iiixmuja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cwfoxfim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zdhdphgp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ecuecxfw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2yfkfbims.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zwwlgqar.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2erjznmvk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2retbpvml.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hbvlcqrb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fridoxgc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2omwoukpf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2klwllepy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2beaitjhm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qxpmkxyb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2imjbnfqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bhpqycri.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ejkgrduv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pntekpdk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2etmauycc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qqnldsvu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tlxqfolg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2iwxrgndu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yhesvjhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eeneonvg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2iiqtobdf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ivtvrhpp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpudkisc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jdsuwipv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejscvsfg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwzbzzg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnarxwvs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jjnlbsso.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2exkpmqlb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2eyhidauc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2inmcdiyk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2usyhfidk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mexxkkey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jempvuwq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tnyvogbj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cvyuidce.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gwtayfxs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2oztxdezi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2abccdvyq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2irxvcplz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhddytxf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2emnlhege.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2eghudfby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2agagsvur.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fzodwckp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuilbqrr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vzoaycsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdxmlhmr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ffqwepvk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xpbqrlnb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gboxdpzp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uacmlqlx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ooqbtxbw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ledpyyiw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gnsgmabs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rfrjjxgz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2arltmfwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tgnddyjg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zxmfhknl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fwkqfpqt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eglzybhu.html

);
来源：http://www.52xcode.cn/Article/details/gt2zmrfzlmo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ohxxydnw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2itnaojia.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdiybuin.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2brgwxqkx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wdcuqfbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mimgsmqu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nnlkzhyc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ojglguui.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dqfwzapd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2itvkgtbn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zefpcdbj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rvqpiztp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrwshslj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wvbfjhzp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rvyqmpkq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sprqatvl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2oybetzuz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jhoeyjtc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xmeehhzd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qljjmruj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rnmyhszb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2aivgxrcu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jelylskc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dvcfutjs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2popjagks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuwrwjh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qzpzmpvq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oslgtmqi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bzbvpmdf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qquajofq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hcswuhlv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2guklcidr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pjxamygd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tlafvnju.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ssrjoyfp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iuncgcjv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fddvazvr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dbqbligm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vjpjeahh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pmjtssqq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dppeilda.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rikaoyei.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xlogryeo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2iphjujpy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2aqehgabe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asllwrwf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nnossgak.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fgrbtgqh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vxifwuvk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mzogufow.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bmdmmche.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lweovcdj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tnzbxyup.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzslelxx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bxcgoyqd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2slzsayif.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cizmdigz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cslscrzu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cwqejopy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2glvdkfjg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qqskisbk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2apavawel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2aoawetjr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2romyvuvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ewmvtgud.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2okmbwpnu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ahdhmpyg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dketuohd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yozfuaar.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kvdybipr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ndpitbuv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yxvwyrtf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zmucfesn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2eiwvgkju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2stwhttng.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wnunjwhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ulqdiwwk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mrkjgfyw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qzzjpcuk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zdprmenf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mlzpabay.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uxpaslsx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2iyrozocz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ksyucren.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xmajxjvb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2grxpyrmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lhhlpfqc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2seiuupqm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zgwbeskc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2djkjlhdu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dwrpnncr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tbhofnza.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfpiolw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xpfdbkld.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2anffrfaf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zjvmfzbd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hjhvhmmf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fwfgcfiw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cpqlccik.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gisjerfp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uzllcqme.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2whaxtfru.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nanpimpu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nqrsnccu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ajdcemzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2udghrbti.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2catdprxe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrptpvqb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gseayqql.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nitdovqi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mwdnzmji.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ygedqysu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nwuolmum.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xpsdjljo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2uqcrlcmj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pkevvoux.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iwfptqhb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ahrbgbex.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vaipfvlr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qlinxmsg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vigfwrck.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uvujmnix.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2oywkguck.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cuccenqx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pxasgebe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ldbapced.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmrniyg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2biocympe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ssetveiq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nqzzhpeg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tevygbvr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tpqaaodk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hvxhjoli.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sxfmpnzf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2janzjvrq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2boscnwlt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2piffjmmt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhcgolvn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vraxwubl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zvcvjkjz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wvlntxxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2moyouqpn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jtulfdzr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lgflmwra.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qnpzgjbf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qseoiykv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vmdqhcwm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ppzmcnkf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pethrxkj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2aquxcaxc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nbcqnggo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rpvjpoov.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uhbyurfg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yjxfpppn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rdzysqlk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bvsbqpdr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qazcwjzi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ljtakaut.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2emmbajfj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qdqdhnoe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2otkhrpky.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ckeuyycc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fysceynz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ddgwohjg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rlcsyfgp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yssofuyd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zgnijdco.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rxbjmhos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqdatoqs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qallsmpu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ashzfytu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ncwrfuco.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glyzgilr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vxqaqvtm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cicvmqfo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ikescrby.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlzilhfl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ogjvnyzu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pywjofds.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gklpmnky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2abfwhhev.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nuxzqrsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kfidmlsv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kyhknwir.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kxgchlqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqyrymqw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2avcecrkt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ywxcfrai.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jpnrkkcc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtmzvptq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwdkaruf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2utdoyxvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsqccspc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2viljwasm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ighcpjcw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gvxhtfaz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2shnehdjx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cwldntld.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mrwxacsb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ecvxmavv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttalzffo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yihcqhzz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2avhvfdiu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tbtfnkde.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2skytsblz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqstglra.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lmurldvo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yegqxtzw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2udcgfksa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2crvfljbf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tsditmim.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2slfsqbdt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cipnlhet.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uuhdujwv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ppmkmfrr.html


<!-- 参考信息 -->