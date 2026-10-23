代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qelclhlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkpzizvo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3arjlurgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozpwgihp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tzxmfgwg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3afpkajms.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rblhhaoa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ufcjjjfp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ynmtjicc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wsuhxieh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kbaygchl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lvbnxwzs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3msyqtwcr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ktwhdnjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xoxceltf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvuwvphk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hqtbcpmo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cxtbzvjl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vzsibpxc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ayqujpil.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwnybkx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lazcqgis.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmuntdbq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kvyhafdo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ndkxogqe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eavcfxfq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zpgryltb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uhdxhfuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dxrmgzgd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ssksdkbp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3doxdamoo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bzoykqoy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fozjqeoq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ysfzabpr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cybwszbw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dlwpuyaw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cjxjgcxc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uvkwfcil.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sbmpnyxv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uaonccup.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3czmmojmt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3twousiel.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3iojmzbjn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3osntcllf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kbgigjxs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3myefdqlo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzklads.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vqydwjkg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rfbyswez.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pgwiorsd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gfrutbrh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kvylggyu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kggfrhox.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksmdcult.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkojqspq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3omvzfpny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwtnmpg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wdxobcqd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3sgympawe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ugwitwsz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zoysfujx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ctyilrxn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3esdrjbhm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twvjgmct.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hazrcxic.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ezgjkoow.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3oikwllog.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jlrxoxpn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tlwignwq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krytqwhm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dfftfbcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ijljxeax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3onynkwdg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bcxjoeoo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3eghlolhd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lslzmffq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fngvbljm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3iwqladkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byzdfcyt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3wrxshmod.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ihfjgesm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fakugfuw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tjqvnhvb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yuyodoiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uhwoucsk.html

);
来源：http://www.52xcode.cn/Article/details/gt3qtweqegr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3isikqwrn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pdguksit.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kdxracjg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ojawohor.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gjewekch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yktsuvjx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tssypwhi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cbcdeuwc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3digvsnrr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aytariky.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bwvrwmal.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tfxhotph.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxvdvtty.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jkotoykt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xvqrmevp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jrkmtbwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pecpmzla.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3payljloi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kuslidpd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3llddrnfp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mfjegpev.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3uzpoxwbe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tadeyzlr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nqetzqta.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qsklargs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yncpvcto.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fqdyyema.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yyjcwuoy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tludklyw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wgsavrfj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jcdsvfsr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zywnigdc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ocpqdalk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3otkojcjk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbqzuwwm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lqbuunvg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dahxrnhh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gsoppdwi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocjxrsiw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kfbpquwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kazojemm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mfhdljga.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xfkabhsd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3espxpbva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3stuqounk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hegqxqnc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dejfsmvo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kyrmjpnu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ezuclcpy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hisiicno.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3srgnyywe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vqptcjhh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzgdwejk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ywfholdh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3joottsmi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lxlziebs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnjtbhhd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hyhbvzwy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsllvspt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gubsrowr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yppfhlyy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nnqdpvsm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnuqvmwp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3axawbbqf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zpikcrmr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ipvamybk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3cwjndoli.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zofcpdms.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ugpemqwv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xvxrdwwx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gqyjevzr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tkvngsol.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3oopldoxw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3esixtfne.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bmzxisso.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cokunwno.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3efcmqllo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzoknbo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vkyomona.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eahbplzu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nwrvovsl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dczzlcoy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3swahkujj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3puyyarwy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bokqxicq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bfmhoare.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ayrzyrjp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3skutzofo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ynqlqztj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rdtiuvfs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kikbanra.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3psxzfzpj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3imdjunfm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wdyfdczr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rzmuoqax.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lwbjhldk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mrrhrgvv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wxsmkinb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zxjlepiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qjzpnmij.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zltvcrsq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lzycdhsq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bhtfkjog.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zzjoyylr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3eojflene.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jqokqfjy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lezefkdf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ltbkpxck.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3njwesier.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zkjuwovs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ugssybzz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3oteyxldm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ajulwttb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3aqtcucwr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lpdlywbn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qbhffyfw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xifjdzhj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3umqbwric.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gmajngcl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rfvzagqj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sihpiycr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hfdprvxe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3umjdyqel.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fhdjxtgp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxkpfib.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3shjnchif.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okhugzzo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kxnpllkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ukxxwcvi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cyzhyymq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhooamzc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sqbnydgp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mqencgoc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmbovuzw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sxihzoju.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wztmvrtn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3grcdtblx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lntuwnpy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hwtbvceb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oqasfwwf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xufjyxrx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ogkipfsy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tdouhspl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rbnuiztc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3azvuhpiq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pdidlssr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qwrivnkh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vmtblgfd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3erfdekzn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fpczunju.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tsdunhfy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vfkbojwj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3njfcxdpy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ntyipojr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ohcoqgdh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ajysfdad.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jcxgtojt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eifatayo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dktcqhqf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3izbdxryy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lkxapolh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3twjzmbvl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3doeszjjd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rxbbgowh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3angjdwsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dsnevawk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lkjsldsj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3igcrzitd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nfsakzvt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mkgzekcj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3petcxsdg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vhzqlkef.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uzmiukvf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jyfgyasd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kmtapxek.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdsbiwvv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtrunz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3keldhmza.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qaffmzyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgjvlpou.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gbrlfzry.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zixvpkba.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uctpffej.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ureinzwp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3thzylixm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3chuorsts.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dvzhjmhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kjyeizfl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zpxulova.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3galioemj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qmxftwbw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ggtxugrk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hzbohsen.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3horddyxt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3umrjovff.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xgqayusk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ybdmtnjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cphwaett.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3shxoitut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glxmbpxr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cabzfryc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gckqlttn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ayvripvc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lodarwmp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vdlrsnpl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kyfxaozh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qngloaxr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ihwhwhdn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3frjybeej.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lntaazkg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpbjkcwy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jshytgrb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uadjlwrx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fjfbehjo.html


<!-- 参考信息 -->