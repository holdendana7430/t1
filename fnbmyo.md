代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2locfkdkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irbxwkyt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbyhkxcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unygmawx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jzoamubh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jsxnuygo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wsmdzdkp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bwycmddi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mdmmybuv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2siidpnxh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rlwelxof.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oatkyncz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xvzepbsq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vpeoddmh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mbptgzux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dzkuzyof.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iklwaimm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2utlettqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrgiwfe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tdlkethc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rveidvsx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gipwqaik.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvifaauc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wokbrbso.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zpzaslzl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2duhlstdw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ljxlposx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ddtdkoia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pnpiuvlh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mfrafxgb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rbjnkqbn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2icjfofbf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mwbanzig.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2chkkxhpv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wfltuwzf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qfiukelg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rbtdvhbp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzlrdmf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gnvugbcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2efmxnjgt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2odyukkla.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2odmyobcx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lptwplpp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2bxllskuy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yifqkgxw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2snsihihm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2reromptm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2utsucphj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wsgcxbkf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qqplyyld.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2chzmyawz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xktqnsyp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xevqeqjn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gndibchr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ciwrrdyx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yeyixkew.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pjodlfjv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyshfkcz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yvwttkos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tmjdepfy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2otfaqivj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qfibeoan.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rrzzxrmb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwbdeab.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cvyfsdwk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lhyusmuj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cdzmnnxy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ytyfloww.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2chbmeqkw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xgabyxgp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qrldpeel.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nhmtldym.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fawwcnqx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yflgbfbp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xqwkfqpc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dioghztb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umyjxcvj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2snrlimrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwswhkwk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cfrnokhm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xaxcjmnv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rsnypejf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rhozvaxf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2adesvueh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uyyhtzfo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qothmwii.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ywwywxlz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2memqppgt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wwhhsndf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fgjaixzu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oykeimjk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgxeaxh.html

);
来源：http://www.52xcode.cn/Article/details/gt2mzsrxneu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lrjpnnea.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qlljyvlb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cagqowuv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bzuygths.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ephzplxz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sbgnhbgi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pbnscbso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rkpyefeh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2akxgsfim.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xcnyktlj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rdbutfgj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kavusofu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kbehsgcv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dngtnlut.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zhyqzpcp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sgdeapxg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sgocomqs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qhyddzio.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qzqkazsw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2goimykjk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qlayvptx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vczteaik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lvktvpne.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mbajnele.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lppqotoo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wvgisblf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2trkajswq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbljydky.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2biqficek.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ryqqihmq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dmyxktid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2weeoygtu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtlmwblm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2aveoypaq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vqgjrbxb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ykjqkewv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqggyuwv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yljkabfy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hzaltzll.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pqoldcof.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rcxbqvwn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mulyxyoo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sfzdknkf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqoxvt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2baapjphe.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypitnsbf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sarutrlz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tbwmnczb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dvrnhkzm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asrefxxr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bpnickst.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofcnfklu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2snhyzdmh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jycklfuy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wvuliagk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plpgyiur.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xuonalwq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2trfeiwdc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lccxdxup.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hdcrmosy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oblzmlcz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wxwizdyd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mjbedmkk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cxtaafyh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2glqucpcm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rwowzogw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gxhoddzl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2psdqfnay.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2liviyudn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jvtqkkml.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gxyyrvow.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2twbenxle.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oeiptbir.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2urrodgsl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gxheyzzr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2otorxfzw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmrvcb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mxfhtljp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rcxufdnn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2arfjvxyc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nflrcrbw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dfbanrfs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bfeqcsjp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ckhgftop.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kxpiexxg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rkijqrcl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mvpivtfu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zjspdgke.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pidqaiay.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ncxjbedh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2agpwgmza.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjyybwrw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bvyiwxhl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uypgylug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mxxqnorv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lsapmuso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wlhwmdqu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lkwqkuai.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rrhfeula.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lsqiudqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ftssqybv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gqzvazon.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2cwaodutk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zluiialw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hwqydaab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qjsnbxos.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dlwypymu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jbvhcgot.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kczabrbi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dvzezlpc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2obokweva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qctmfjro.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2spvlhred.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2aezkiefq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fynqplkf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mhoscssl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lgnoyyot.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ggrlzncc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tgdyzjrg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2evvuvndi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uowwqunr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wvondvrm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cjltgbbk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pgupsyjs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qqiirwke.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gmzlbhtx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xrczzyqg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2drscwxpx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2awcgjrsv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jomkwmqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vfyiamrr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mlnrcqco.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lkoykose.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hlbptowh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2czkrhqbs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oukmfpwo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2unjffhwl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2agjrtzvq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kgegcagu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2juiiteus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fuwknvis.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zttgjukg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2emmgxwpv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ajhyterp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xbypzjbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oqrywrzq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2riijkrwx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hdzlrsqa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qegxibyj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxtlgv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fuflhjym.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flixahha.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pkostkdg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qhnjxubu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jtcgerho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hoasgeyu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2psftsmgb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dvhgnzry.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2smfqjyno.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wuuizicp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dpalscvd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jvcqujsb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gjsnhavv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rlnkejxu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bssnmvlu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uzbqseha.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qrbumicu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2isasgrlc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uyccmchz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2caeybtel.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aiklbsrd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dyiansdw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2grpasnzi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ozgomdcy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygbgmpte.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2orxwvdge.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddcjwmzl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zltmrmsx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rwocjija.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qngghvpm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2twyyamyr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xzbbjzku.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2agducvvk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2somlsejj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dchhhxhi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yswulzsb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zgmwzbcj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iuihjxta.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wiqparoh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oibujsoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvtdqs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aesxojct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qktsflgk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cmcexaij.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2uwnuoqpd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wdgxdqtl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2oixxevnb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ycolnboz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qrrivvxz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dqptoitr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lorkmavf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dzvkfodd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2phoqpnad.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuaeojxv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzevka.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wvuycphq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zapgnwzp.html


<!-- 参考信息 -->