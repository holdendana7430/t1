代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/grtuyfczo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gsracycfk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gctoslynr.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gtpxjwesk.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gncutqwga.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbwpptpc.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gsvqssdea.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galjkwqif.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gofiuwsyu.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gxoczgqvn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gjedpwnka.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjwrhbajp.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gnlxhhpox.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gdkhaucxe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gpzdcnrtz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gknaocrkv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gmdozswqh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gtrgmzbbu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gaetiuohy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gxvffclry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gvwuatovt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/ggunjuxpg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghbordcoe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gjzhhbutl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/ggcqwzwdb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gdewcxkki.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gltfjzbnw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gqvfhlmbj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gbowyxftb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfykvefbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gxwyucycx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gtvfxewaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gcnvqtcxa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gidqvxfkj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gciazwaif.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/guhwparqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gudkjikom.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gljjffabe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gjaouvhgx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gocvrgcpx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/grbqtjrxy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbasozl.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/graublewt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcopjzshc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gwaypqrpe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gudywikhg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gjwqogzpm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gfkgjvmpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gpdxlhirp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gpcwlhcpn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gdlpojmwb.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gdbddlffs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/glkjdntxb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ggsdrnqzt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/grtnvpxyr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gmoybgfyk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gdtglwreu.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gwpmakvqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gfhjchivt.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gogooivav.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/ghjcywnse.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gaejebxpe.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gwexxqtrh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gkeskogaq.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gylplbguy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gzghzcquk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gooyuzaxk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gslajrkcz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gdokiejee.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/grlgtkofl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gmwsudgzu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gplsgrewt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gukwoqjtj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gtukgbarl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gkbyngeyj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/glqbozrhd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gpkfjlpvt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gzhrjtiqi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gyfrncklg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gekjlyanq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqayqmdhy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gqeqefznt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjjhnejef.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/grosmqokr.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gamvzukxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gejoyxhol.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnuacaroc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gfzuuncts.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gyhztyydz.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gwfqchcqj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gmjibzzyf.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/glptbxulg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gcwcsrcrc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/giprsbxem.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gpriistug.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/geqanzkgc.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gqklrzgwm.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/guyvenurr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gnejihtet.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/glrkbycfx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxqsltdje.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gvhskbbhw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gawkivyzx.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gwtvchist.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gqifcbodz.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gjvgpiaao.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/giuxgqtsr.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/grbzqgsew.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gcqbqkrgn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/glmpfcoxg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gzyudushu.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/glbhliunt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gessckhfk.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjgvjwjdg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjyixvgxm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gcixfqhqy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gqizskggz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnwacvw.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gwrualsrl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gdereupvr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/ggewsrldx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gbcwqmqcr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gwvaxgfnw.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gxhidwuli.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gipngbvtq.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gtfqeocpm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guvmdhprl.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gnieybrsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/ggrjrpdel.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gswfiobma.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gxthurekj.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gbepanstg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gulhhjfrs.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gzeveaiyz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gfdgldsfn.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gsymcisdr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gcbkyubqs.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gmoqjsleq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ggxlldgdg.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gdmnlcyst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gizrtuvll.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ggqlrpgku.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gggnpmlwq.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gpyxmxmni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gknxnferv.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gexmkpnze.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghosrfofz.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gdjmdnlai.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjesvbjej.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ggfkaesix.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gycgfdmiy.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gmiokqggb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbnjemulh.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gywbcqjty.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gzlprtgsg.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gbrcnppuv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gwbnkhxew.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxeohymjr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gijjjnpto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gqmlrampc.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdskixowd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gceqvinye.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gajemimcq.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gzzeydudz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/grvyjcqhy.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gzgzsopzf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gkzvqksbr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gixvqsahv.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gizihsobs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/galvnmohu.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gfjunrqog.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/guwajocks.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gbzleeagv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gfnbcpmoo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/goroqndxw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gntxioefj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/grtsrfoey.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/grukcwacw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gtlgtnekv.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gkvgcioye.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gygqcxhwl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gtvwaybvq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gwwtywtqg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gokiaeeqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gsdbtvvpb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/grcsvwkje.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gqdgigdyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gknlcpquc.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gmmmzjgco.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/giqdxpdsj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gbcqkhgsx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gkjurynbw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gvnmhomod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gkggdlsfb.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gqqjzovss.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/goyiaszlz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gorngpqxb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gaarcdsxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gqyhuxzcn.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gtoywlmcy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gkrrihjjf.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gqhmyxlqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gjlbmwtkn.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gjporsyig.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gjqkgvasy.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gcovlgauh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjcpogvkb.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gdsgkwoxf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/glfgpyhon.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gopgtpuji.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gvhyxilla.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gahqbbacn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwffhtwrn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gattjgaib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxyfktwbm.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gmvkehquy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsnegfspr.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/glgznggrt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gymdnhozx.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gxeejfzwe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkhmpnrj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gcuygxjba.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gidkwdubq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkwtpgozc.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gtdnsxtxi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsgyqdnjn.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gqtletuar.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzngkqjcf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gwnsxegjz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/giduqbitg.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gifkganeg.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gucziyyjw.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gstjrfuem.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gckkgjuqi.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/godwpdfhl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gcmnzdnou.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/glgybydzq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gxjhbjgqs.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/ghgmfzivm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gweyeocjk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gwoqlzagj.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gihenubhj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/ggenwonqo.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gkxlkguvy.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gxsbpfalp.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gemqvwvrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/ggyqdivru.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/glyudujjt.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gnbtdrkvc.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gmesbvifg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gkyijwiwv.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gdofhirqp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gjhqmevtt.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwrpmrtoq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ginyfujpi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gzcvikzkc.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gmjxagugr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gkdlmbgnt.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/giqmhixnk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gzowmiuwa.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gxwrzodks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gitdpfufq.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gkrsxyrhw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gghkzrfjc.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gaeuecgua.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkbpnxutr.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdybyupxc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbvkyowck.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gbnxgbdfl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gecuuswhx.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gchrwigky.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gketdfzru.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gwcvodizj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbknueklc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gfbaatmfa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gbveklsnn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gqfnkmphk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gotcxvoea.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gxvfsrlrh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gsykizffg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gysmaknnz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/ggadnffea.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/givtzpjhk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnqhnvlqq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/guiyxxcso.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gvvroltmi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/greauciwi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbqgsagub.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gkeqddtxe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbzljvvzg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/ggvswuhtu.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/grxfxvgcd.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gefyckzxg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gmsxtbcvq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gimlbmsjk.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gnfsjukpt.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gfyachiqu.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gdwzbhppq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gzyaabjze.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gykzygsgi.sHtML


<!-- 参考信息 -->