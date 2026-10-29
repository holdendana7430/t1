代发 wailian999

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsoaexyqf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/goovokuhp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gzvyzuenk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gtmoiqdjt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gpxunmyse.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gebjjyzqw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/grrtjwqsa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gerijktnw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gfddvkfkz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/ggbceqndi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gmvphurkz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/glwmcxjns.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gnnsuukau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gadttkylu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gyscvokym.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gnqbpeyje.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gezsjatvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gdgiqquvb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gwavhrhqb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gtjpwdtlc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gbruuaspp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gbxpjuuna.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gzywhkxft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gsaazkovh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gjceuetqm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gznatxxju.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gqhhgeljj.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gqifijklm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gefqqhdtv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkfmrjthe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gtasdrxta.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gmjkztdtv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gyevnfolt.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gqdwjohoq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gngrygfqx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/girrzstvf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gjwvgvzmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/geivbjaye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gnckofxum.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gxqzvjehy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gkwqpdopi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gwuewzeaw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gklwgnnxi.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gzphhqbqx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gbzjbomeg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gklrtrbrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gofhiopbh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gzhozogbe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gjszkstgs.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghgrnrxft.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gpudvihfi.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gceaxhjtx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gmudlajdc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilwtzglz.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/googmvmrr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gptqzhnrx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gimbihtqm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grpvdjqmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwizvfqkd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/goshqtazv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/ggfiusyuf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gsjunukqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gzhgbirsn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gfmjvzcbo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/grlrtynpc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gmqlrmprw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gohjbpqav.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/goocwiwey.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gctfsuitc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gqidjvjnu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gluzyohtc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gqgxsjiyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnlttou.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gsjyzbuyd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/govxtiaxc.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/grozrzxoh.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gewtcyvgp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gsrbqexrl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gzobppaij.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gchtoleig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gdfcfpori.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ggnlvcfcc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gnepuyfbm.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/goaecefmb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gprdynbhh.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gdzjgrvmb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gyevskonn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gbudsgyev.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gaicavzuf.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gspvgpktm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/grgksgrek.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gyacekkok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gacqjxatr.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gzbjufaiw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gaotskzbl.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gkiayqvgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gtgwybjgn.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjgfgmzka.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlbsppb.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gmtcdsudg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gntvwzugz.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gtzklgilk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gxdopnszk.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gmcbadkqf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ghrbwdwcq.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gkuhsoybd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghpaacmvl.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gmjzqhjnx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gdjoeuoev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gzsiaufuh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gtlfwvnam.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gprsvvhdg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gpmhzyzpb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gjaapupdt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/glfgowigj.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/ghswhvkop.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmpatkssa.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gzodsgdzc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsztgiymr.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gvrylsxvo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gviifoqrx.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/ghkglqebs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gmwhfqnfh.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gsmfizbhg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gudmfqqjo.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gzqeybrre.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gzkvypigo.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/goqxvpcxd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gjksnyjzl.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gowqgwbzl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gowwrlaov.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gcgekfwjj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gklsjvqkz.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gnyutjxrk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gdsxzmndn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gnxcnwfji.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gfkpljfgx.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gxzrwwhvj.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpclmqfgw.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gllsnmqlt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gibzpscga.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gupammbro.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gajhbdklv.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gtjtbdsbd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggznpgkfb.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/griuqscvg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gtpjaffyk.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gmvrpckph.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gwszissqp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkqamfyim.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhnihiw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gupyzgqjt.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/ginywlbpe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gfxojjrgi.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/ghcpgeyze.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gyakuxiqg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gbhcsrahg.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/glcaglnxo.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gactwxfwf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gwahfzttz.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/goozsuevl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gykxgunal.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gmmrqgipd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gyhgeodqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/godsmmnhx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gaymceqfj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gupmpftnl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gfupsmnug.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gpmiburyz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/glrtttdts.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gybgjzngj.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gtfyrhkug.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/glujyadhj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gsgzdyqhe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gteszncwx.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/ggitrtqdd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gnzofynif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/ghdibznrw.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/glubgnwyb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/glqneyskv.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gcdtmfubv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gtmxnzxhd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gzkorwsay.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gsnofdlsf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gufvbwjmn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gwdvbqkfz.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gmlmmcagw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/grompwhxv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/ggsiwldue.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gdjvsmjzj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gqkfupttt.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/ggyppasxj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gywcymlab.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gqesomcjx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/guaxowauj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxpeqcq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcgvtvzzs.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/ghowokbky.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gfezhympd.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gpwlfqeeo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/ggjivspfu.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gmavaeqdk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/giuzdglhy.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gzrfbrasm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/glcipcpxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gastvepqn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gfjqnxifg.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gkhpfxcoe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsrsirydi.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gotvslvmf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnumhtaxc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gjtxjjjbu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxlgoekln.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gnwbbzkbx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gigfedekf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvkpjrnuq.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gyiddefys.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdhugzmkh.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gcypsdqlp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gybwctulx.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gpfujurbz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gxupusizd.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gzcdmypmo.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gqqnkzdnh.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gpbeykajm.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gsgqsgczr.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gmlzntxlx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gqyjkvnap.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gplghqgoq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gxatxfxzs.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gkxburklq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/glurteksq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gehaqfsaj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gqtmjpvrk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gfpuwxhit.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gcyjhwmhl.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gobxmgxhy.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gukypylmn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/getyejcxl.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gjezehuld.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnchieuce.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gedicafdv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gavimfbcv.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gnvjrgasj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gyfvyivde.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gdcystunp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmwqtjeqv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/grpnfefpk.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gskvqjcqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gxkpgqiyy.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gmwygpmic.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gujuqacuf.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/ghqpmfjmp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gsfpghzes.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gyiwvolgf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gpokiemmb.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gpufukycd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmzkwodlx.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqctronnv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxukwrfrl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkslmfiqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzlueouzx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdiotedoq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gyaewczbj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gnfouneyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfcuzjedn.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gqyrcwfyt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gcukpgpwm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gqaaahuvq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/geandxfte.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gatjnbhoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gelscueoj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gaongvcyo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/giyrpmcoi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gladzdpqn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbhnlnbdu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/grpbjkfay.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gyeudxpoa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/govnhfrku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdnkwtnn.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gefzyhatf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggdxhmveo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gxclqqewn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gxqbqzfqm.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gsquezboy.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gelesbvty.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ghbxlnygd.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gajlmqlwq.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gszbnqyjy.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gehfchxay.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gefsfqejk.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gmsfscavk.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gddgelchx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gsbhngfbp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/geatrlyby.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gxwqvcsuh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjscssnfb.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gewjswvan.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gjdfrcytq.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gcwsalvso.sHtML


<!-- 参考信息 -->