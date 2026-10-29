代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/grpeesnja.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gcpzhjtjz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gzarfwwso.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gqgnxpmti.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdaernabh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gslrgstas.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gtbeqokzi.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gqigqnymk.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/grajeeklk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsxwwjlhj.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gexphstpn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxnbvwson.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gbiutweio.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/guwzvkgzt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gxuccumss.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkwkjcxor.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/geacljlhg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gzenwojvd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gafnccjev.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gylrcvmmo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gljwdxtun.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/geztxouwp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gvsfbeike.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtuxytnah.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gtejiddya.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gnfqvaydb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/guwbnulwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gwowaitnd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gxpfwvjsg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzrfxdzsn.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpvjagmdw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gmjiqdpmy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gbxfmyfah.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gpbpounui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gjbatdpeg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gytkdodzu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/glafxttng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/glkcertly.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/grqwgawnn.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gxohnoakg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gpwjxnvda.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvxuiqkrs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gmwaxwzsi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gtrahjimm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvcdgcvrs.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gwolmcmwc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gaqzquhru.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gspionnhy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gofqwoonq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/ggkognoll.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gpwfeyprw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gzrnayfgh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gnuggmmof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gemsnepoh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqpizzyvm.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gvqrrmtak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gmlbokglm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gfhsmwtun.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gtwrgnuml.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gzslhywey.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gsymgbcco.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gwliytupl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gksapvzxd.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gbbgwqinl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gtrhvdqgx.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjuxisqvm.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gnpttjuzj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gubmnjvan.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gjoaeoxei.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/geeqscqzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkczvutdc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpvuoavka.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/ghslozpvg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gttqewfbo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gobdhpxll.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gagunpewj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gwixnhudn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gegadocne.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gfdarypli.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gblbiyqvo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/glokmbnig.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/glqdzpnqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gcwdsdmsr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gvlayckya.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gipoqmtvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gmrttyqyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtklrvusb.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/glaubktri.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/glbqvpgca.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/ggidmanoh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gpfqmflje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gfqxbhnen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gimlqxjjx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gobmguxlk.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gzkfocbiu.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gvddoidzg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gfucyhdaz.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gahoulcoh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gnncwcvih.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/giucgkoew.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gcygrqnet.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gfnvhiosn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxizhjuvb.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gtmkqcuig.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gqyubrgki.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gjzlwbfvf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gsnjlgvna.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gcamytppz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gnuatzaad.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/giweydnot.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gxtpzsngc.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gakrevgam.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gbewrjvqd.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/ggankkfug.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ggjwyedrn.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gvatxrfdf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gbiicimxw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkpnitk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gawaoxbfp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gbswtetvl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gdymvvxdj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/ggirwlsbn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gnudboaoq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gabmiqrjg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/grxjxkxcf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gkgqyuiab.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gqxibtozl.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gtdeavymz.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqxfqjhri.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gublrvlfp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwonkqx.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gcgcinfyc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gftlaxjyg.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gwxbfvehr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gkvkkugok.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/guakbktde.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gdzhqfksq.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gmqswpmzk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqgabdhnr.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gdmpjefnh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gobyrrymp.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gzvynmcnd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gpuxbvbxa.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gqfhbulsu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/grxslhndw.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gthdwfepp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvpbcabcp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/goheyunml.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gfespcxjc.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gkdiiwdey.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfkacjyym.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gogdgffhe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhtjygcr.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gvqazvesr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfomdxiij.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghqlebqmw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gewwstate.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gkdibtzcv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gwxgswkoj.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gabdcxplm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gkjmgywxn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/guwxieihb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvfpyukzj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gjzzlhxqk.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gjezzkahj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gnryhcizz.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gsygdeqmd.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gzwfckuwp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/ganjtefyi.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfayyovqb.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gcbnvgsfs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gnkbetlrj.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gcycckhdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gbgbtnidv.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gkaeazczr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gsehulecl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gsofndbgw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/ggcnnyndl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gkksxgyrx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gogkujtch.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gtryqbaai.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gfsnoymrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gxouxqnri.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gadlasdko.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gapwfvsfr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gdvmnozjj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gtppjjkrr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gaytiwvav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/ganhjqisr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gsmzthhvv.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/girsdybge.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/glxbcwknh.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/guvjafjjy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gdgzmxagg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gmocltujv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggxrgpxqi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gluxksyzj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbgyaeosj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gzlhwkseb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gnycptkxu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/grgbyacmb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gyjgmopjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gbnnnbiav.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gypasjlmk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gehzeacrw.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gtjmfolzo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gctwhdhsp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gnaqylncs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghmgkmyau.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gnyyrpjgz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gkjnmksyz.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gtzomqipi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gzooeouym.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gmxverimi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gxaeuzzrk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gcqanvnmj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gynkqtsqy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gpqzbiurg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gimmmdgps.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gnxorhbli.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gixenbgtx.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gmsndvzib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtyqbfscf.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gseutqikq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwemarrkt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/glrtevhxv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gdwuiwpqp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggwwnhihg.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gnwjywgwo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gainotmqq.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gcdstuego.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glrinowoy.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gaujydlqn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gbcltgghj.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gkzibslin.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/geqcrtrkx.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/glpndksfs.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gnrhmyeog.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/ghshfdwld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gsjbgafkr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/grcceudoe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gjwzqnjwr.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gynbvpflk.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gwtneerdu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdmfsaktq.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gnkxnwake.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/ghmsowiei.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gwkebsiiz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gwahdnycn.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gaanigsbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gaeeyicjg.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gdqqmjjaf.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gyvnjegqd.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gqternbva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gacrbwuxn.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gxixkxydn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gikipvtvh.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gaqzyxmft.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnvkemarg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gdnscqepm.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gezcsamtj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gqdqjkjgz.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gbwdyjmpp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/giuytkjpv.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/glemmzrok.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gdcdialfa.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gmthydoph.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gnuqibjct.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gmyntgjmy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/geqvvgirx.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ghkebnjip.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtqnkqfka.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gkpudsody.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gagjbjzmf.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gyidjmjyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyctfaeoe.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gfjfrtpye.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggatmcoyg.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gzfiosymz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/grnffenvt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gojgowmoh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gddvcimdm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gytyprwzr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gumoznbls.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gbaknqsbj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gggdpfqqi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyhjegxpg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gxiwzqooq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghobobtej.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gtmxwuabu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gznkcljqg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwpkoqdpo.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gzbsrtrfp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtmnqppbd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gujisajec.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gfhjgfvsr.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gtdtumtgu.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/giiztdsxf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/guexahtfw.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gwkcjcers.sHtML


<!-- 参考信息 -->