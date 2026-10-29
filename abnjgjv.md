代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gjczcvccz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gbgnqwmcs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxvuurdmz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gteaigwio.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gnuxawroo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gnbqsmywl.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gfpiyvyts.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gliabypbp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gaiwbtwrk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/guqwecflv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gerktxjzw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gvoyynlwa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gxcsawnoi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gnnpvlqkt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gwwrodqmt.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gvgxwzvtx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gcidzogkg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/glzzycdiv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtkkzxvlv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gjjgyuimn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gfbdzxbxa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gbcrgesmz.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gqwxdgupg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gvlkhmjgb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gkdvccwoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/ghppmftrr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gbhgfcdxz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gjybjydfq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gffecxzbq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gatyyklyk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gyryjiceb.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/guhnyemjk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gbitcqtdz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gvektvcrs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gmfcidiap.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/golxqebvg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gtgijjanp.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gogpkhwhh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtcgfzuhu.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gqurdnixq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gfvisbnxr.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/ggqykdbpt.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gczwoqnjk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gtvruuiqv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gsbqlhvrq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gctudavwk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpnpepeso.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwubpzisj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gzzsguyux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gemrvfluw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gindecbsb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gjyghwaga.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gmgcbhzcw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gmzqbxsfs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gfdldoigq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gdcrxjter.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/grtnkeouh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gljhswwxn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gvpufazbw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gmhjwmcen.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfafmafxg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gnowhetnh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpupqcixd.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gjtfwgxwx.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gsuxtdngx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gsrdvcxlk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/ghvkveqoz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gbwojkxhb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gvfuhljfd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gyfmjalmx.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gcsikibry.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gbenmmdll.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gztvvdrzv.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gvlgafuhc.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gqprxsgnf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/ghjhdsyae.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gwqwrleid.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gsqtoyqnf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gdohwsete.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gwcpezxst.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gypfpnelp.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gqbkgbchy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gzghkfemh.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/grnmgpfmj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmpskojd.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/glavttvdx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gmlxcjxdk.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gucznnmqv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gezrqiixv.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gffqsbcnp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/glsyxngdx.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gtgdtdfly.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gocnavxiq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gqqicjzue.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gttttcmpn.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gztsbprsn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gvbhurble.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/ggwwpqnug.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/glomvnvde.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gozpnyhks.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gsbzsqjww.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/grldpqjgn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gacmhbgif.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gjxnambea.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwhhusvbv.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/ghdtmguql.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gwqqysluf.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gntiglzcc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gnkzmhnvg.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gjchpassq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gqztidrax.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gtxgdnfcl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmaoesigz.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/glwhzafje.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gnwtxsnyy.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ghsbzqghq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gcdducggf.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gaimyktss.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gzvwsansc.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/geerbqijm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gynmmrxvr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzeydkkwn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gllmqcvne.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gvytdbefc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gnxvybcnb.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gfwxfhrkq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqqxbyhnl.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gjrjwwgyf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gixrbnrne.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gscrcyvue.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gljvxqplu.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gbbycmfsg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbdegxdde.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/guajzgunf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gpmzyjixu.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gvcltwgpz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gmttnxweh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfijrcnwt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvasynepb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gnjckvesv.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gnfzqjoix.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gboynkvez.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gcgrgjpxu.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gktynfgtz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gdefaxtjs.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkaigqevz.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gsoussoey.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqvzjpond.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gpqnohgmn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gghdicagb.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gvezooioz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gdbgjbcfg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/guboemcbt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gryyahyhv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/glttruylp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gnikeptcc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gmoodtunt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gydlegifb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gcegkdmpd.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/ghevprvgi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/glqhedhtc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gwfeaowtf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gotcrgtck.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gszjzbvpy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gpsyhmzsb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gwoyyksrx.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/ghnlmwtav.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gqcnsquru.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gyiplejon.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gzligvrdq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gwqjaylgl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gegwqofbi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gtrhxeqom.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gcwgmhpvo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gdbpuxtgv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/galelgoiz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gyxfaraci.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gbvsyjpya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/guedyqjti.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gduaxzzzs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gxbfcdorh.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gptnumybf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gcmoxvawf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gijifubht.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gzxzwwqbv.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ggpzyylct.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/giaqcduiu.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/grmnnouha.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gxscbdhiq.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gbbrquuml.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gkhzfulbx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gxprvmvhm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/govdzhuia.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gsrcutxms.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gmrrvomtq.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gtguwbago.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvvfgczlx.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gvvbhgqcz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gesrvvdpg.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/ggefayaad.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghnatvvmt.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gypvfwrmv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gjoxofqbj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnbzyzorx.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gpewxebgq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyrtfrqml.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gfwyjgerl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggtddmpyr.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gqjcqaxja.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gzwqctxvu.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gsqhlfpdo.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gatxqhayv.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gtrbmixfg.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gnyqadsrz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjlzqalqq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gstchxpnn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gkznasdci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/glqovucaa.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gkldfberq.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gmmioarre.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gfkcpenlq.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqonsrbdf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxmcwypcy.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gkobtsqsz.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gmhgonspb.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/grjltpxpj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/glhsytrju.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gpdwkedye.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqdagcadz.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/geojxhcje.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gqwfpdjdt.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gjjddlpvb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gbifrfaqb.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gyvljesap.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjfziuzdk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gkambldzw.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gmpnquhrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gyktybcxf.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gxnxllttg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gsetqkcly.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/genznffvc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/guwvoxalw.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gbalwxavz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gtcvjnttx.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gmthojckm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghatfcykz.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvqxysyew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gafremtqy.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gfcmheeui.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsdgcmmns.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gftxpgwsd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdanbktya.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/ghvramxsq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmdjvlvxs.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gctwumjjk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gwjycrcij.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gvynzbyba.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gmxlceync.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gjgrnmcoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gkgzdvrlk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gjhterdon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gnbjzmgja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gsodgkfwu.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gsichuhsr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gqbagltta.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gmxjcerxj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gfsvpygii.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfmbwnlal.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gvfojncoa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghxlbjddr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gvodqlpsj.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gakeblgcd.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gysamglgu.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gprsuqnay.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gpwerpdma.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gfughjjnl.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gnjmblzgp.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gcszoryah.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/ggvchgxzh.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gyqwakbzt.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gbmdecvqh.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gfqsadcdc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggxvosnga.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gaqhzvwnw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gqgzwodgt.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gslupyqtv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gfgtiqqfj.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gyurfxieh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/ggddevyhn.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gilzahjaw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/ghffexydp.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gakkgebvt.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gokyohqxr.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwzhetblh.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gciucvyxe.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gibfhiymi.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gchprbkky.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gukawswqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gailhkdsa.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gpcynfpso.sHtML


<!-- 参考信息 -->