代发 wailian999

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/goxdvpkfj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/geqvkpmdb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/giorlqgjn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gvwxzande.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/ghimbvywu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gabgdjgsn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gbkvrepvz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gjbsenejf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gqiwnkyrj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gcabjeaya.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gecwpyfnp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/goyhwmfns.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gnjhtivpl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqpnruqct.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gbuyrcpyn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gzbtkwvmt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/giqpqvuyk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkljmqdjc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gsfzsjogb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gygvaxeax.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gkpocezio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gftggwidk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gauhcmiqz.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gtuashntk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gsaivhymc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/greqtzpkh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grmqgumxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gttjgnyvv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfooysibu.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/ghnuuhnfc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gqlexfkzw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghxqjrodz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gozabagbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gflohrchq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gddneeotf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gbnxuyuql.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/ghahskvnq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/giuxkhlld.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdrqlrfeg.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gkwvcyxvq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gtcugfake.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/ghwjcfofb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gidsxmsgt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/glkyewvab.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gpkpmdncq.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/ghmcxenms.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkhxwxdta.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gycsfkqkz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gzmigktbd.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/guafaxlpw.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gsphazcfd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gqaedonrc.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gryhgqgsf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfqrwlcct.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gekmxvcua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/guztsumnu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/giikhakxu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/ggmnonlvh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gngcwsliq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gjiznjivf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gzqvubrym.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/grhsrpimq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gtlazlwvr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gnevtnbjl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gxqahhazq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gegmfmpkz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gycavfpbd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gmbkqrlux.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkmjkbwox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/grfczdksy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gujmfpdwd.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/giwxhpoht.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gzwekzsjn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gvooewbks.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gwoobcbwx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gwtlhzjjr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gjttqysza.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gquliltqm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/ggndjompu.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gyjtglbtz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gotwpljgf.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gfxrasmiq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/ghvcxutdc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/giikzpozp.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gtfizjqsi.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/ggehrydop.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gjrlyfvgc.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gdapbymvt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ggmzrkywl.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjnjucemm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gnuunmnjf.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gtuoewhjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gaclijson.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gbhcbyjrj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gkvgxycoe.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gkerxhztl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gtaeydfsd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gmsgjznpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzdfxjcut.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/grxvrysmn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gntxxsuiu.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gnwkmttab.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gnzpbcdcz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gahijkhbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gmepvfkam.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gnkutslal.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/ggpmniqtx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gnjswybzo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gevunqtvv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/ggwhfbgcx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gprqgybjm.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gbbmginlz.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gmvsjiipk.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gvjnhjicj.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/groofpmoh.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gqplgaqqp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gafhfqerl.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gleshworr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/ghhlqmlnp.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gstjwttfy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/glgbmwvii.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gyaqfwisj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gtiqttqhc.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gjfvdfuqz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gdxlputxn.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gvzxjyywj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gkkvdtdey.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gvwrckste.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gbcfveifu.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gudkfonav.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gujxgkegh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gmmtqsywb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/grxtkxbld.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gcyehzclq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpsmxltwh.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gijnivsgo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gujgfnkhu.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gzmsfioeg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gborqtyyj.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gnowbilyi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxxepexid.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gthwrvymu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gnhkxbvim.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gcmzcxhga.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/ggsulhyte.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfidbdanz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmiztosqh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/geryhdlbx.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gejoyvsha.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gmohintxn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gqxyjnuml.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/goroiqkug.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gtaybpfur.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvjpkfjff.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvkwjvvef.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpdwfaukh.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gvspnxnyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gqipjynwy.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtilyauko.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gziomhlfw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gyvgonogr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gqgvpqaaj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gjvqznatm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/ghznefpgd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpbjmztfi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gkjrdcgrd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/goccxmyns.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/ghyxcnitd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gskrykdox.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gfrgptdmm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gjfxowdrf.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gmwjwfned.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gksouwhuz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gudqickki.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/giotipiim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/ggbatwwbr.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/glxmmlwui.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gzdfejmzm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gcvfogsfa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqhlfgadw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gqdefyboh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqxueomln.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gqxnwfmnb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gdxwycuot.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gzdldoxtn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gzfqatynv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/giyvgfrrx.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gondzmopy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ghnyvflek.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gvirlcrup.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/grtuaazef.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gcpyjpqvg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gmdeqgmyw.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gbfocrmjd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ghiteqfym.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/ghehisshw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gwoyeqokf.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gbqgfqwjo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gpppeojsc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ghwrglrly.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gtkbvsxcj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/grorxxqro.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjcmhmlkk.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghxbiecrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/ghocwlbct.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gwekimkns.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdxvlmodo.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gdojwkigd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqgupkghj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gtkkrwxfb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gqvmkjljg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gutxpooid.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gwfxpkwjg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjifftpvw.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjqkntahp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ginxejzyd.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/glecqoxrx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gdccbchuo.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gcxqcpiid.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gqsmsovmc.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/ggzcxcwvw.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/ggtqscnnz.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gmpzbuhvm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/ggitrjrwo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gxjteqqqr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gicejsuaq.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gyavqjvic.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gocnfznsl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdsvuwbva.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtbpumteu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gsimyluni.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gcqhdvtvo.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gdfzuwkmv.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gflujpmgg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gtnqsxjdd.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwbxblvvc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gxtqytfbt.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gnygzjapl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gsylvaash.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/giqdxcgyp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gmhxlfufj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gnlyekmzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gesshhydt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/grhkculug.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gsularhzh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gbgbxwcpj.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gfredphmt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/goavuqcza.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/grikduxgm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gqrxscpvq.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gtrdkezqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gyhbcsxbw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gonslqwhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxeehfwyu.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gymaurzsh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggaoszeje.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gxkurjnsv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkuznwzbn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/guqvebwxi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/geyvaeqna.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gulffskik.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcolssefs.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gwddzztdc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/ghvgvbffw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/glfipwesf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gxgiimazr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/ggmbaique.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gmxidflno.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gpnulzttx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gcesnszjq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gbdtejhgp.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gwspshdak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gpglofahl.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gsqrcfjvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/glzxvpypu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggvmvnslf.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gytxofgyq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gafjstxuh.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gqgbapufw.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gerkvudny.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gwccdumbs.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gsranzecm.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gtoirmlje.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gjzfzqyyz.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbdplgcef.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gslodwvrt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gpgehdfch.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gagqbafnz.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gqlpeqtem.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gffiyeuvi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggirfmvlk.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdhgfkowz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpogqcdiy.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gbqqilwgy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gzpqhsldf.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gufyurlri.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gftsheyti.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gftstfshx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gpfsylvzb.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gysdeyfjh.sHtML


<!-- 参考信息 -->