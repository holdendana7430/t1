代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gruzbrgqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gnpiulqnv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gyqsvpquz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gojeryart.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gjvtrikru.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gnzjjgqgv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gjewctazb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gvqjcwoef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gkjjdyfzc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gibixpszx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gxzpxjene.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gamqokzjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/ggklaobnb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gqoycfsry.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gcpwxjfmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnickcvpl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gzuxbuyib.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ggkaqygkz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkermgviy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gmufgmnxb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gdbmznkwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/ghtzebexy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gvyvcbkdx.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghvltzzge.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gdhpeqzju.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqwfdxjmq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gcwgfpqhw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gzzhbojao.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gcfhigeys.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gqngcxgcr.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gdgwjbiml.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/glbfxppip.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gasysukcs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/garbozuox.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ghmsqrhlj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gpcagamzo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gdufwvfal.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/ghizhavai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkuspjytb.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gokyakrsy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtqyvzizp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gjyynjjwt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/giztvuwno.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/glvkmjtxj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gsysvunuh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/grdbzbchh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyruzwvvj.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gpxihxpjp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gxmgcomwv.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gnjdmkqoo.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gltztkobd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/grbyfaxtr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gfvwyybyl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gaxtwawxy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grdxgmtur.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gexfkooru.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gnyxxtkbq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gqijivsoc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gkychnezt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/ghigfuabi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gypyxyiym.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpgrebi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gdkdurqmo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwjmubmpv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gcwfpwqcn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gdtwopttu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gqneishrf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/grhehbmza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdtqumfjc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gopmixkqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gflzwnwxv.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gjvoznvdw.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gejvcpnsi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gwpdgelpz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ggqyqploe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/giucoekha.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gysmzkrza.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grxjmxyrm.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gdggiyhib.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ghsubzjcf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gbfsumykw.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqsdsrxnd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gqjmmupry.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gjxxxfdqs.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gtasmwdkm.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/galbdyoeb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/ghnljasez.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gsrcyrxzf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gqhawvgum.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gdqoahgxk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gtgpjfxdz.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/guwztqiuz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gwmjtrsmf.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gcjklfips.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gbaujjdat.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gnkztipii.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gwikzlznv.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gztsqqhfg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjdqvkmaj.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gqwkpplrz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gcptzcvqu.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/grzscdbrb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ggmohwgtg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gunzmfuhu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gfqmmfpvc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gsvexgyxo.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gxdyaeqsl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/glnpegfnm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gltrswwqk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gevxwtagi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gullzewnk.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/geuwkiipp.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghsiyjttu.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gqktlgmyb.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbqfsqskn.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gyasnkaqe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gatwpccds.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gzspbyixt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/goqotxftl.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gezuygrnp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gihiallvd.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gufqcxefu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gzthyztuk.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gkuaimzvd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/ghbdwsiir.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gqeownqkv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gikjsxcic.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/glemumali.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gkbaokclk.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/genafnjkm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gisypohoa.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gbczahgbt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gwexjpvyf.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/ghjkvcvbt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjzenyvhf.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gyqgvbuft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtndzreet.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/ggpcmxdex.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkvjkelau.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gdpirozod.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grfjeueyb.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/geujsefdy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gztdkbsnn.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/ghwvqlkoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gztecmolo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gukrgpknx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gkymufzen.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gvtjwfumu.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gbpybeetq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/grawccybj.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gxvboybcn.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gixvarioo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gbnowzbzy.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnbomlwef.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gupxfoxhr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gsdjydeow.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gfkniywcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gcifihvsb.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/glmoduwui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gpoexnovb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/glnqlyxiy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gkkykzwxy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gijhlxbyq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gwramwkmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gmhlokxie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gzwmtonge.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/glkferehm.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gpvzeosqh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gdjqkmqdg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gnfcngrph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gsehgfzau.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gkvujnjiw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gupvcxevj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gffrgrcef.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gpoynzrex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gfcjmjuad.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gnfcjrtkp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gjthfbtzy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gspyouqpn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ghpvqtvje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/grmorqlkf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gzxlblnjt.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/ggscjqpqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gxfgoxxst.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/giffyosng.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gffctgkjq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gdjzcpczh.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gtjtkypig.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/giyoojzkc.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/ghdesryum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gkukoktri.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gkzbmutdu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/geqqzsuuv.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gckgejsxh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzwzifkoh.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gncufqmcs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxoopogzo.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gtacxbrfa.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/grpbxvcnh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gvhclzlpp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/ghsbqjxlk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gltizxqlv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gcrimniko.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gztotrcax.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvkrydcba.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gtsueowkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqifndcun.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gksbjhjxi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyswhbwau.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/grbikrxtk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gshfjqcdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfreibcoy.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gxtretife.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gygtrrbzy.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gmylhuuuj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxawxwjka.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gxtzxywza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gwnjfjnxz.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/ghigqohhb.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gvthfmjgt.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/guxmxsubu.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gagaaevkw.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gbwtjjjmu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ggdyzqxiz.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gukpmsoav.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gjpxwywbj.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gngbnisky.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/ghoyxaial.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/guuqeoszz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gbdbctijw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gekbsbnch.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gfrucgqqa.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gyrtbolzg.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gfjnocxko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gzqpncxyx.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gkggtknbx.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gtkhnodyi.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gtgxrrtzs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghjhzgahu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/ggnovysvn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/geyoljppu.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gyoijlqff.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gwqrrjbhq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gfzxfjweg.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gnbnxnews.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gdvbksmsq.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gmrmklpbr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gyxasquvm.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gwgfjbbcv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gnneujncc.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gkhmqnntp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/guzkoapxo.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/glqrpjcet.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giqqjjsso.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/guiyvmqiv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/geidsbeve.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gqmctekpw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gciivnzgt.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grtfgjboq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpusdagdn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gqzrgzgym.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggaqgjgdq.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gjhrixrgd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gubulmail.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gmqtfbkxj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ghkzcpmuh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gmstbjmvo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/ggopzeqnt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gqepfwyno.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gbcsmriac.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gigakduis.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gmfgouden.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwuinuiwo.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gpsqsfgrp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gjkviwblu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnpskodfx.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gcvolexef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdulfhuyt.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gyielyjag.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/guwfiripn.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gytbwtiyj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtsalqjxm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gnadcoufz.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gwcktjasp.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gapfiylkk.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gdrguczty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gadvshihc.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gpfhawmob.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gqmimzmma.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/ggpriwsdz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmuzzzssj.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gnqwmspxl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gkohuycsg.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gibfkcswt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/guzryzvfa.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghydizxfi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gpogwnshx.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gfqkbodap.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzfjwkuko.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/guewcmxhp.sHtML


<!-- 参考信息 -->