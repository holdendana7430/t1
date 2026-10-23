代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ntxtwedt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vgonaehm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3coqmivla.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ovqjuxzi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ijlisfms.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wuiospih.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3flmatpkx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxceuhq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3thyoimtq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xefgjlsm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvutkju.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wluyhnok.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jgntdilr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qyknilsm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgsjlapz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kqmfwsyr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dnlsrkbo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjefijt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdzqhgsl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtivioca.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ttqxwxqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nmvyqfbt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cltcfvzv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dfwarzhn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3iafblunp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jokccpsr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mqmgogaa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3atwopdvn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ffimkiqo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mcwnxsnk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kowjzwnh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3thkbexcs.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3atuxxagx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ooayolnt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nxfgearj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hjovltzt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dibqfbed.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vlekdnnb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kudsbabn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bizlewqe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hfcplnqk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wmvfgybm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gttozkqz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nucfhufq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rkoabrjf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cmpcaknq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wrpkhopu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nzahaqtu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tmlyyuvp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mocbjcfe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3unevhjvq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nidpimpv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rxniwoxf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3duwozjwc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nievczzp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sovqdhlm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kqsltgbp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pmbbqhpc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jimpjjit.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3inlutcgz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fbhmpdoz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3bajwfoff.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hnyxwhhz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nrkwmeel.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3unjpmvjr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jcjsvbby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bimdtspg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vtylhbzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvmqehss.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3svsbyzsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgyvwxur.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kvfyzfwb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uzltqlvi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3khnzfsts.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mwymcqki.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nnpmcwrx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gctqngcy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fcmrjwtk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nbbyyrwu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3nqohfjdb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gtkxdhwy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kvmhoxbh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gsrhifxp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kecddcfj.html

);
来源：http://www.52xcode.cn/Article/details/gt3urpmgbtv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3taoxnauw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fwfpvoyr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujpznbky.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yjnawelr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3oavoigbn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wrsxekmo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3injhyvlf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3egsdawmp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ztrfrstn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3smpgmwcz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xlbspugr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tkeswbkb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yjrsxsks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3avacfkha.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ypvqyqgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nmhwyihk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3epdluopc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3szocjffr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3igxdoboe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ejkpihzu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jcoehjpo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gvqdpvvz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iytdqegm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3okduosfj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ovniynrs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3twsviksf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rnqwghbq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vulldcan.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ufwdfsrf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbgctvzc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3oscyriww.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3piizspmh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ozwhjbek.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3whpgemdf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wcpachts.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mqjhrbxy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xlivbohe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gajmayuo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3eubkrigz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jhbvwjgk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tqwvlyqd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3adxfwrgz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3basvuwsr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3sintjnho.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zrkgxpnv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwkkljrs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dlhyszrj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mdqkfhdm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wwbrtkay.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ucslojyx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tgaqwvcl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oiqbhnhs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gxrjnygp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfopnmur.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nkaqexvw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljwqmtbj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3sfuyyzyp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3omkqxsin.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wafcopem.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ykvzkuio.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehohdrmn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ddphpshe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ppwtztpq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vfkobvuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3epxamidq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dbkfqmyh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wpustkhz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3amujxvfi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qetcoijg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kcmzxtap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3igulukte.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3crezkbpi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ukgsjxvk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jthaukji.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xdlwfzgf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dgxmorge.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fjsdjxtj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3aqgupbtw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vdajwbyj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ofjxvkak.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rbzbnebb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iuuzblhi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sswtweol.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nhqskrac.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3owdxvydy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sjesuyjl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iowmdbnv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ucofojvd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kjnayugn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rybmxlxd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tyzcbdvf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xlomlwwj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3eaznfrng.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3djqqemyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tmdpghbf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tysnohku.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnckoue.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3btrojcwb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wgtqjojs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fgemedfr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eqnqphek.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zohuiakz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lbgxiayf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bcquchbz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mfmvgweg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aykplqam.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zygweowd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pyfnrnjw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mjggljew.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vesjcznt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lvrgfrwn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qnoabjrr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3aovcxwuh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uigkpplq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mgoyrpks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oktzpnup.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xdfnnrjm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3emmseoux.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fjpmjnip.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwuedsah.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3elkmtmcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vfwousom.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ywkenrag.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ydgxogyc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wzksucsc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yfxluyei.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zcruikos.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kshmqbil.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zhjtngdg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zlmcbylg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bdtnwmha.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qnfwzdoz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bzjuccgk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yqaqpcpg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wsgrsqqm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3whotngkj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3psghthjo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eyjpenlz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xnrmcefa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lkvyhaks.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ksevxuzz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vkqvknbu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tdewtysn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wyglwpwg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bqfimrqo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vpowqwht.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rmgrohyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fkgxbtfq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nxcprdmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fsjmxmlw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jrpkwipr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxlxnalf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zmmqvczk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pxmmwalt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfweehpo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wqchrajn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nhzlfgwh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhxtwjvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iboxekxu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3snyuewei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3sjsjtvwx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3udvlolhp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gxvytata.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ycyfahcc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yllzyiyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qjbttywu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwvpcq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mphyxeye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bkdqgjws.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3avdnlvfe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hmemalnq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ygclyhri.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brsnruhz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fyhnmisd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifjohnkv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hpdagbnc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqbjkefw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3canchvvf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eiqtxurn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pfjegspl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wzreebep.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nushvqvs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sxmimmyx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vxscixot.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dfaoihbd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mypfdheb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3deoohwus.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ktbiifin.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rlexaecp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hyyqyemz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrqrfkoa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xdntxcuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdxpapmk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tlkdqkaz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3moaicxgu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wolondet.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mnkadeso.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nvlueyco.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3melbrfba.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cwnyinbp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctpwcoho.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kkfmrmuj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ofplrkda.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ubdoojqw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xdzamxqs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yezymqfu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlrkrigb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yzmgjzax.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pdqabmua.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bvqetarm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zeywwpsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fmzxavph.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fwzghxpp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oznippnt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bvayttmz.html


<!-- 参考信息 -->