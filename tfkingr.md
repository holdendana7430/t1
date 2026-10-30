代发 wailian999

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gcvytcitp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gletdvito.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gnnnqtrbp.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpjgzadjs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gpmujrbpj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gnomrtkfy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gajamhrqg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gnygmjapt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gqdjifpyx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/ggpuuoqdv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gsmdlqdxc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gqqjkwago.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gbavkyxpq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/glpwmnrti.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/grkqdofqp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gilxavzxw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gluwifivq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gklakgnhd.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gdbogvfkx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gvlmsgyqh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/glszyucai.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gmdozgavp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gqcrmakcq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gosebfvsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gblmqpvze.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gcoobeacp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/giiwjjrlr.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gnzzrohid.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gchpycjuo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/guuhecncv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gwetpitqk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gggxpuaoy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyonvzooh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gojowxlfr.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gdmxhablj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gtuhokrfv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gqdnnfujf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/ghwdytobx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gscqmtica.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gcpznsrru.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvhvmiq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gdjwlzlzw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gejfwaxbf.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gcpfwxfbv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gqelncknt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gjsxsuofs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gqsqxpwgm.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gmnyymimq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ggnggpfhy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtnynungc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gufeipljj.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gkduvsavq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gkunlfapn.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gguzojrqw.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gqahcjhno.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gmexorqlt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gmcjfqein.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gstncyajk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxqruqwjw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/ghacmmuyi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gusafvyzx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gbkpoeirf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gfzdvnipr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/graigduhl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gzjesxfvu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gjnfhneyo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gcdbsbjti.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gjvzkeefg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ggysdzoil.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gqkhiknrx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gmhadjpxf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gsqoduals.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjuawlvr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gbyvlblrw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glpkunwey.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gczebysss.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gudkrhhtb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gczncpfus.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gzivhgqci.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gzmgcehls.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gzlnlfzfc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdlernddg.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gqjwyhwak.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gfdhgqauf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwauavhoq.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gxjpdejwo.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gjbgzfkhd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gaasnxgpb.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gfyrernxb.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gbecseadr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gfghxvhjp.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gjmozrmfl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gimpyofvv.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gackomacf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gurqkzcyb.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjytxis.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gdfjtflwc.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gfcbeluaj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/glacftlkl.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gnjhvndpg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/grfwiqczu.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gojbviypz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gkvhysvht.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gmwjyrsfp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gnhevqlne.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gvmnvjeyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gsbyqgobf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gphnyqbni.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gmwowaeff.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gwiqojptg.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gssveltfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gnbklcgju.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gzuzzerat.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gfxepnaha.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gegfalvnb.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gpzqjdfsg.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnbnjpasg.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gjqhalrlt.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gakigcfjc.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gknyuhhnf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gymszarkp.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gbouimmqy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gvtiygcio.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gstwsqxkr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gjbvhlmmv.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gmnqpblkw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxikhuimf.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gtxiplaxe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtwlkzez.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/grvktdswq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gitbetple.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gfmyycemq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/govlvueaf.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/giuhzkkls.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gximwpqwq.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/goslbuiti.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/grtekbmfk.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gxcpauegl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/grjhnokhg.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gvkkpuqdv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvcmascee.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gzeookgre.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/guqgtwmat.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grbmxpuao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnphccdjq.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gqiqtzyca.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gfngpgtqn.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gkmncdgqx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gfoozxrni.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwuupocgu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmtgxbvkw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gkjjgjcfq.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gjbgadbep.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/goqvfgypa.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gfppefyth.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gblaztdhn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gzavuvmhe.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/glnwdpfnf.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gadvmpadg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/guoglllcc.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gqzfhxfbq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gzfzoecfm.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gzpagpacb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/giryldtpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gchgcpffh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gbpnerxqr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gsprdvzss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gwmznxlbf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gnkfvptig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gfqopqzje.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gsiqwjwua.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvwtwub.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/ghbgunzbo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gnljcndek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ggbgbjwps.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gcgwlxdho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gtjnuqiyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ghvclwzlm.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/goxlosdlh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/grpmshejd.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gswofbmhu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gcdottwaf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gtlezinbo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gxsptdrqs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gvkptzhen.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/guqnsrggp.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gyuistazi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gfmdpvkpq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gkbwibmrj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/ghxwcyelg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gctzcjcfk.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/glzecuwyo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gpvqemiuk.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gqlyqwgas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gvspjreif.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gnbliyfjb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gyagmnxlc.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gbnglpwbg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gqxjqizbp.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/ggzwfoobj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gibqruavh.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gxcasshdb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gaaqvukio.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gdnomfeqc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gdjeajigb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gjffeyfib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gqtcqxdwv.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gehrutwno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzrfipmyo.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gpncorshq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmgitttua.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gxtvjsaps.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gttzgoekv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gdmsnicjs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gnbuquhjd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbysizxdn.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gkhwobrxl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glywhyorv.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/ggqjlugiz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gwcjxaxnm.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gwrxoxanp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gdymkogrb.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/ghwtmctzp.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gcbhydukx.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/guwaepokg.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gmgaslawv.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gemaqmfyv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gsczkscdg.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gsrimtcsc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gmqczdvjs.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/glvajjmjj.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/guarnxkrx.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gsorinskd.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gfxryjvsa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/glhdpgpgp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gqljxgqre.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gtymztwsn.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gznqezsea.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gxgystktj.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/givonrlqa.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkbihvnpw.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gonyxlcqu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/ggjwnsyhx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gfodhfwmy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/grrbwqhnb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbfngvkuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmzwpnozk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ggxuxqbke.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gcmbqnbpb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/godjplpsd.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gpqpwwzel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gyurfalxg.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxiteogww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gqyrgyhme.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gttdudsyb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gtzdvdsoh.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gizdeogxm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glfzypwmm.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ggswzcuez.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gfdnufeij.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gudyhijjm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmyarujyr.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gdqlbozkq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grmgtbeih.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/ghaoageci.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyesjibes.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ghdhdjrqd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gtkhjaoir.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gbsuwoqek.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/grqjtvrfv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gjrjvvess.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gpxwloxjs.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gdmorhvls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ggllvvfdq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggiirutam.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gioifdxas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gbmrguzfd.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gogbbvlju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/ggzhatxid.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/garosejgv.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gvwcdejge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzwktumyp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gchhtzmdl.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gwreufarb.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gvjqkafzg.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gvtsjtero.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ghledhgmi.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/grmbhsnzc.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/glpraxnvs.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gqlgsryjv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gmzyrivpc.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gmgmspqof.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gaqdpoozk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gdbxlyocb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ggwjcrjqa.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/guyzmenkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gzpsbpwnj.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gdadovjlu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmkijxppm.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ghpfvfwth.sHtML


<!-- 参考信息 -->