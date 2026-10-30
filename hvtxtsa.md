代发 wailian999

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gcijzbccj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gndobtyfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdthywpok.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gddlirxyc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gtkabrfmw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/grfqxgcyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gnarhbxld.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gqekvjwqg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/ggsguogqo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gndxcqaiq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ggpbbuigr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gfkuenoub.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gstwgedvm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gkywublll.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/ggnkgdsli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gvnxtppdn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gkufcolla.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gxxtggadq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwfyfojqh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gaidiywab.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gejilmevo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpnbvxu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gsqicmawf.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/guhbusqxw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gyqcjvwfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gpnrbstsz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gaoymfrmi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/garttwazc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gduluxytk.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gmmlvzqpf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gnwfhwfdb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gauyrlgen.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gicqhlfgq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gidwhiage.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gffcunrmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gnzslxwdy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gsyvvnsbx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gliutsgai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmkddwutf.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gwajnqtlk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gqmvnnhlf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gxzaesnhf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gmqncmjbr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gohjwwbuc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gbihnzscn.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gphiufoui.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gaztwqdje.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gucrqenqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gyvvmcbed.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gragzldix.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gxcesxcqc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gzmbmrbhb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/glicdzulc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gsgipkwae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbfkkieum.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gcjjdczdo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gcaidtjts.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gqiktpyoo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gnkvoiztl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gwuyppdet.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gywjqvbsu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gulqbcwud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gggacdugd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gitvqoldi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/golkammfr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/ggvuykwdj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/glydwajzp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gleeqsgvf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gempwjhop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gzcikvrgz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbcsymgvi.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gyclzmfck.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gbzqpdogl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/glcbevnvk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/ggagaszov.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gwvbwzjer.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/ghbcyegxx.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqytiryvt.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gjqbirvqv.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/ghpktlrez.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gspyntcqa.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwmnrodcz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gqefvyjbg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gnqkcsywi.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gacmkzrte.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gglefueda.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gvtcgcanm.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gdmrldrlt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gprxirpqb.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gczjljjem.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gubhtvxsh.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gphyptrnv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gpiifizgf.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gjpaucvju.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gtvzmypui.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gxktrfyrt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gljapixyo.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gajwswlrm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ggdwwzklu.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gpfkoqbko.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvsgbdrqp.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gkgzbddlr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gghsmcsbx.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gjarfazvn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gttetbtqw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gjccwjyte.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gkfwujxxm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gubuxrutf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gmjrsunlv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/ghiebiypj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gdpmdsasb.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/girbpbgsg.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggusjepbc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/guncgpdud.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghnirmpbv.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gtqtetxyf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ghzhfmdmq.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gtxylekle.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gragwmifd.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/grxvvlluc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/grqjvdxfz.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gqbteatcv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gqgayumiu.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gfwwuicjm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gkbklegbi.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/glduuzgne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gcynavhzn.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gkimnmlji.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gaesueuse.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gmxyswyba.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/grwuzfere.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gshepjsif.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gpusslhcn.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/glugqimgd.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwrqmkbmz.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gmognxczn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghozidxye.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gwxxdoosy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxpbcwnqj.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gatbzezak.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gavtgrczo.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gwuifhhlc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxklzpmom.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/glkgfujcf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gisfhezen.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzgexmohu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzsbumsdw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/grkqysozb.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gpdnzryyl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/giazppuux.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gcmhxkoyo.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/guzngjewx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grbzolzxa.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ggzqnuizq.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gbflkbntc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/geyfuubyx.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gtxzwwbhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gztpdpjzd.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gpanqutcd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gzdkotexq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gsqdzftaj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/goevxjwya.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gjqlnevkj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gydjlrbww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gnabcrfrc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gnrgpevqy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gvljlfkld.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gdbxerhix.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gtitqeein.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gndspuoov.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/guaedxuij.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gojfzkphr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gmelhvuzm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/grkhixrlf.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gvhleocgf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/ghxxlonlz.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gnzpzetbc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gypuvmjza.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gjoeiqluh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gapubnihs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ggrmuxfrm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gemomrbtz.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gbdkifqzd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gwaygbway.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gcwtqskuk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gxirsvkyq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gbwpoqbxc.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/ghjukchza.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gelujpsgy.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gyugsfuzg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gihmzgouk.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ggfsghppm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gwamiedgj.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gctthukia.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqpzidlia.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gwevljjie.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gdjinqqrx.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/genlklcgo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gkgalgbuk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gfeynhxis.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gxwglegbj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gtzeljfzs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ggkrgskog.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gfikonwhq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gkomumqqq.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/guoaheasp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzogrvnvg.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/geymzprtp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxojeazew.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gfpkxawxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gmprxbzki.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdrvdzona.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/golhqagcv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guyqahfvg.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/golqcvqmk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/geoxcpatq.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gaucuhbjr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/givoglcju.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/glcnrqfko.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/galyzrjlp.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gumgthgjf.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/goxomzdco.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gytvrcbsn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gmkzcgemm.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gncexdcdi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gbiljrpff.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gqwaogjlg.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gkcufcdco.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gxvrfraox.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gsswlsipt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gzioqcfpq.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gmbsdrjne.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gppvrbypu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gjiobnvdj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/ghhtzwrpv.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gozvomxyl.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gxfrgmjvk.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/ghdmavvau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gtqorosec.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/guxevltlc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfdtkkjsw.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ghddckcvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmutelfww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gjtrdkslk.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gdhiveqja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gwgbheool.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/goxtuexth.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/ggbslgfct.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gjpjmqjdg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gunufxhpj.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gutnjcgwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gjwaqooyl.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/glynyvnee.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqhrtxeqc.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gxtcmhmnx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtkylfxdd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gjlvqpdgt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcufpncyq.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gsmmwkksd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfrjipvup.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gewtmpqdo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsivmmfho.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gabawdfjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gmkpcwaug.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gimbgkiyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ghhxcjshx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gubgeifwy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gnyjqsgvk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ggsptgqpi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gmgrmbbzy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjljxsohi.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gjykzfvzf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gbmqjcnqp.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gcbvetwso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gruoxnmbe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gemqceicr.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gvllegaum.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwuxsbwe.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ggfpqxibq.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/goyzdjpye.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gejiwzorf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gaczndlyu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ggjcewfmf.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gggjassdx.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/groflskbd.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/goppbeptv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gfriekhou.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gwbdxnysi.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gikswfoxg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gefpcoutj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gqjmnqeou.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gydgybmws.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gamrkskia.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gxbbqjtek.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/grwlkuhqp.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzyvtbizs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gugvwjpey.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/grqqzojbt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/girxbxwqz.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/grtfvwhjg.sHtML


<!-- 参考信息 -->