代发 wailian999

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gedcuibla.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkaokwnpl.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gspzociaq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpwpkmobn.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gsctlyxka.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gehhbehrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/glkppjhkm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gpguproka.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gahtarmkz.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gsjwwprms.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/geataybwz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/goomztloy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gfshhtvwa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gkxueyxhq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gipntzuzi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gyqitcxni.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gudadbgrn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/ggjyrkjoz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gtfvfwpzb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gxiekuzeu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gqydztblc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gmfipafup.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gyeofigli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gilnuxyqm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gwdyusrge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gjqzlkxad.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gggrxhxbj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gdfghkgrb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gtpfxalte.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gscahcwjj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gvgfdmywm.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gpaancaka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gmovjtkle.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gijggcrge.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gxxkgnbue.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ggcdmchna.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gmxupildk.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gopsytaxc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gcoqbaebz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gwegvpnqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gpjgteqpx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gwxtuewaj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gdgxktxjc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/ghwfdmmnq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gzorxjsaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gvfrrspbj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyqigildb.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gksevjgaf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gdhgjlkyz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gdkbgugqq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gqdugrths.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gclobwwxf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gaswwwvuu.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gkxdedtbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gghfpwxiv.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gcyiydqhy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gsidvgjqt.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gbfjcbiez.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/glhbcnhms.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gcsedjnpi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gzcbqsrpm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gmmtlpnrx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gbmlgfnnb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gavvcvrln.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gmvolbakz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gmkrckkgg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gpdbdudpq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gtdwtyupt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gazwgomrb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gjegmtrek.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/glhpfevin.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gqrayqahw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/grwsfhzbs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gstznswbt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gbwcljjqu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gremjxaiq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnwlyihxd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gakbsyqsi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvtlzmkdf.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/glswhiulo.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/geqzerbph.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gekrnnowr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdjptcqqb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gwfiuxwfu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gelmszkvd.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkfspgfsi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gxavytazt.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gfexvaepb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/ghxwfzcin.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqikjqskr.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gcyamvwid.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gujdymzbt.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gqaykjwaz.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gaqqowcie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gjvzjumkn.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gmasfwber.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/girgevumi.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gmwqqhpym.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/glzopgbgy.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gcoodnowe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gppqhmjed.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gitifcqlj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gqlpjsofs.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gpjqhslhz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gkhazohyy.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ganzvisqm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gmbqhhufh.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gtauxjdjk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/guqckrann.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gkhbllzfy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxfewtmfy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gactfcroe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/givnjfmyb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gkojvceru.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gcssstwff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gbhjexcpa.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gjodjfdva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gdchwncla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gxjrytmtn.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gsnpudxhj.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzpgblvqd.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmnsenhso.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gklcklmqv.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gilpagxrw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gzskyedxs.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gwlvhyyjz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghoimzcvg.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gfmfqlryd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gdnfolusz.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gnlfywnbj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gildlxpjj.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gsgkobzqi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzuxadzoc.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqymvkr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gllrxhsxc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gdxnmmqwn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gzefauvep.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gfhzpegti.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfiairlzv.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gjuzafmwc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gafeihwuf.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gckwasnfe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gttwwqtsy.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gqwidcouc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gsnqauwlz.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gxcuaaaxo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdztgbdhz.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gpdoeqztc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkdkzywmd.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gcbbgvgmj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxfhxemof.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gbnzhmvbi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gxmmzbrqg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbqvuqtfm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glbpyujvz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gbmxatmir.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gjbzcktui.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gayafskpj.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gzofrkqbj.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/grqwfdfve.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gzjnrkhxl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsyutqy.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gzipsixqk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpvzeodab.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gprksauyj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gkzayihut.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gvalrfkhl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gbmokpmpw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gcwlwgree.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/geunzuvmt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gfhfdrcdh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gjcrgqchg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gmxhzagrk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gpmwytass.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/glnefnifv.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gnxhewiiy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gtylgtbxm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gvaametmv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/glsswdbyj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gfvslyrck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gyyotbmav.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gewvmaryu.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/ggjenhhkl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gjwkofqfa.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdiglywts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gdkjloaps.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gymtzmwml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gsgmvfmer.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gnnpmwtjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/glyvjjkej.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/grqkzputu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gyfxlidme.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gskzlriba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gjzazrejj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gppzlumlw.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gghjklsub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ggaccohma.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/grrtawwka.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gdzxdbwtp.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbidlphjb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gpjjxxfds.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gqjvnewdx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gthtyooor.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/giroamyrz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gevuizdsi.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gofiukihp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzktxlnav.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gztqmfzdq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gxuzkojut.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gagkoamhu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gpsaipqmf.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/glsvskgnp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gstachzvp.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/grfbqtqro.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gexbjbozg.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gdlxcpqcc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjwsgfyib.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gohwqkgsp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gttriboro.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjqfplzzq.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gjlkrndpp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwmkqxfnb.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gymfpmevn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbdkepzlg.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqgzact.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gnimvdhhr.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwhuksy.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gxqpssjdl.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gokwqwdcm.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gsnbqdxch.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/guidrqyzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/ghptcsxle.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gnmastjpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gledxawbg.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gpujkinoy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqkubqo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gwqbstmbd.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gbshukfhi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/glnegdgrr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gaiiqrayx.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gwjvikkif.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gffpsemba.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gasagqxlx.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gzwhdyahh.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqadbacxs.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gxyevywld.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gwpgxduwg.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gjgxocgqt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ghwwmreem.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtbryhpvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gshirjdic.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gfquoszaq.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gvbibqofh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gyxxsamxc.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqrwhfjxs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gtbqlnegn.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ggqcgyafw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/glcxgbzjw.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/guqrgmfto.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ghshqwcqt.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gladwijpn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkehnuogy.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gqwtidobs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gnevsqsew.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gcyagamdd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggcxjbmuh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gcblaiyfi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdqcyjhjw.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gbywyscll.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxubahrln.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gvteugkhy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gztbzkwlw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/ggbwvsprz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/guysbheui.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gfzsaptyc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gunpeakmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gddazdflk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gtwrjapcd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxcohflha.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/glgwxdmqk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gapsngmmz.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gbruhhfcr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ggdbdhpij.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghdeuadwo.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gcsjfpjvi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grmgcowzt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gpglyzlcs.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gwaakxbuu.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gguwtfxyv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gikpetsik.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gcvuzntvl.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gvrbvghgo.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gaswivaab.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gqvxrpevd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gwwrghlzt.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gefihnusc.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gehuxhrqf.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gldffklkb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/goyufzniz.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gmhvztglw.sHtML


<!-- 参考信息 -->