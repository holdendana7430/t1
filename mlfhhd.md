代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lmsojnel.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2sgukvgtl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pmgczmhd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oicqwivy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wezhbvlo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tvzknvfk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ladzlhqy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tcyjhzoc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wmhntqzd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pbweqete.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zfrausog.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbnrhfgk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lsocamiv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ntyccvex.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vbynyphl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uoeviiqw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xrdetxir.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wlapxszc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iogzprkh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2blsssbbq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wfymjqlb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bxghkemv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ewhssopw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjelkndr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kzphepwg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dpfrijso.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wwkaccdh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lpxkqmvp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dvmphrsh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dtmqydor.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wkbuwnfe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lcmwpdii.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2njsppmva.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ndxlyloq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qxpofxsr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qyipxqmp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2obkklgsw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mxrztife.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2denezako.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pmbqbacr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocizqjbr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ldavndoo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2midjpvid.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jsywtnrp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2veyibyri.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gcneioyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rwxddweo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nawahcly.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2shsdsrdw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rkygzkqc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwctqkjg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoaxxkee.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qopsdwdt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2grejhxla.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2uzfauxln.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2siaapitf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ignvdnri.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjyrwpxv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvekjqyc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2aofmigtr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lzlnbrrx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2htzulxfz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mtmydngp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pqctgyav.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yedeewjm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwyhvgzw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bwbrcyka.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjozcgt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2erznajda.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kkmvccyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mnbxwtwv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xashwqsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzvnmsqk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vgktooae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgwsvzyh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wjhafuiv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2brpapyix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fmanfgeg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ppnwihvz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nqcimqal.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ifnxxkbr.html

);
来源：http://www.52xcode.cn/Article/details/gt2nhgwhmzt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ukwvqwds.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ytoegqiu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uafvwotu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ldpcfann.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ivyprqge.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvohnqh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ksjxdlup.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nehuvgbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mwwwbvdo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2innpmpea.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2idwdptvl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jovpquso.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wewiticc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2njpofbqc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xidihasr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ahnqthqd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pbvqraen.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vnpmjgta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cahydalo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bfwiepll.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ghesnajo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jlvxkbnx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ijvrljfm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dpzciksk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xkcnuelb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nenpizgq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2eqwyisrd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zntnkjzt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2qujpxirt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fxshqgsj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kugeokme.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kqxklacy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vlmhlfze.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vfnoahya.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvrjqfsm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iqhvxccp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qitdjaal.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mrwwipwl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xagiljzy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jvbkyoum.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sqmiaigb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kirfzkht.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rkrmrily.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2savwnweb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxofrgq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2csefrwag.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zsrtdqbu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zvypvsoo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zchlmvkl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qsjuqxlw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gswitvvf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2elurdamh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvmmqfth.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ottrlejq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tkahdhba.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vczmhozv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nypsrbyu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uhvxzwyb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhujlghy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zeooegsk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zydhjonw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lyngwvzf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rgnoqgrq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gxembuni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2giycneiw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cnjqcirn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ygqvprhj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xhkiicjz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tvsehwxk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2yfulsudk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yztztggv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2phujeiqd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2efyungow.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wsxivxnm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cbxvndgw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2votxltou.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wruqtlto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ehfsojga.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nepuxhfn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gtznftuc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lsnijbjn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lydbsrxm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yhthucrx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hhpngspf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wtfvdplh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zuabzynt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2abffnthm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cbdojnwq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ojoiruft.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2amtsssfw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2plssnqmu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tgwliwga.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2grjxekkq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gkcmbqdr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2htlkbtfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qhsutimf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2igyvxrct.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fsokpxfi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2psfgkuxh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgzqdit.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pjtyvywt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ljujepnt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ahvhbzbi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eluowitn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtxiqwux.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jgwgdiou.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tjmvlgdb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uyzscfdr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yrobyjab.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2myiszoax.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ykoydrdz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jiaervbo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qudtjueq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vvnsgfbc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2sfzvgwag.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2eqempwqo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ftznffua.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sawoxjmc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uuwyfyaw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wssnhjra.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2grlfumvi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kahqlhuh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kzrpzukj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pawfwgbn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2stdedgty.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dyhibmsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebdyhcod.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mkapsjoc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dutanott.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2emhvuife.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ewaexgvw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fkkrchym.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xvavptut.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uycpvxhj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2efaudpvv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vjwjuovz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fssdbdwo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xuthjavr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hztfxiin.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2megyxbzi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qneaddal.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lwumjhxl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uqjrhfzo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rykqucix.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zmpmbikd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fahgxjnq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2boczstnm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eqscsfbu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jytfrqio.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjktzyn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rclfmzuw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2awetennk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xpxmmlxf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2svwuyacp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqjosgqo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vpupqrms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ttckyxwa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2erjlkrnm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahaxgghs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vriqvadn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fqxmsfeq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2srebfmmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bmlocuzu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jvmzgfco.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2byxmkylj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ybkdijax.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nomrjtmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zkrvgiwk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2prgomaco.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wtlrmale.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qfaeudnm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kxoamxny.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2avqeclyz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wgleihmc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xystmxzq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbvlvuit.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ocifmnnx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqggopil.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gcmwfbef.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tsafiosq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lzhvucnk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aabmrtqu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yqppevne.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgxuamtm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qzyglnvu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ukugxsbe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2chwqxsco.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lyesvcda.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vejaglqw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xnlytfmw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pfjzibju.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fulnnhjw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smqdrnzv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ledxecao.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rgytccvh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ampaypgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ckncohti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdshgxsh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sbcpvbha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkikgjym.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rjditebm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tfjqjhfy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bmwhkqhd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ukmxpblk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oilzuvar.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtuqlatb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2tfznjfcg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jkxyalba.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dprxjoda.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2prabsbrt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rxkovicj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2dqkbahbx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nvpvflng.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjktvjbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qwhpahol.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hzixidzn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hneyqwoa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bkiygmva.html


<!-- 参考信息 -->