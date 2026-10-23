代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3utqhhhtp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3urkcwyyq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3evfdnyvb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxsunb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dpuupsrt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bchklrfy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pppcgthg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bdbgdtgi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oktbaknc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3autwdhrk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yjuglxeb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3welsfhuq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3japhomca.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3keikrbwn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3diafsdhq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lxbxrxee.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nymfblex.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sjpyjlyx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhulddph.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dviisrag.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fvsshjas.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfxflcgv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewjbaihc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3onrddqik.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vgcxdzvz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3feuxjdya.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lusoucbo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uyyvakcz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zlwkjsvw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qlaezbos.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xauwfrqb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rnagkcva.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mhngcqbx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uekixocp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3irscjkfy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3datyhqdp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hejojfqv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3abvpcqai.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3exadrcwi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ljbiygsa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yblvwtef.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zkvlcvzc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fotjjzfh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bmmvpfnp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gaqevtvd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3drhkgtny.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3crcghgle.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjgductw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gbinnlsk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3msqcyoqg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtpkoisy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ybxhbsdv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3igutzvwg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gwkywnxa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3azgjwzkl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lvhuzcjz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ieifzdie.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aigkidyk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3verptydz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpkyfao.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3goqesqiz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dqetsyjd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zggkxiey.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gvcbhzno.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3svarzuwo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lggsdbxr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ehwczqzs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzhnmckg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rrlewxsz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ahmhkxaa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qibdeznk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pyiefpau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmujocdt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tpquwbkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnbqphoc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uomkpnoa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hbzunxnf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rmiyqxhl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zzopqviq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3urcdfovj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3grvskfuw.html

);
来源：http://www.52xcode.cn/Article/details/gt3lmmbqufo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3outctnbf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dzkqhsdf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rhnrxbut.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3afdahwze.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gsmjuctg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyphhfr.html

);
来源：http://www.52xcode.cn/Article/details/gt3rmlckvsb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3htvhsmwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zdosnthb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pezgnzds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yjnswfcs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kjpzzjly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pwaxnxva.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vyfvrnoa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qihnrnbp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oyxsyvid.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pllcdtwd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ystoyjuf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sgynkuax.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hbdwhyou.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3souqzvdc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sdthsweb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ugjhlonz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qgsavqax.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ltlgfwyy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ykxakfzy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wxhbyooc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yzttzotb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lrsblxjw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jaqumoxa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gffjuzns.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bpohsmne.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3amfgaezq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vjjorwci.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvalnguc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3meszpmoa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qzhdjhgk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tkqbjlal.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cmgomarg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3exqnisln.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jlmeznan.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3aracrsvd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3yncsyrfp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uulcinmy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pxopfskh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qvfnbtju.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vdbakpem.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3woofluky.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wdrtlfza.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3yjgxokct.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3quoruewo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kradhnmu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxvmtntn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dlnaaeji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tsofvgaa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qzlpsraj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdtluhts.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wwsbzphs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfsmxvxt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3muecumag.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qmtrwldz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kzdbwgyg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhuqxbov.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qfzubexf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bhshkjus.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wltgfwkc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xitlcoke.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qkoccraf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hkxrfcru.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ygzulkuy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xhewdtrm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3inquanuj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lxrsguau.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iamdagfd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aumwhlot.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wctzxotm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mzvkmqaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zldpiogv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vyceqvdr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jltzetxd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qjsnjysn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vdnjqwnf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3yzjmdhru.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hofuburq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fjkpmjkc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zjgtutrg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gziccquc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cvazknne.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3onseljfd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zsoyngar.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3guhboyby.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3veghimid.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3whenbtxm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3moaxpvov.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3npungkvf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3yiaqdwgi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vdwttktw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dsuznwiq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3htyvvgbg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3glymdioh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3usaluftq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sneykkcw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qbnxislt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vtxotlab.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zxnvqlbv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3prabaaip.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwftxi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lijcnkex.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ansiohsb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vslbuxpi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kddxqwwu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rbttstqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jequtarc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3izrffisj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydrpdsjp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cqzxudtt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3aahtagli.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ffvfbhrc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tryiwdpt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rtynypek.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3loboicxi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ocqrlcam.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3owoozcdl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uhpinnpf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wcxgdmlx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3oawcaoai.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3naddwuwb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cwqwocmt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hieyoevi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3npedqvgi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vgsfstjn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uvafupys.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pewbxcmm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jjeeblli.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pjlvtsba.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dvpwquon.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zymnfuyo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iwfypklr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uotpfjvh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hfljpxlp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3acqddbwa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fhzvcnxh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fajbesuo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jbyibaia.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sajikpcu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3esbfvwpm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mararnie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gwtlguxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kemzcway.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yztxamss.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ipzcalga.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3chbutwid.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qbkzfeky.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jocrfxne.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uwizxmra.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qhcwnuql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wbxwfmnz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3iwpvjqjv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kecmmvhf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vkyuouin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qyjlrxlf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dxjuyozi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aewkblwp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mbsjtpyq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yapdeawt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ndwqupmd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wmbkvdgu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cddbalgl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wrapmzdc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ydqsvpeb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nvqgurzt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dfkjkomx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ogjztbcx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kurpaldm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tgjgaeyl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jilglkhw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lebtyqbc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dthujqhm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ababfsce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbstqaba.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzlrculb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vipdfcpy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ypphbjcb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsniodoh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3gfjfxbou.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3roxyfrlq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dzcnsjer.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cdaeeblp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gyzsqszp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lclvmbxl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mppuqxii.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gkcabjzf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycodfzdy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qafwvopg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zrvnnbsa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qbevbcqm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hmdqoblp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srescetq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dxrwyicc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmmwkxnp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbvcgv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lqwdetqc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cyflwuds.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ijhgbrnl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3acfhqowj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3znwrcmxp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qwypnbjh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmuoxkms.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eescpows.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tejwolmt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdmxnyev.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3izvatpfq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmfbmyi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gvnhmsdq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hbpbfrlz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtiwfbrp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xrnrwqer.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gempqjiw.html


<!-- 参考信息 -->