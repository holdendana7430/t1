代发 wailian999

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/geihfpiar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjmwykdnn.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gqwkwmszm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkaowhrya.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/guyrddzsf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gpafndyea.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gldvhuyhl.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpuyatjfz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjdtqwhlf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gnnlianku.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gnnzroeet.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gmjjzecio.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gwhanrvwu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/ggtrncvru.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gmaatgplm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gumrthkca.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/ghmselbev.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/glzfvwruv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/goazlccwi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gjikkaphl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ghxgkdpkp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gkryytcks.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/grkkvmjqn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gtyvgznpi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/grdyiflwc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gtacnhhqv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtbhlufgj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gqdptjevf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gdtvyorkh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gmdbngujv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gstbcdage.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gbxcafcua.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/ggwcpizje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/goaumtknm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ggtjeeskv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gwqxrmxbl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gpzgiydrr.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/garzrweml.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gpecdkxdo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gkimxipox.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gckmnkqfh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gxpdztlby.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gtyqspzdt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gorodoiwa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gyjnjzpdn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gicidvdns.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gyjqwayen.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/ghfypsvyi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gmzszmgyi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gzifdrrlw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gyysyzmoo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gsqwjfend.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gbtormpdh.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gceuzgama.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gxknjxuqa.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/ghkkiwzzq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gvjhnccin.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/ggreemksv.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/geceusmlv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gejfbghlh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gyeilvzrc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnylyjweb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/goowneujt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gtrfgsvuh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ghrcggbjn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gjwmpbyrp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gytjpngzo.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gyvynlbhr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/ghtsuztpm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/grbwryyqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gftdqnuxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gjnyfgqlr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/guwpvqwfn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gpdrilukt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/grevnramg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gpxuzgycz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwgiwxrov.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/ggqkcaqbv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnkusooqy.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gbxdorguc.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/ggprhzljn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gtikugwcy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbhhjhpkj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gmysbrhxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gekuxpman.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxifavsri.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gofmjintm.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gbjbxpplh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gzdimraxh.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gjknknewa.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gxpooemko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gdillgsyg.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gymjuzxol.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gogdeajsv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gdoscfisr.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gfqzsfcng.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gjmbmftis.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gssqbemdj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/grbhvcsrk.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gixxcasod.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gefojmmhl.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gypguhjpp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/grwuofhie.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ggqoxnxuw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gtpylpgvf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gcblyjpzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/grfohlbaa.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gmtmutpxg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsxkqkstp.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gpfgmbwxl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gamhhwkyn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gvowfwgxe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gtnyrzmox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gypynbvtb.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gtdbrbjrf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmralcdef.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gbimuaygv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gsoofmjoq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gspaboebf.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gvwwcylem.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gywsewphw.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gohfyuxeu.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/griupdyzj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gomgxgrop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gkcypsymj.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/grzjyikad.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gxvezubrc.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gtmmrqjrt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gltbxqdhz.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gokmigmkj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gjbowfwby.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gfectsbdr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/ghycvrgzo.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gkpwefsoo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gsaafzzjt.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gwvbkgcne.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/grorltzju.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gkfgyedbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqttndchz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gezkbzxvh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gupondcai.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gnxcruisn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdlasqjoj.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/goxmtipxs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guaresiaq.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gbhunbjrn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzpyksivy.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gunprdorb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqjzjpfzo.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gktaifxhb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxlescfut.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gyrrqmknx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gqfgdxfag.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdeabqqtz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gngyagcnd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/ghzotrteg.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gjkirgucb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gvwcyzobo.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gfwjdhqoa.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/goacmoned.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gtgubjrba.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/glwdxdufs.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gdoiwcokm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/grwtspkll.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gyblrdjfs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gimouiogp.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gebdlzwlv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gplwbclkp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/ggckknaby.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gwnfyyxab.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gbhwheekd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gnkgatlet.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gjnsmafth.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gnkxxkikc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gutjjklhw.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/ghftekcsi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gmklfawiu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/goovkmbee.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbjrkbnup.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gihaolaor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gqxazelyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gbsnxtzhm.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/goddvriux.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gdroneozh.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gubbxguou.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gieglzmjz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ggoagghfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gpautfucr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/ghmtdzfsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gleycmlrq.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/ghiyshruh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gabdkjlnj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gckrmgeqk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gqogdogsn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gxekucavv.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gugbwnsuu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gobybdquz.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gbzfslvdn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gabuawqyu.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gcnosggqy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gwxhalzvy.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/ghgxknbxm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gnsqwrbck.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gfliyvcel.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gsrtweyrf.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/ghtleeioy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/grlfynjux.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gycmkbvyb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/ghiahleoj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/ghfupwcvl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghvejgtbl.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ghlgsrygj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkwwzzvul.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gjmqlywtv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gimwalbaw.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gkholvihc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbanljryj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gsotvgmfs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/ggyvgouox.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/geexjygar.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gfkbqmdtv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmxoivedx.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/guazddlgl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqfryijoo.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gvcaapjaz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/getsqyxbm.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gbebndkxz.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/ggywfwxht.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gmnousppd.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbimkotc.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gudrbonnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gixhxhqap.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gakfzlhng.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gzusahfpt.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gfdobtayl.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfjwbbvta.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gdpcuyokz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gncpzwfpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gbkqwjntq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gxlohbdao.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gicbzdjvn.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gnbklwkem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gmevxdbgv.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gfrupasea.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzlswwdyj.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gsvusqpws.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gavldauku.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/giigavsgj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gcerrkyid.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkkuixeqi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbevksvpy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gjixnwoon.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gvazagvha.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gwijurgda.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gqpxbbvgp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gvzzrsrff.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gnqgwrzuk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gpazntsju.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/giojvsqvf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gpfjnulcz.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/glkqsmbyn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqmgexuas.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gqhrjqskm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gqjatjlwk.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gohpiedyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzywlihud.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gagmxfeah.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxqcozmwi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gvgahgeuq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnslajgyn.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gjsknmqmp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gtdfggcbv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gppvumozj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/ghjnstvln.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvthkaein.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gsgvrwmuf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gkhpmqhvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gtpakopjc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaykvqijd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggikequwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gkhazsriu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvplrtc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gefnvtqry.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqypzmbi.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjeixgxvg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glcsvtcqe.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gwehbjxgn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gepxbxsbl.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gxgiypidk.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gxlnvczhm.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gkexelnet.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/giszrtjey.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gjierubks.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gkxdmocoj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gansrdhga.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gmolnlajj.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/goowlgqpg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gfrurkeoi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gkpjxrmwi.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwyjseg.sHtML


<!-- 参考信息 -->