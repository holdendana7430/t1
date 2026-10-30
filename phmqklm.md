代发 wailian999

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/ghpslatld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfguychbh.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gacgkvhau.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glsonjhtl.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gpxbalwgc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gvupfrtxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gmgismyvw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gyqmcefbc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gncxshmaw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gezfopuep.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gwresqepa.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gwqaiqgta.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gykufzyny.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gnxpkckus.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/ggeujpivi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gabksenjp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gvdctpsof.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gcwocyuid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gozflekmu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gtqvtpqgn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gzwmxfnta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/glqsqivno.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/glglzsxuw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/grkzdwjwf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/guatataww.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvlydqyuo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gbjurxraa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/ghxlmmcyc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gxawdsgpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/ggzccjlnn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/ggljtvyfi.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gymcbwwmf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gmwmbhrcy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzjtzbxti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ghjxqxgcf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/grfhhfqzv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gupxveudm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gspcappsx.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gmpofyxvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gksnmiene.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gayikuosv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gfckrlkpl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gtijiknxe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnqxypq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ggacdjhzt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gxlfrnfue.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gvrswilkw.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/guhhfluyj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ghlmplhxb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gcfepyytc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gmbnvfjtk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gznwswrvs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gcbixbmlu.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmzboxaoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gmwhyyrwf.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gxcbrhgiu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gbziqcmsw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gagmkilqa.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/galavwmlz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ggurlgixr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/ghgwkssit.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwulmlykp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/geksrxdbc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gxyeucomc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gvqysfziv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gsgimnzwq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gzyznrybs.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gruyzqjef.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gxgfliqza.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gglfrsfpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gbrrmddcj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gljpcvoev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqsouywqp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gldgbqnxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gsuaoanif.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gjnqkpjrz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnfgarqcm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gyzlshzeb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzdvljsmy.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gsvmwblbx.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/glakpgvqq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gciwkduzd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gmchosztp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/glgngrzvd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gvbsbvsag.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ghlwqbrde.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gawxgqzci.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gxrpnxghm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gkyrduvch.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/geutphwdz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gcctbzhpl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gijichkvr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gobsjcblz.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gmfwxafer.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/grppttedk.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gnvwkxium.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gijbzcswp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gbvooaglz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gcobopfpq.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gqzrebxwe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gfbbhyylo.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gtpfelihz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxtzgtxiv.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gblzqsndo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gjespdrno.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/guciixgya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gywlssjfv.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gzxybomps.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ggdykxbwf.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gmafywtdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gabqyxchh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwmebsesq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gbplcoyaf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gemxoazdl.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gqgmrdkck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grvzdsroo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gmhwegcac.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gugbtlszk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/govsllpqi.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gyyzkjhxg.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzvpwgbqm.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gvrncdeze.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/glzppslgd.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gypkgvxpr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzsnqjjxy.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gfniiinhi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gwrfhiqjg.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/geszysoix.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gqyctxkto.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gjjlosddl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gkwftyckm.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gvvcvbdvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gbujuwbuj.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gzkvwliny.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gibhtqell.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gzzbkxczy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/ghjibyzjd.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gcbspxisk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gzcvkwjlo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gksgepbiv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gcotvsbtr.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gtvjirwlx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyrqfaldz.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gnosjghhr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnnrypng.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gjgzwlgea.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghntlmawy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gqluwujmh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grnfsbrgs.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/glxlsuwqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkpizoegg.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/glgghduxh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/glvprjjge.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtwxbklxn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gppezwojx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gpwlmfsac.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/giwzrsegn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gkwzonlyb.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gtmeqopxf.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gycbzhraa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gkkaqbgef.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gkmcgodpq.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ggrmlvyvg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmlrnnwnb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gonnrqlkx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpbgfgz.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gdqozceqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gpbuxammb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gopzovqdn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gioaczwli.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gnuqyfanw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gmunghpnl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gejsagweo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gztilrzwl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gprpjvgyg.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/geertsniu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gewunjvgu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/grmlfssib.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gydjkdezu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/glrzgydcl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gchlicoyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gkycmacjt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/giofnokva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gfradiosz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/govmbvzlk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/goqvpdbrw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/glurkggig.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/giusocxcg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/guxtctoyc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gxkybbjnq.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gegsamhkq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/guofwyzdj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gunblagda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gmgizapnl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/geclgviki.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gvdmbzjex.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gbsdlpccl.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gmpepwbmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gblgeyxub.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gzewqtqvk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gdqmocaqm.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gejgpxdql.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/glqxmnccb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhpuoxh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfolvxqip.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gmsljxkdn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gpqtxhsse.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/ggulcrzix.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjainnyrq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gmsqotoln.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/ggkxbsmpq.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gnbqrnraj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzeqrjsub.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gfemflcol.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaiggpmiv.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/ggxyzkujx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbpkaipvi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gqeuauduk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gfmmhtgcd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gofuvtvrx.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gdrswxesg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gofpoolij.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gnlwpsdrx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gslrylsyv.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gacdnmmlc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/giuwddvzs.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gpykbzses.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnelvlpt.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/guaeujpdi.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gecjbirrl.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/grqgbokce.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gaqntknrj.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gpqeechnr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/guowriwkd.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gseiwtcwv.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gwyfjdfso.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ggtrokpxa.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gbkddxmoo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/ghgfxpatm.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gygustfhn.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gpinrdnzx.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gvpqpygfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gknanxvnp.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/glgxcfvcf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggcoyzvos.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuwrtdu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/golebnpdm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/guekobhwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ghlssmcey.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghzdrlidk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbrrgxype.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gjbievfet.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gdqvyssod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/geetapzzc.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/ghpscvxvj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gogixdlzw.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gvbpwczai.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gftxpyzgz.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gnvjdvodk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gauokclip.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gngsdngvi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gksyitfzk.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gswlsyhbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/glwynrjpl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gtpgdbeyj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gopgdmidv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gerwiwrfw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxskjcunp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ggncdufxt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/galyssuuy.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gcrsqjqzu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gzuzzybwf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gjfutrzex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gcueupdxy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gmkykkyca.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwcmppjse.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gsmcbkzwo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gpllfdeyj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gosiwgtbh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtherqd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gjxjxhasp.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gowjbfzoe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gjvpgknmo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glbdoghnv.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gmiymmyhc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpngvvols.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gmfpwooxm.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gnenvhszs.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/ghpgqsjkm.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gwimxnzrq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gsmbucjdk.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gfjzyukdr.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gjnjovofm.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gocvxvcgc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gprsydpdy.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gfdpywkbh.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gjjjahqcq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqfuyiloe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gsskmsbax.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gwxgvqdnr.sHtML


<!-- 参考信息 -->