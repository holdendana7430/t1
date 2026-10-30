代发 wailian999

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjjdaxsbt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/grqtpvuzl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gljgfbxpj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcexakkuz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gonyrsggp.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ghmekqygt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gboddvdxb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gsfxnyjro.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtohefyvv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gkyuistau.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gszqewsth.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gzavbhxjc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gtjjmknke.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gzfwcfigm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gavqqltzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gnnvmgpxj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gaymmsxsk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gcrgynfye.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/grsnuxbxp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gwgjprssf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gefbrvmoc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gcmjnyosr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpjdwyqmy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzzujgzdx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/glosccgru.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gmkocjouz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gmhmnolry.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gdtzehcbn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/ghadfttqf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjnmnudoa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gczmmhjab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gbveejjge.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjkydecux.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gzrjbfykr.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gesnteuye.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvlbkom.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/grlbvpnrh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gfljwlcpj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gmvdliiqb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/grbreyydv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaguyoota.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gmzqsobnw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gzhthhrkx.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gvzncdtrz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gfzdyradi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/ghvfvfapd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gkdwlotae.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gkxxwamce.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/glardnrfn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpvjzsvzo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gfrmdabyc.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gmeaqvnwh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gkavofqed.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqdjbxodd.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/glqdztswv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gifzoxppt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gnzxpfxhl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpwqwgozf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/giukbzlpw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gkhmarkzw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/guxhzrmco.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjrquvikd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gqqmsukzb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/guofsmjxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gdxleusxl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gtpomexmc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gqutqkhgo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gxoeungab.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gswkhfmcz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gvdvojwlq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gcamtinew.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gxfisorzb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkfncxqly.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gucnfivtt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzcnmctip.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/grilyoobm.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gdmpvkvoi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gggfwcrho.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gvctnghaf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gesacitcu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gfemtcbhj.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gdcppmbpp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gczuoemek.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gelqkwlev.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gbnzeynfg.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/grfqmtlyf.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gdoyrmpsy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gnudwvung.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gzvakiujy.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gupelaxpz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gskrtyjwu.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/grlnqqalh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/ghxfcogdr.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gdlulxazk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gexutlsls.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gtjbccmxh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gjkzmyhpu.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gptzrxshp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gbyzjcqvp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gvfonpvbh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gstqcatxs.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ghcwrvczl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/guxglwmtl.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gzuftccmz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gtripfzpq.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gnfbnmugj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gzltudsmd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gjajymcuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gkoiqqohg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/grokycwir.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gpgkuyeik.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gwwllybbe.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gpgnkhhmr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gsagqeghd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gmnuyekvi.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gobuytkpq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggrcmhxet.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gdudpbspm.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gopohcbqz.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gxqbgblgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqhfidtfa.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gghifgpem.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gwgxnvvyc.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gnkkpqssq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gwetezhec.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gspkmbwzp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuzwvhy.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/goqkxchvd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gekceuqsg.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gvxrloysn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/ggeyrovnn.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gjnuqnurh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gztxhamaz.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gnqdzahci.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdajtwlwy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gikpuzsxr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gnokdqmyz.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/ggcpcwdhm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwrsjkcxk.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/ghshlqezr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gichweisw.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gecutyfgp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwuijqhak.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gjuimblge.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzinjjsjh.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gcujntssi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdhyrlgtw.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/giyskoafx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gbapukzoa.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghvmholuf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/genbwklbg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gmhleilld.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gitrskhqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gpvuudbqk.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/glykexxln.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ghpzjfroh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gvippdpcw.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gmwhnkxhs.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/ggtjbbbcd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gdulpkbhl.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gakowbdam.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gpbvvtzke.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gvgtzzrph.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gedqibxhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gzzpiuhgl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvfzwfgqi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gjxhfnfvr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gqigtbeod.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gfxjxzvbe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gcmhszmtc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/giafdhucr.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gtachaegj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gefvwulgz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gntxgtppj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gnfmeijxb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gqbxashlq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gbldjvhfk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/ggsvzgnpx.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gearvomsq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gjxbibieo.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/guorvydfd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gojpyayiq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gxudrjttv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gejmirpcn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gwwueqxsj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/ghtvdpgza.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gxqlkcgjm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gvdsqhkdw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/grqumrlsr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/glnwbntpx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsmyxtuwp.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gtxoyqcrv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gothsobcx.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gvanpgwmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/govvusnlm.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gwrzfdgno.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gqotrpzjd.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/grfexusim.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghvtauyvt.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gztbsyont.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gcysfzztx.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gcvanoldv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gizjnbfhb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gkempngxx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpaegxh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gtfhgaloc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gqchjddsg.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gxosexlsl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gnmdoygeg.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gljgotctm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnaxbtuwc.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gzxzwdafa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gifyoacvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gxcwhxtvt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/ghzeywosu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjaskxrak.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gkjbzfvec.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gihhodrzl.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/ggztbckej.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtxbocccs.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gumxvxrbw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gvfsauwdm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/grbxvkocj.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/goxbwtotv.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gkxtzasaq.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/guwivsrqm.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gmnbdqkxb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gxknweaus.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gxrjypipw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/ghrlxhlhi.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gvfgoumus.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ghvhmhunf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gaqfyzzgl.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gexsjvvsb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gixnryjes.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gxxvlmuas.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ghcrnjdid.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gqiousgpx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gmhjxgont.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gusoadmkj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giafzeyfj.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gfgabnysx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gpstjpnfs.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gitdggtji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gldqjwwpb.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gbuvuyiqu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/geujlqyjg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gbfhfapln.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gcaxcgyyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gltcxehrz.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gmlpieqoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gulpdppfr.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdspqbutv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gozazrfps.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gsqzxuvvh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gbbzxrula.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/golmcxolh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gukpfcnlg.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gnllokprj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/grhrfaeqw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/ggdaporpc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvztvkwil.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gbnuydmje.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfjhsxlgv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gdpjjaugo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghxecncii.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gkdpmtggm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gqycixwsc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gcdnhmvxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ghqmhwiim.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gwbjhvqtz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/givwlwmgy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ghwptuyyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/glqbvwmgs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsrbmlkcx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gjvcxtgdf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/geiqmikbz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gmwfbgxjp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gapddlqqb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaekcpllr.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/grvlqnfyd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glgprnvzl.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gzeuyjpvz.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/glvuoyrps.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/grlxlemys.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gvvvtflsg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gprrxlwyd.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gcsyxalgi.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gjeamouno.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gdbqfrnyx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gojqfwcnk.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/ghwnrehbe.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ghliecjfb.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gsrubqozq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhbanday.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gucdiylnk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gnpvpuqsr.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gzzafxdew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/grrkozqad.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqtfjmaol.sHtML


<!-- 参考信息 -->