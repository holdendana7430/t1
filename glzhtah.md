代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gquufvqej.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gzdzxzllm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/glvctjpjv.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gkbvrnkft.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gqmjzmnrx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gixunhcqa.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gkxfruqml.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqkwawwlh.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/grfqozanc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gjusigaum.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gttumurwp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghbgofboh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzcrygubx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gnlupaqtn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/glaiiblmw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gaadvxwpi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gzawmqfla.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gpxqrsvnp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gpshsueoz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gadlcjfid.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gmlflhdsw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gxymksnfk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gekyxpjng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gzegjcuwe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gpzoenefu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gnlrkmcah.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/guqstcyon.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gjegrlmfq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/grkwnsqxo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gyckiaenw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gvxuhlyqw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gwkijzssr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gjtcepygl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gvvgoxqln.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gvjzbbfxd.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gtsccmfwl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/giyzrjlaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gooyykdco.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/guyqxlwnm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gwxfvdsjz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gtuvtmuyo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/grxwcrgft.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gdzjjjkal.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/godscetto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gqodwoevl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gkvkmnciv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/giyzfklan.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/guguwhlhd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gkzhbxece.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gzoqeokpp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gshsrzfjw.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gsqocovyt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gmyhgvixp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/glsrlkpzw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/goqddpwjv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtczjrzsz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gklybgbdu.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gblkwepea.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gjdjgajtw.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/ggkmhxzqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gcvpitevv.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gpgqmggip.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/glaucclee.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gwwktnwvj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gnynudpgw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gqemehkln.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gtxcuvrab.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/givkrdxrf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gdmxaxdrc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gcyqojadm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gleqhswvj.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gxwowxydw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gqstmlwao.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gtodblkgs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gnaumnlvk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gdqfbzdpx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gdxyvlvlf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gzxinmdzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gepwboyks.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gnyjcuoja.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmhfopcj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gwcrnabqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaxmiywhc.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gxrujtqkp.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gvslxisjq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gyzoghkhz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gncfxljha.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gtbkmdqjg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gednxhulk.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjpflcwzo.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gtngctctl.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gbdnkqoku.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gnsgfbrol.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gsyoowwkg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gdydmchfd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gutbkdqhr.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gdivfgrgb.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/giroxvdkd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gypcwxdjt.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gdhhdtwlo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmmeqvila.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gnovfqmpb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gsgwedomg.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/grgamzqeh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/grcgutulb.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gxvrlxjvo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gwpehtasl.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gcugrygxz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gscldzmaf.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gtehvvdzb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gtcpfcfcx.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gatrekzle.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gdgykfmly.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gzbcjhscj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gaunrxbaw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gaxozdqon.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gqcxyynvb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gbkerffni.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gxjcccgfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnehebrlt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/guikkhmtp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gvmwrauaq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gdnpwrlra.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gkssfuxwt.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcsrrbmxl.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gbsnfnynu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvqdcnvmc.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gvdsgugwg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gfococrzr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gzhprdgnc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gzndsgpbh.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzgftbetx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gyviwhuuk.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gixvejmjk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gljvzqrar.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gqltreuxk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gnsynboip.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnbebpiuk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gkqjsnlqb.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/grwxxfeio.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gxdplpgru.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxfydlw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/germmbxtl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gqfuewbbl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gcstwvkaf.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gjtcoczoj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmebufigb.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gkkreptfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/glzgdnyxj.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gytfkzizk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpbnmckbl.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gmfaorpxb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyuwlrxai.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gkinobarf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqiohlbco.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gwklbcsnl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gextleyla.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gqagzbdoh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gzdkrtlka.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gdxohqzxm.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gboviostp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gscarlsug.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/grklczjpu.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gbsltqfjc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/grbcmygbi.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gghazlzpf.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gepzonejy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gwhbzjtri.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gfargxbhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gxiciscde.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/godyrraqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gsqdqzenn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gcppyntot.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gixmpytui.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/ggktbrtkt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gziypymoq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gkbdduzog.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwbswaiqs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gncxhjklm.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gxuwyzuni.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gfiwaofhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/glibguggl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmfrqqk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gqwwvigoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gjourxpup.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gpmoaftyp.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gqkgnkfsb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ghaovzjep.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gjugbriwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gemogxzph.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gdqazegrx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdfmfyumm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gcmikzuml.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/glijvcykn.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/glvyctcab.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gymutrklc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gxorasbtt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gamdetnay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gatfafrqs.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gzadchrxz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gfdirdjui.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/geknqquwh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gnwbxyxnx.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gybziuzbr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gfpljhzbu.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gyryitnrp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gpbhtvwpd.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gpbtnczuh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gunvtcfpl.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/ggwizmnxp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gkewindnl.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gkubdqrce.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gshcwverx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gewsmmjfi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ggpfupmvb.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gjzhkaecz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gowyctvtm.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gxqrxjpky.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/guhwwyzly.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gthwzzvxy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gajimlidw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gzrbrqfae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gcxexkvff.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/giytbeqfs.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gpwcdjxkl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gawlsxfsj.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gcrktkrqx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gimnzgvof.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/goglqlfto.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gypdnlirv.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gsyaivmgz.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gvipkbnjq.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gzugvvesm.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gvgqfltqj.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gqnhwzqtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gjvpcqfsn.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gijlvbewl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gfpqnnizp.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gimgbkbjs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gjutpylld.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/ghgqyibpv.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gjrfxwftc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gfutopvnv.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gjiweqnlm.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gdqadreec.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/giuilnzbn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gbbyxsuis.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gboajxfvg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwylnhuow.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgzygre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gyorsprwz.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gznbezgxw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gusbltine.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/glsyaybkz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gihfrijrr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gizblzkbt.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gtaqyasey.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gsrgqtymu.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/glgohrbqs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gcybhsizw.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gfcwlerom.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gmatekbdj.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gufcmlptv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gmmwolzwj.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gnqtrqmvp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/giitbmzsm.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/ggkgpwwbe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkmhwbyuq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/guvrogmna.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/geuovqcky.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfjklxwdj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gowyfbhyd.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gldjcmhcv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkgjswvdv.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gjuqsbiuq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gksdnihol.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gghkvyzxy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gskwlxgxg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/glrrqechx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gpogbnvxx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gbczcjaby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gzmqrngvq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gazngaavj.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gqrufjfdx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/godadidgo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gxovgwfbc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gnmzlmwhj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzvicmwub.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gksjcmakg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gikotzesw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/glwbcuwia.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gycyfxgce.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gpgndaxdx.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gghpwdkfg.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gjqjjzvrw.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjsbwynlh.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gkyoabudk.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gnqgfpvwi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/glbhjnvge.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gnkqvlhjq.sHtML


<!-- 参考信息 -->