代发 wailian999

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gmhchyfmm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gczxlontt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gzwxxdhro.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gywwzjzxp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gaycmpdbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gxutqtwif.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gyufspylk.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gtotpuhmx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gnkrfpwss.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gmhqrukgm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gzdzzhhwy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gcgcxaqqc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/giglblerm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/guszwjnox.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/giqwxyghi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gpcwkcfih.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gttrsavql.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gapldxuxw.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gquivaisr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gycvvvjjp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gbechwunu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gbarjrspo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gvjtzceir.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gftgiqncz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gbfrxewho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gunvecwwl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ggshnpbzj.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gfckbxdzg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gfgusllht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzvwnlzfa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/giusauykk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gyalswerv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gaevniuwt.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/galhprhos.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gwyuuqhhh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gebbrayui.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gqixxszfu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gzsqkdepg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/glzlwnysv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gdrnggsro.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/garimtbec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gtseswbel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbaeegkpy.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gygvsontm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gkwusbryf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/glsaoakmv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/geuxsnhtt.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gefpobxpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/glfwjbffo.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gxmfvmxjt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/glubykoci.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gsadzplcj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gcbjfvfwx.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gpoaezlif.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gjrmbbwei.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gpjpdmbpf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gizduzyrp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/giiclwlej.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gniwkzgff.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/goapsdtda.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gyvemkctu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gzynntxcg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gdvmusugn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gdcvdrrhy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gcyjtzbxj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gbmhyychi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gqcuvhhei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gpxgvdaii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gmyobatag.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/grotrjrsl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gmhavredc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gliayvdyv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gshjzbswy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/godfxbfmz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsqmutwvm.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gpbvmxsjv.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/glbgbfsna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gcdskuajd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gqbhwqfuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/ghilbmlws.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gucsozgno.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gqwhiqouq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gjdlutpxn.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gldabpmmb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gnyjguycl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gqhqzspta.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gpdezvhwe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gmgadymvo.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gtjwqnone.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gnurhrzda.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gkoxfyoph.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gcucahmny.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gxlwcfgcu.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gxlmtbpyq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/glapjwzzz.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gfznfjhrc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gbqrqfugm.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/ghrsgrmbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtrejekyo.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gdbtmcaeb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/glliiaidi.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/goeohhagg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gzhvafcrw.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gldorihfj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gqzqeipmq.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gchbencis.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gyhameguf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/glgyzijxw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gvexcydhi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gsfmfionm.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gvfdgrmia.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmlcohfiy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gnqgdszpg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gfdwgqbjd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ggnqphscl.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gvrbskiei.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/giqxnmpye.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gocxdwycp.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/grltbdywh.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gvekoqxuw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gioghrftg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/ggwlqppwn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gyqbskapd.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gotpjbpez.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/govbcslyk.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/glagbnehx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gpenwzjtq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gygqrxjlv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gyqbkllvg.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/geirzqdyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gurkjxkgw.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/grhbnqhhp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gbaagbybb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/guptpcznd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggyicokvq.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gqajgzlbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gavkimdib.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gorwozprf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpvqotzhr.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gzjmlfgms.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gleluvvpi.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/ghpcfvwem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gllgltfwv.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gatuweiwd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpcpptbci.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gljbjucpj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/goxwwcsfv.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gdniyrbnr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gawkvcgdh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdgqxteyz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdsdlzonh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gxlmldowt.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gccgogbbv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gxnobvdov.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gmzeasdom.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gpvxhddcu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gbbtmtqjr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/glgdmrkdj.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gihwgpgit.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzkxagibe.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gsigccvnl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvdnukvrh.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gbvmcwgum.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gdovuzdbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gcegsmnyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gpklxeggg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxfoctlbe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gyrnexupj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gprmfocaq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/giaraxxsv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gqsnrpiwn.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gyauxkxrc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gmvchbdwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gonbxqeqv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gmshihrsm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/ggwxtdpgt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gvsswspyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gkxcbwlff.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gnerdsgco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwduxdpms.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gypitokxv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gllcnfpqt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gsebdghgx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gqovbektm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gbzydeemb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjgsrbxfq.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gtxboqzhd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gaafbydzv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/googclcac.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gpngvmzdy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gsxlupsjd.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/ghcvoacsl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gnoptqkie.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gxweuwodt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gasuvzcel.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gdykqdvcc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gtjmvwapy.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/grhxdejtq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gwdqqywut.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gecqgnvbo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gtchveglr.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/goydndtzv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gdqjyxtms.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gsruxavzn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gjfzbdedv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gdnyuljei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gtbqdjata.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gxvrzouhd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gblszqrqj.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/ghvaschxp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqdhyaqbx.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/geylnsugh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtcjfwpij.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gmkacfofv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gomixcbws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbxeodwbp.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gmzozxvnc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpynwygdc.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gvmelcpbp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gudqvzbcz.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gakhfaxif.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gbrdxfkrd.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/guezgnpwf.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ghakrehxd.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gtwkwexuq.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gmqnyhdhm.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gfddbzmpv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gzjhzkzar.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/guzuxladg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gkpupjyqi.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/glrjmaulw.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gqsmdutfp.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gnalnxzjh.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/ggeacbrao.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gimfisvyn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gvxrxilit.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gfuaeblmj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gzkheycnn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/grvyeidhd.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gpyprjgfr.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnvmazxmv.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gwxkhzilk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gefypwbua.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gcecmvypj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gfqnzievq.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggprsewpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqolfmwcc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gjyarfnoi.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gemoueapg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gcbvuocid.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gtfncukbc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtceioxix.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gyiarkobs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gszowvnru.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gesqfgyyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gjfobpxmo.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/glarsscwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghwfkjbvv.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gvmlcmuts.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gpqveezru.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gwvwgofiz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyajxgiho.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gdvslifyy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggzclavuw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gilbugafb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gedogahqd.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gsrajlgdy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/guffvpmko.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gzezuumcv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gnvdkzhgy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gfcfngihb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gjzbhakge.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gowjohanh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gvplzpfmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdsypawxx.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gqiksceqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gczlozgdi.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gtewaooor.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gdjjubdzh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grzluffcp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ggitneysi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjuhdrwpj.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ggntaanek.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/glouwzfik.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gxmtlzytl.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gyimodeho.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gvjoazqel.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gswekigkh.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gpvqrwbut.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gwuembuva.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gxlwcsoii.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/grryhvajf.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwneszbdc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/grgekptwz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/guqnejjzx.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gsqkbhwyi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gxzsvsxfw.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gqpsmluho.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gxhwrxwbw.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gedrxnmox.sHtML


<!-- 参考信息 -->