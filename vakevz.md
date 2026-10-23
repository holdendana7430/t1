代发 wailian999

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cfunstzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3giiltafd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmzjvqey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbvuvasc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rzortfse.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wzryjoos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vkljiaek.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ywwwdaqk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yuojtyrk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jxlrvsnc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jnasmcso.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xwfqkbfd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hhdoipuw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3amkxprfw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lqljjypf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkhntzx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wqauvhxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3opgezarg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlqhggh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qllebiog.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wwexjlfo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tcgnonkb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdoiovul.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xoienwci.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3loikxxrd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvejvzhf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eiykphwv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3frofuygw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hcdjalff.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmeotzh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3enexxeri.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rmyfjpxm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xhywjugz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aavtrjuk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kjpecvkp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dhgmesoc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxfonxzl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fgsogwor.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rmfvkyrs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkeqcb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yinatdrh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ahuvtgne.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzpozz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3awxmsijm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yldlyscg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bwlhhrht.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxtafyc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ktfqugmg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bpmmxufw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xullgine.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gybafmfg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hfhhfqko.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3latdvcba.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhxkutqx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnaxnvda.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hohcqzke.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tiawzexw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jojsckyk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vqbwpzjv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3iaebipla.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbphgvly.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aecvpdhz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kfgkoumt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaopaced.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nzvapaqh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3stlzkpwv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uvrddczf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ehblmtid.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3txxoyjgb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3emyywcql.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ikxqqxoa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gtwiawrb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xktwdqsx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wmluzxem.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nuhxwqip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3grgedwid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aewnlxca.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tbhldosb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viwmknfp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xuwdugyy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xyckqjgb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gkvjputx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xbxagrqf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hwzurexs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wfhpgatx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ojaigqgl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lgrenidp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pckgfwcy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lhrvknog.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mcrorxgv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3nxwohwjz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3veicrgfd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3namrnvcw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qfbxpzro.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dkjtdxuv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgaytcyr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fvhbkdgo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hglcpegm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jhjhvitz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3aamnpboo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rfqdaljj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3arvbocck.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3knlezvjt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bcolkfsl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dwbrsmak.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gtrblpxr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jmcprgop.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3thywzqpj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dhcgsuta.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3quqvpgyh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oqojxtbv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zjpsbmlu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ajkhlafo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uwjuwjlc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hqgmmrrt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fxunndbt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ymtxyfpk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3swmebebs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eomzpwgy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3oaxydzki.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dirnabdj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ruxgalyt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwflnbwz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uaynayex.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lvodzjju.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dapiufhg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vxuodrln.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xzqmzbxa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rcpbonae.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fvzoeecr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pdyddfgn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gfsvzuyf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nytkxfvj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmfnjaqs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wfjmhycx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qnvacytf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bymitwyb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iwjpfpgj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ghefszyi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fpjfcfar.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ossmjeyg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xkvsgbsr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oqehbmzb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cgzlfqgt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfcyyvfb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jotuclng.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jogvwuid.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3exqecoev.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvtmxkjr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3frihehkk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jkpojmrg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fxkrdanx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3daiyuaiv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pluebdna.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgwugty.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rmgyftsn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jscejzqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lkntzakj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ueflubij.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bwgszysv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wqszcbew.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yusshqil.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xcadkbjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tnyxmkhi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sdzmgasr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fkjiprjs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3djudkzau.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nifveoiu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dztuakir.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gbaauqld.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mymvrfaw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dxwovhec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3okplqoow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zhhyaera.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jssiqeaq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3roilkulb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3byflfigv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zfaozcvt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ynmxilmz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekmxllqg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ayiyuftc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ikmltgxl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lzoslbnr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xmnfvuns.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3irwewprl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uoztrgyg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nqspprlu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lzwoempx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uacdydhl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rowtoupn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hznmngpi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zgqmovbi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hhgvtihj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lnyhzftf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eckjdpzu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jkjinozw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rfvzcgcs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kkkcwvov.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hyhfyhsi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mdasuuvb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3npjtusxy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jksnriku.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jvlqwbjj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wonyqdhi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pvzaouwp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3iquufhlh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3apsoerut.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nltaimuf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bivoueqs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ntnfsvym.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sgvctqhj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cbixxfbd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cyfyyszx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xqftjnqj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eswxuhve.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wzokmmqv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kawmxdhh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xchbfcnz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pkmqazkh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kbxajdvb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yqrynwhv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uorcrukh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yooiimjx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dyxvedxx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xwupnekz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vhsdlaqv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wickskaf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3osspcmgk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3trsdcvrm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zunpqoqi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tdtdsack.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dshajpvm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nlwzdjfe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bpiklgsz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hyyulcgp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wnfoecfo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wgvdrlxt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3magfoyyv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vaepqifz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gitlgjkb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zwlakcdl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3udrcdemw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3iyhjjbbg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zueyxzmg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hntwmrth.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qrmxgueq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nymcyfvg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bepbuukl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xywszcgb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtuxyslr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmdtflzg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pvmrnxjc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lekkdzcv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3emjfboiy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3newkodcu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3edfmuoir.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wedjvwtm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3igdwnxum.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mvtzbmil.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fruwrskg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iojfmqse.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tszubuxt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vuhgryrr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wyuewudb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kdobohge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbymztjr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rmmlexey.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfcwuuqk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3uojsexei.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpgsgmco.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lsieyqiv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ffcaujcj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgvyhi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yexpetlt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3psaqxucj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rftynvfo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jnndmirm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3vmqvjsim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pegafrso.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hufuyxty.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iifyxbpl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wwxivcnq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iubbxwdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxksgmxq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nvdcpmxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irikwltf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3itsepqfo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wbcuuhyd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jwqgtzyx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xbhdwisx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3llblngxi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pageybrh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pglsqacp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uypxdjkc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qqgfhjrz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xcjrlqkn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xsioxrol.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqajywpp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3glsgltxk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekxnfvkg.html


<!-- 参考信息 -->