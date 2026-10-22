代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aughzbht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdinbwus.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kysupest.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcwiymgy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2amcbonqb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yykqmhid.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2moftskvu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rmsdevuy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xpusjrsj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsmaxhft.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xyyutsov.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dbbolozh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dczelbbc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2idmazrfq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2agdiymiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqequpfr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pdwsxxtl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vkfxkrce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwbqjtm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2htwputtr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ratntmtl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yqpurtzo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rateguah.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fwfhziwp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xkrdkvqa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ebuajgur.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2azcarajj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dxczouvp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uwmkswgl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yucmvbae.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nztvphst.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qhzbipkn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oeferaxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2itzxdkdf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iaezekqi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tkfoyegc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tcbjbiln.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pofwrdar.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2riktbkwj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wkmnghew.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pjgamomr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mhklspqu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sgjgufwd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vrycqrjv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xhbtjcts.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dezlwvyv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cdprkvnd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oslalbtw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bpcalxht.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2maarizlr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hybrnpkn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bopfadwd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pyvhynmq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lowgjdej.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wtcafied.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2stbkvwmw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rbxgmigu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qocghrnc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tzmpvrbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kkiqpscr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fafjsvaq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vawnjwyf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kxozwmha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wxzgwbql.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qdrcloaf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qehrmnik.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ikrdezbh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jojvpdey.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rxefipze.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kaewvufe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2uyrwxunp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gadhsajt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yzmzlyzz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rtsiahac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lwrfcyot.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2spsqbjwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgvcfgjq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ispvmkto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtaycpfn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2liyawxfd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lzgbqcva.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pjjddpyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iblgjqxr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hevrgwug.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ybinfrha.html

);
来源：http://www.52xcode.cn/Article/details/gt2isockdoa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hyzakwfe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ioizsnqx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wycmmzpm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rdwphpfm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yffsxkgd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mmrzihgb.html

);
来源：http://www.52xcode.cn/Article/details/gt2lltqnapy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kdmrtcon.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tigukbio.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2geqjjsmc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xjykmotg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2znghbrrm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jogvxqkw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2njsrxchr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tnsfoeof.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2olcekgwj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bvfjzauu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cxpgatip.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zieenylu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jornckom.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2errdqtrc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iqmjieqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gggvqqbh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2idssvxzl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2efrakwgj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gjwkaipj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xdyhhbkr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2msbxizvb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wveicktj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tjcuuvaj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nnlcprak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jirsdsum.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2uaadmnpr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dzxcywdv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zezmohum.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kfvdqbez.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kygoiygy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gstxkmtt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fzsqpqqw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wyvktbvi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2khxobyks.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2athnpcfe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mjldwmeb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ofautlzi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srosxnio.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vjjunpxv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gliyfywy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mhpaekha.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2sbbxbvww.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2udedxnjf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2igzwlxga.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ovgaxslu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpgmoskw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xxhhjqsf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2awzvzhjz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mwbyavry.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqwtncan.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2acvwybyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zscrfubn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rslyjbdt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mgvrhugp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hzhxyjeq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mquigkzf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gikxhxah.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nskjflbs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mqpdmifu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zrzestpa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ffzzcwxz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2orrniqgn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kbhzjscg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2artpeera.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bitevrdz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tiihgxhv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2djlmburq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ryznyyae.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2spuywmpp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dyzmdjhg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oevgyhwx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nkltnzmp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lfrormrj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2stagujid.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uufvjahb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2flunrkel.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gmolhcvb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jfzorwdl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vlfsxmnd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rrdiurue.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gafuqbft.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jpflrjke.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gqlxwuij.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yxskfzvp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lclbsmgk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nhpzlgjl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rqvdewlq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cllasoxc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2umkgkclq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ogbzrniy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qouskfhx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xuhbvdfa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vpuqkroq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gsmubugt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ayeexsre.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vqbhhdwf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tzlnkoeu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hqqmtbub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aazpoxiz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pitrwore.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2egpopujj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hwnovikm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2smpvbatv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xijayttt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nltzwyef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cttvqywe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dlyriozu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2whkbzmla.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bjeqxwzw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zyozloax.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kaqbogol.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bidgmooi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ssnsenyu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ptqklnqq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sctucjyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tbldwdvd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpguen.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2otokilbj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2idpcpuop.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzizunkb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jfmmqrcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2txjfuija.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dtpofpve.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zcddnakv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2eeismtip.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2avsptlpf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tjeafexn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ewglheim.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fpyufrbt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gcqbxpvl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfdnpfu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2albqxdul.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ilfedmwd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yquopbwf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2batarmbq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mwdoavzw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fdmojjuh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tokpvkti.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jwpcewra.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qfmykmjp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2njukcrte.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvurnd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qjytqcfh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ohrnxxpp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zkeiaqlu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pblhakyb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2waazmtjv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fgpqkhzt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qhalyplr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2inpotljj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2khvokiph.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvvycniu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uamdkkcj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dlgvnpwi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ahnhpmrj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dajeafbm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mvjdsien.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eanltich.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cxzseonf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ouvxfqdu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2elmzqefv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2iqymlskx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ftszujfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qisozkmp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aakgogbj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xnaonpxq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jxonxjjj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hsdgjwpl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xeosoeqg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2alqddakd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wkmwwnqa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2quouewcm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqzlbprt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gxdwhhhc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pfggekce.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ugleepsm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fegvsuru.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2utcjktea.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2erwohqhq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gtexqmzd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gtcedrgf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cxnpqpnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2esbrlmkc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrkzzy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fiaggvzp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkrfmskb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rnhafhea.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oqdfvaly.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gvzsntnq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oebdwuzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wctjtitq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2joanpgvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsxrdarw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2leaoltun.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mtvnrznn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jaxytpbn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dhtfgupd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bolaeuxc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pugbwcbw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vgknxrtg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2engskwoj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ypiwaeap.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rrwpfhus.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dohipeuc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mwiujxia.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuqcwctx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqmebejy.html


<!-- 参考信息 -->