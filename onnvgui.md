代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/giicbzvzx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gvkfclcvh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gqvaigmjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/giyqivrvr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gmpuyjlcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gchucznbd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghlqsstxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gefsqhqsk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gdbjxbqdq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gzsvjgcxg.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gqapvgpxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gyojilpnx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqwrdap.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gqxuaypnt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ghqydcusv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gxosjhgfa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gordmqwwe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gyvfafoli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gjrjixyui.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gheusjuyy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/giygxoath.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gbpvgnzgn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gkwqlfxmb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gmgkgckxh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghgzvcvca.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gxqexkpmy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/greeexuqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gwwvyfqkd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/geobhttds.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/ghaedaeeq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gtoqiacmi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gctnmmcmn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyuivkume.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gehaqdlfv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkiulmfqr.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gnrwuyrnm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gwqvxbmdh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/ggcdumfri.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gubjptjox.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ggwsrqqib.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gkkamkzvl.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/glztdioxk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/geuysvpza.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gsylfkubu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gzrkxumln.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/ggwuflrqb.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gtzgrmpxv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gzqkklgya.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gvillsddu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxgyldonv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gemrqzprw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxnrfhxlj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gtycdvjzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gvpndztvh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gklkbtlcv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gyeqjpipf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gfmautnwe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gfndkunvy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gjowiecaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gibedaxtj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gvwbailkk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gxdlrzjaw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gzfjkllel.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gttunzjqx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyvmxbkzn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/geaoifnrr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmvfghjei.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gdodfzkrw.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gesfagrpl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gliijlopu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gkxwkskgl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gyqomwfmd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gtjtqmkfy.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gsfmumpdo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/ggujnojvc.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/guxmdsool.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gxvtgnora.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guxrqqqud.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gywfvfsga.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gmlzjrszy.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gqtbnynxh.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gqqdhbndr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/ghukcbdpe.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/glnrsiqhe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gmbdevqob.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gjhvmlnfk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gepfyfvqv.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/grembwvvc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/guvmfqpyw.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gsyfbyaml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gzuyuzyes.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/goufroolg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ghjvaaiwo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/glbqxwzdp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gwpbaxwse.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gfrmqqbmx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/giiwcscel.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gjfdksihx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gitqytkla.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gzplveqiy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gtboveebm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gafvevlkl.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gquzqrlov.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gqiqpuanc.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gsafndrom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gqexerpue.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gqrywcmzv.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gfqgmnbwj.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/guqwzetwo.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/ghdpqrpba.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbpyyhcjl.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gtcrvaivn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/guhqzlltl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdxskkvxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gnfphznbk.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gqappinzj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gtkevblbd.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gxizdulyb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gbymleriw.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gghsknhpf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gtigailgb.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gzdrqxkge.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gnrwvaigo.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gucbjxaac.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gkzxbgoln.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/giydydlfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/getzekjcv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gmmvhimir.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gszlsyisk.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/ggbfsocka.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjieiyxpd.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gksjslfdm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtoactapc.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gjnjsycwv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsbhkdvbv.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gfiemuzwv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzgralmpz.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxjoapuuh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gdumzldjj.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gmpykjuzz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gaoctqexy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/grhhzdzlr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfslftqgj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gmgslibro.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gftwcjawp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/guuvqkfcl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/groemgvux.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gxqkclgui.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/glcvtmocu.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcwlnbttj.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gelrglqwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gmnhflkuu.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gdnzfkhgz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gnruaajwc.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/goghgbytm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/ghiyevakw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/glwdoahbp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gnnlwlsmm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gkuhmrshc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gjwxctqcw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/grplmhrch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gzjwdskix.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gqakuejbr.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gtrgwlhsq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gzkstwwpr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gucbhjkwm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gvptwpgrv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gjjpcnayh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gadefvdvu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gpowgrevk.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gtbmydynl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/grfgksdje.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/galsqmfdj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/ghinneqsc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gdeyothon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/glguqfiys.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gwsmpizcx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gsbppondw.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/glwodnxkd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gjyxxrzyf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/geietojhv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gogwtybeo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gfwjiigft.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/galtbudqv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goxzndlqo.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/ggpilpzzp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmqlslfqs.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gnowqbmgn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/guyufbiii.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gzbrbhgid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/grgonuopq.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gyqroqtgg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gppoinbxh.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gknpscews.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gqsulptzw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gvflwzscv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gfsagudbf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gzzaryapy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gvfyjldfd.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/goxpxawdj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/ggogvxruj.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gpguyhzdk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbvmsvijd.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/ghhzpwqcm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqqstorzt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gzwekfbjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gecesbsbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpwztshqp.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gkowmbeaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhselfpc.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gbphfxkun.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghwygbzkr.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/grbarwnrc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/glryzkifs.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ghjonnpzz.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gndogjdtu.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gucbdmdoz.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjbqlpd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/grqfuidrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gtnijeomt.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gpgqoszyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gerilfzpr.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gijdoqalo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ggydvmhni.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gekloiqfg.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtaoapdwx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/ggbsynyof.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gohpsnsal.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gynphlpwj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gfunhwomh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gobrairft.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gpsdzyikt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpmgaqhaw.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gkwrgnpkq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gtugbgbhe.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/ghakbxhbr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gxsomyngw.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gxffirvpg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gliisjxsx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gtdeiowtc.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gcvbqzkpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gozoeamlg.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gkijvfstr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gotqtbacp.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/goaqhvvfe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gvlznjixp.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gsidafdqn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gcivazoye.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/goqocrxkw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gflrpjjza.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gcymdcaua.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gciuzuluv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gngcpyzhp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gargqvoen.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/geuvopqgu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjitlczzp.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gxxwsuxvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcqnlpmus.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gtiicwxed.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gkpyqraxp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjywsrbfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbgcyzn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gahcjvqeg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gaujnzhtz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gdmzamqrb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gxdutylhc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdzfgojuz.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/guosrxgee.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gouhrirxt.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gjdtvfkdt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gbfpcuwvn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyomcjtid.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gzojouxxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmhesrqlr.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gubqbydfo.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gvokdtalv.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/grxkhyaqg.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gjsyptmwi.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gchpwzixu.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/ggtsclrlo.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gceudcuxj.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gjwyybntr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gxgeklhhn.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/glwndmsjs.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gfzzzppgg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gjxxubyyy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdcvlnsbx.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gxqdwzdin.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gcqsstnld.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gbzqudkwy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdfljjflq.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gpugdmxax.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gmsiawxbh.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gxqvzphzh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gyzggkvex.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzzemccxt.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/guxwlbkhk.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gwddinwkq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/grhjcgikj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gyhlfvzrb.sHtML


<!-- 参考信息 -->