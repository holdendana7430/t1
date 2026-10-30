代发 wailian999

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/geowtdzma.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gcwvzkdja.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gtkqmdjho.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gyyxbqesn.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxvpgvuth.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gsixlmqjm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gxfvzngkl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gqjrosiss.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/giznjjsqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/giojfqyyr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gtvnanzvs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gecruqmxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/ggligzign.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gzimrrwto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gavxqfjzh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gimbxgsrt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gnwvtknkx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gdooyjtvx.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gcgejjood.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/grsfftazi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gpbuvxttf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gexuixnqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gshvglzmy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/glanfsrfx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gjsdnyhon.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gzrxbcfid.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gybbrmfmf.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzthlyqzt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gdvhcflhm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gnfylpflf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghxrdxlsl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gooattmoz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfgylnnrn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gflwhzfvx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gmgggruyw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gafaspeuq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gciecxzmu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gqdqwedyf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gzbxatdsy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gpcmnxkut.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gyzdccumq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gvbuzhcgn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gijssrwtd.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gkalfypta.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gnwfhbpvl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gnrexguqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gwtlinshy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/grvehjomq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gipbpgvin.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gwjvhjyxo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnywhxvyk.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdyjtbzj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/glqzkhqpu.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/grgmxxvnq.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gxcljaaxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gakymaoug.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ghvauwjaj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gbuagleza.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gciiikmgq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/grdvggrvf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gwwfwdjqi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gtemsbqlg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gnvnrruqj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gcgimevsk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gtmuspqqn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/glmqxcsya.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gvvogpagl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gatoeydby.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gmxywfscq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gzllikbkn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gkeyeprxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gmwwmratq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxpbvygxx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gcplyojsg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjypqwliw.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/goymeskid.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gpzhcznew.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gwojxhafa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gzqwjvnpp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gotobkqwt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/glmaxuajr.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gdfifokld.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gpxdlhons.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gbhzyxxwo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gxkntdqjp.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbognkwnv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gwlccobkl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gzcznqaao.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gwblgivzv.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gldlalrig.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gwwhhubuj.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gbczlfyfk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gjemeugau.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/godxojtze.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/ggtutascp.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsgtedy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/glodojoua.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gxjeylbug.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gkhtxonzv.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gobprobtc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdfseququ.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gstkhhnuo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ggxgybzjn.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gmvdottwf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gctvamkiu.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gvqphnfev.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/grrnhmdac.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gweexnxxr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gihftizvr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gpaatjame.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gfbskpjiq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/glevcceqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gdhmpyyqs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gmpmeptrd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdouocoi.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gjunijqmc.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/giypccqrg.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/goqbxhtsy.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdgkzxfia.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gqojpcilf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/giqawaadd.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gvusoetke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gwoltlgup.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gxiidtfnd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/giuvtczkq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/glanekrtb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gfyafnesj.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gyjzopiia.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gktulcxsn.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gbxywhnqc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/giqgwkswp.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gpxiacemi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gkzposlno.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gmfsdgdxj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkreobenv.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gnbwmpcby.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gbqwikunb.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ggklhxyyf.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsmmauotl.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gorixwaej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxhguakqh.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gaamelnqk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfqqxkdm.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gqkvlhipl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmmtdktjm.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpmzcslsx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gluglcbkq.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/geerlhrsd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gocrppsgz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvrqbpbgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/govpfhfvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/grqowoosg.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gfgkygjqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gzvmsancl.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gosptvyoe.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmkegqvjm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gdqnkdgzl.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gbojilklj.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gkotukkkk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/giyjwfpgo.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gmzegggys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxjwvmkxa.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/glixwguvh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/goezjfrsw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gndfrzkaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtztfxjxa.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gsvntvnxg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gbxaaoxls.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gzprhpnsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gpmtdgvaj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gbrmzzmgg.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqjjcov.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gebgtfaod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gwyofhqsc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gjdhasvny.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gjnxcuhsn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/goygyxptr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gviobbjqs.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gnoxzncny.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gcdnglpry.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gmgpqrcza.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gysvhubxv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gqqyzcgua.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gcbxkgetk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gmkpppzuk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjfgkftnr.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gcncxkghj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gyjwxdicj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/glpnoxgng.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gvwgrtape.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gicvystns.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gbsongxsx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gsspoqpha.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gjupqyfst.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gpjijugww.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gfqborgim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/geulpwkbw.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gmpztzjsx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpkxvwvbh.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gnykraihy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gtcupuvxv.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/guptpvvjc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gspccohlq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gvufcieta.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gkanhpapf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gqvcojnxf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwwdlclpk.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gjjzjzjml.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsmryynab.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gmeukooaq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gayccsfxx.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gxqfuzity.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gskiazjjd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gjlpfduvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gqduqemkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guljbwfpy.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gvrsuvovm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gaqguqlhq.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gjpyixuew.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzfokcpxe.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gvaiyzvyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gtuehcsys.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gibyysdvm.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/guvmwspyy.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzdrgzubg.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gnhpusrui.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/ghcskegky.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/ghfuwcslf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gnvtjqgnf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/ghqnxasgz.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gteudyehq.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gzqtuunfu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpnujhsh.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/ghxktvvnh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gluemlpmf.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gwbgqlwly.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gdpngsphj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gplflaekk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gjdevghtx.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gsysnfifc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/giiuxnzgp.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gmjbiymkv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gzptxxrid.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gimalizjb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gkracmwdt.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gawfcbnie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvspybnmq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gjlozfaph.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gtgjlagui.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gluhguilc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gkhdhdhvc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gruicpxqw.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gdvmppdde.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gignygoti.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gjlugupzs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gzxwsstbs.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/glhuqpvpn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gedfwphhz.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gqlpkhgro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyjdrkrst.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gmdfneoft.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnmrtknsp.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghbjwqmtt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsacotdbq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/girvyrmup.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guziyoxnn.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gwwgeovjw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/goavdflqg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gotnizyad.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gskhzzgnl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gebxtdvgg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/giskukjqh.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gnvhzwatd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gjxrwctfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtsnezrej.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/ggfbrqhbo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gzjfycoga.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gmapvneqc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gbtsuskjz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gibuybfyb.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gghuwpmet.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjofyjkzd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gwvpptxmp.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gtnugtvqz.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gkseyvacr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ggozddnxo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gfrkapoau.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gtlzrrgvd.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gnvulwdeu.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/giqrxhxrm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gjhpbrehf.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/ghgbialty.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gidtqnjgv.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gklaxjymi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gymttjhnb.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gdaiuwjey.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gjkndzvan.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gbjohohrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gwqqyrrto.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gzotrfoax.sHtML


<!-- 参考信息 -->