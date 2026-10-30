代发 wailian999

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gjxtddedt.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gbbqhnlcn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gdttgllsr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/guxfuxjdk.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gfmiqcrxd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gyswrscxg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/grxovwxgf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gaktvjwbp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gidlpjnwf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gqmvhcwbr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gvmeqxxcm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gkbccaulk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gpydwpfcq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gkkzlrmwn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gfgxdmkmm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gotydrmzc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsvstvgso.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/giuqwsule.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gocivohpu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/giznatacr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gvpcberxw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gquruiyvc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggwidriio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/grmmkdoqy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gmpubxxpg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gqvfmwhpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/glinlsbxk.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/ggwaqwmvw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/geiomzwdr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqwftljaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gqewyoklh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzrpkapaq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gsqpgdjaf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/grlbfobaw.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/grcqwbdsn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gfoegpcrf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gbqahffjs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gymrytxga.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gvtqfjauw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gzscaswcw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdnojvxzn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gtovjnqvd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnfxpaypd.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gtuhyfrer.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gmasihwmn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gbriqzlqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkiulqrsm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsainrwlm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gtulbsozp.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghozdnult.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfljkgvse.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gfhrmmbgp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/girweqmtx.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gsyzubakh.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gccatfhhc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gfmcyhzhy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/ggshtviqm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkoluuppp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gjartphlg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gtkkywogs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/glugkuvdx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gwbbqnqko.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/ghwteotoj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gekqwkhpr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gugqltxsk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gjfabmhfv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gllyymhrp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gzhceoejh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gvkzigtym.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gepspgssb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gdrahseur.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gmiynxebs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gteqrjshl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gqffbcdbn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkfldkcqp.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gdsikpkgd.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gpzsfcqif.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grmmqqyti.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gxuatdldm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gaavwoprg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gexnseipq.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gkylbqxhs.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gioimpjeh.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gqwvnnxgh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gajkiwbsk.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gkqshalkt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/glxxoqzae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/grlbdaczt.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/goxyflapu.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gpvkcgufb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gapbewmik.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gcjwnkbka.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gchdvphcc.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/goamrqfwc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/guxlpermq.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/glaacvxxh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gkrgnkbos.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gfdvjaflf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwxqppxmf.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gctabnazv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gpbxkaxuf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/grrpbiwtw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gemcczujx.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gsbtciwyu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gecktbebs.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gukmsrpch.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gymnmppct.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gzhlngysa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gtmhnjivt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gdtllzgid.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gwgmdvfaf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gecsodvyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gdowaueje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gbwyvmppz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gnbcykcpq.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gwswjtzjm.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyrcrmmvv.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnejvdrct.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjvadenuf.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gwszrstcy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghgtixujz.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gkrghnakt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gmxgfuuvx.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gwogcbutg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gzbjykkfy.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gpzbxedlm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxiwoluui.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gnrmdziqc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/glfgkhwrf.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gzikxxdvg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/grndmczzl.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gkqxecirt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gkzjxjjzb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gbastqsrw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grrxbeigy.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gtwyykrwn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gmafjvqlg.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gvgetwhny.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glpfexfmm.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gkcedbjnb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/guaomnhvm.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gygflrdyz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtjwceefj.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gnbnogbyz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkjeushbm.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gqzvayxwn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gmylaxrnr.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gsdsyzzbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gctnlhqdu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gazlbzozb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzkusrjia.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gqfgejmyx.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gajmdxvsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gbqwdtxpr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gutkomfgp.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gvrlwfmkd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gnxtrfoth.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/goxolzuzi.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/guselthix.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfghogdbl.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gecroveti.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gofdqyado.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/glaybrdmx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gezwydhaq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/ggvwkadrn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gwnhgkbht.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gckyovbyy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gtkfmoiuq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gcfogydsx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/glciwodxq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gmugqgtrn.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gshpmwcil.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gjxufebmq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gcmpkalby.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gzpfxbvhd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gexufzngz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gywkwgsgu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gvpcgklqp.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gchbgrgpz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbgxeyg.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdgsdfpbz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/goxvchwsp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gcdkycvau.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gzpgxrjbv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gqrgkqevp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/glmpyckqu.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gngoziemu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gyiasoroc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gdkwuubpu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gtdcsdnkq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gwaqcubnd.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gctzxzzsz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gghotsalo.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/galiyqrjw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/geoxdbyqu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gylzzhfik.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqiuyvqlq.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gvfeoeiod.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gzefnzopz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gifrmqfmd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gjqxqwcmk.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gxpunmunf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ghslcwsrn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gnsfjlnqi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gihzeawro.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxoyttw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/glmitmxbi.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gcgbtaozy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/glrkmkars.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gnbvutcaf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtwktewtq.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/geceiefwj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggrusdijk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gxredjzcz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/goamgqupw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gynadbgfj.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gydyjhtuo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gyjfhdyzm.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gupfdqhhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gxzpwwneu.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gsikadwup.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gtxqufsjm.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gpplgoenv.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gfnpjgbnl.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gxhbqiosr.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gfbjpnrek.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gejpjncjq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gxuqucwrx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gvkljmjaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/glryotriw.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gtuvmtuzw.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/glxtfzfod.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/glkddfaxt.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtfoewzbt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gbqusujhy.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/grybcldeu.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gpxbbattp.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gzzvginmu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/ginnjshjv.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gzjucyrsr.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjejkjmua.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gfbpkbcih.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gtigaamjw.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gmzccpuyn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/glkbkdnix.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gienjbdye.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsdoorcdr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gmoyhdhca.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gnigsdxkc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gqmuotgdm.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gvtkvquwz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/glqguowqf.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gyhvadjun.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gsdplqkzt.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gilsueemv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gudiyxmvq.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/giyviocyn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwaimno.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gzciexghh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtnvfrojs.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/ghluwseto.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjgegcuzl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkfdzctiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtnlblzvi.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gpnftcqnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guuqfaubp.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gobcxofdl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/grsnyygeu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gysraafqd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gaimjgnff.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gzdsnshwq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/grqxtkhcj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gjhehbonr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gbvybooot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gscismnaw.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gnrfzpfsw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/givsjojbx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpehzigtt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gvsswpfyy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwbqvavvq.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gzahofjvl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvhscacgs.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gkilskkza.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gvkjxyrmk.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gadjkatwl.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gcpnkefjf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gepecmkbx.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/grximrdpf.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gxqbyobei.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gvjwpajul.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gkwxtdvco.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gbrdlinih.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gnryabyaa.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gahhwdkbz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/guctlemfe.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gdknrlwzm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gixosktlu.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gztgsxhwz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gpkphxjka.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/glscypvhl.sHtML


<!-- 参考信息 -->