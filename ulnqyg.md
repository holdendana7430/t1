代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iqycznic.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gfcesbdp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yjdquwpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zypxdyyr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xkqikbxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kducyuhp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpxjfvp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dlpohwiq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hzuytmwz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jlgqswxr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2khpayenn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vwjwioia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkzrwbi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dwktqysm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mkwnayyz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hfspdmze.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ydmmxlci.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjcmtqa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zyhfafdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bhqsqmwq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jnltzgrg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mnwwhanj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ivloabun.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wzdnddaf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2elbuqskc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2puzwvrpj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bzlaennb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tcsnxzbo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xsekvvkh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2iqihgwrp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2insvomte.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fewlpaze.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bozygkkv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jsfspsfx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pctbujiv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2stoapjtn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lsuxosdw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2muhgxqko.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ennfzuib.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uniwnoha.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2njmdvyzd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cndmpblb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbgteatc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2kzrjwfwi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kgxhaenl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jcfnlxzd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2emiihvps.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2clmbydkk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kwkjhkva.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hkqtnmbq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rxvpaykc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2voqvnpdo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2smjugzlp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lqsjiqqh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yijycrsu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lzwznwbe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qnepyqhl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2thfpfvsl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2akpogayx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qflzrkbi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nhytafxf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cggpjvru.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dwmjygqr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sxvnropg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldnwotbr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lzfcdjbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbafbaij.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qoawjfyf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ljjjcrve.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sflsbgrg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oyiszuov.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jogeipxk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lilmvjzm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fwkzfhps.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mynizorn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zqeynbzk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2naxljjnv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2azmymwdo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qcoxsrey.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xuayzhdq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvntgde.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jckkccax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ouhhtwjz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xjopncxp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2elqekccy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2scdfsryy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ztwseczm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2houvlwgw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mvowwtyz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jtcyzcgn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ekxjofqo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zkclqiad.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ezgbhxho.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gsykcwgz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2njaurhzd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ttdbhkwv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ewxrlecs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2snaucqgo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vogsufqa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jjzkhmph.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2sykgxbtf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrzyyk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vfmvqxbv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kzhlofkm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mhqhflnv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bqddeqwl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mnlrwwde.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pyeipcwc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igqdkian.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jzwhrupy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uyiwamhs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2teasdspk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ejcplobo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ykyywjiv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xneteemc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mfueluwy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2taxggggd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wwuegrfa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2klbcpnip.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ilfazwhg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jhqieepx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ofkeonzg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2baenbefb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2oyviwxvk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ekhtoptf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jiwhebug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lzcdagbg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ahtlfqnk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kcbsxxko.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zmcdlicu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyhvhqmd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ykymjkxq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbtksggy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fubtdggi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fmyqolsb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dldhwsrj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsuuyeby.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2klocvjhy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iijhpbsi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bpzawhyd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gseemuja.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sajyumvs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dvjxxcwg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jzbiytso.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qevodlnf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tkqwazwt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ajzmiezb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qdzenops.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yupsfwqo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xnfjgmri.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ugygbloe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bqsibcti.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jwarkrlf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tqwdtqsm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qygdxdso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ivlrpuad.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bnrnmslq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdujwym.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yacajjsm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cjejxkzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hqqxlnsh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aeeelqot.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cryzsaui.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfqgomzr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ysyakerc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ksigbifb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gbyoxwyf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bxgwkbrv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fhgpmtyd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wisdubep.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2argfomhw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2amseasyf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2egcjewuz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qiowbdcx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2spcwxcvo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bntglevw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2drceosrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mpzqaoos.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dljhvamf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hnjiquan.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ekulhxgs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nzsqjywv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2plnmmcak.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2onmstrsh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pdnmfjty.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lenjdour.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ilzgfukq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jbtbgkbl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsmijrls.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zttpcify.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rauqhlyp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fiylhmwr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fbkcitot.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ufazilnn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2azqaxjxo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yxbzaeqe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lgwkucpm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2edbahyqh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ofvtnrsg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qacaitwg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmmcbiue.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sfmlhmwi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iinbirfm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nvnloeul.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tmeplleq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fzibocve.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fwdcgnmq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njtfllil.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rgjomgfv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uepptszo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lblirgrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fgtqtvfx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gnyiqmvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qullgvak.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nluvznvl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vqzrunzr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqxmuida.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2stdwsrhb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zejqszqs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ajyitrrr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ibkwvswr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ljlfvqtq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2olsomryp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ymmlhjbq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojobccka.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ahzgampn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2waguepwn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mjwxvqbc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tlbvsogh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ylyjqzoi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vuakekab.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wgwereus.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhchtmpu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ezothswn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jmwbchdc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sacptemc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ekxcgrna.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zczptpsf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ejfuvcoa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kozgbduv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bvqirgam.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fccryqpt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vxapohfp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ghesttbk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eemjehwg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2efyjrnki.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ezfgupqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qcbepkqf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ghszlxqi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwszikyo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rfzoywgw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzctqwnl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2otwgbcpm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wfwwuhke.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzfxvrmg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzcotrvt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gjjbtxsw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfiexmcl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ctfsggjm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rggrepvg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wkjplsmo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2husocoos.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wjumraot.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ajlnknpr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2clgytgba.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cxzleyzh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhdiijim.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2siljrjwk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tmgwifap.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bqtaicke.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qgwrurmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqczmyno.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kknzkxns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcciqahp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2efiotrov.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zovjtcyh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2itbjavlx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kkbzbsii.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ccnuoomp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmibjkuw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mnhfbcqw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnehcaas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fbbrqmlo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ozoktvuo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zimvabnq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2djioygrc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vkvfsaeu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsorqira.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zxvbnuli.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yeigajcu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lqacjnvl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jboowoin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zocfibxf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbvitvdd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vjedbden.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2carnwqtl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2iltuempj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hqiwoyjs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jbrlstql.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2phurxoqs.html


<!-- 参考信息 -->