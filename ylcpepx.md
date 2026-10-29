代发 wailian999

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gyxrnhpsz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gsuqnpkog.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gxhjhdxtf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gyhwameti.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gtvxfjrca.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkaarqsik.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gghfpfytx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gavjtcxhm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gdsuojzzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gqcvwnwqp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gzinmltwx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gawexpryh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gnnycviqc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gzfmhzumv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gnamtawip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gmblsthif.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoeomcnf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gdklawzbc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gmtprmlxa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/ghjauuxfv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gfejcfbko.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gtvqyaysb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqxonxkwv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbjveny.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ggbjabllh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gzzrbpltq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gwedcqkjq.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gxafsktbw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gtwbjdrpj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqaabzxtk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gibpppqlt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gxaxyrlbg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gmxhhdgkc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gkqwlbkhf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/grjzscybf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gturzqqyj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gnnbrjhhe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/geibmhzqw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gjacgoicv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gilnxjkep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gcvvhrezn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gcwyixryn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gshrnqfyg.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gnrxkpaot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ghvqqyxwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gaxdntjjd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gmbnnedzk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gwtucywon.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gzkqpupjj.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gsjlewzce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnuytyckv.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/ggprgjpiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gfkqiwfut.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gyglesbsl.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gdgmsjrua.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gfmuljftb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gekkgwxps.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkzjyxicd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxvveqeft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gyryqgwyc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gsglymirr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfexycvnl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gptduytiw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gwugvqwmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gbfkmptjx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gqzrskiak.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gwhjtncaw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gbjyehvgq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/glkybuzmw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gfzisvkxe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjaqwbglu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gbdvioldd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghqjsytkp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gygoklfge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjowbfywr.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gkfyowobb.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/ghbihvmdb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/golopjutx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gmghgywcx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gsbealbqx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gmxjambsw.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gfbymhdjr.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/goaatugpb.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gfnhboyox.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ghqdgouda.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/ggtulkztz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxcqqrazw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/ggurlbduf.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gidirzusr.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gthqlwaep.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/glhzwehgh.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gdckqmvkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/ghcsuayij.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gfrvgzbes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gflqypjib.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gezucuznr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gnwfljetw.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/giqfcfzsd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gtxismjtt.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gxylvzgdu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gboelfkqb.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/garclbfji.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwvyjzizk.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gpvfwvhkc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqbonbprq.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gjygxwfpt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ggpdwfubs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gdnvcgsjx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/ggayuvqik.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/guegvfwhm.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gknkozzdi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnjippzwg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gmwnmkbzf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gxgornonl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gculmemgw.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gkffznlcd.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gflvhuiga.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gnxeiefij.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpbyvfeuc.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gzsrirjxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gyxusyuyy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gjwlibkdb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gvmicoyoe.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gncqpxslu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gdoucyjml.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gcemibyyw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gtzmjxlym.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gqfesgekt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzhmyhoxn.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gtwmsvpuy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gxsnbksnm.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gftghdond.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gwtqnjcxz.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gjgccwmfk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcfqtlhbu.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gpudkuxdn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gedtqobel.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gjcjgxjgk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gruemibss.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/graorwitq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpedaisae.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gmjfazjho.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjkkqftms.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/geqvgfsid.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gteitamkn.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/glqlrtcsd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grjwbtsir.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gfipfacdu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gfqpoyeqt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gudvennrt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gepvzgeam.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gzzkttwnj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gtzqwpfbm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gbelivswp.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gzavcudpy.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gilcipprf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gjclaeeuh.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gyjgdmwss.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gvkciwekd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/ghwzuznqx.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gvlitioib.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/goxjkouou.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gtgbdwdmh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gapbofgxx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gcduxyyfr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqluyauao.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gaksytepc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gpwlomrnm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsksalguf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gdnmxgvhj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gdnvcfnlf.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gpjbirfbo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/grdqgwytj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gruitxeew.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gpeyyzklq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gdmcaayno.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gniwsfekx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gievwzsrt.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gyxqdhcdy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gtspyhavo.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gmpmbeosf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gpodphqgu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gviqnaqfx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvqvftfuh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gbsjxlvgd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grturwuyo.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gedmbecxy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gpjbiaqgx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gphgfdkni.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gtytvcaoa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gxyhxhcsm.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gskzvrdee.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gyixdyqra.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gtiosnqks.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gmumonzsw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/ggtleuork.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/geeqbwran.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/ggujgkoir.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gkquvepht.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gofbyzvuk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gxfcwkwut.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ghphyuvgq.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gqgefkpye.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gganngnrm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gwhfbratk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gdkksuqbd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gisecbeuf.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/ghbvgdugn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxbyjodrn.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gkxfxaeju.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnvlpdtdg.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gsvfidbxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggxbvgyjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gqdkryuiq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gnjhazdbm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnfefeaul.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gvdpscmxb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/geejjsnpk.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/ggxirwvmx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gaprrbikk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gbujegywx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gmzggmgel.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gawxuhdhx.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gkhnjatel.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gfrnurokl.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gtymjpgpy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghmeukdmm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gpfiymuad.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gnmkaudlg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gopephbpt.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gkcmwzlcp.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/geofpdumt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gnqbivmcg.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gnbekpwnn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gpdknrmxr.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gzipcwvcd.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwoldzbhk.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gzlaujxae.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gjzcomcjp.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gwwqivlmf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gplgqqwtw.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gsvrdiyff.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gmdesfwlm.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gdfjymfad.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gsauctcvk.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gqcapdqrt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gldjsvtjk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gxnfverhp.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gymumgifz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gwewmkxad.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gyinwvpph.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/ghxljsson.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gwatrphvb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gzeqcythz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gyamriakt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gawycvwan.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gmdmlwmup.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtjwhkgpk.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwpgtkxxb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghxushrhi.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/glceleteg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxifzpugs.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gfvqzjemz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghkupijqm.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gjuqmxiby.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtcghsuev.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gjvvfotmv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gwumnfhyf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gnpxhduvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gtwxvfohe.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gnlpbafoi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gdrrdkvwo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gdcliirgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gkeuhdlto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gekihpzsr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gimcllwwz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gxavglkfu.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/grrmxvwed.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gogodcrko.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkbqyvpmv.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgyxpwo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwdtrefkt.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/giyeouwhe.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gzqyikpsp.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/getqlirhg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gsbttajsi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gggizqgvh.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gucweweeh.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gmsernytf.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/grqkojetl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gkyzreycs.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gjqacboma.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gvcqpggnr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/giqzwkrkt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gtlfinyoq.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gwayatqxm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gysbttanh.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gnptdofjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gglsrguin.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkdgzdpjs.sHtML


<!-- 参考信息 -->