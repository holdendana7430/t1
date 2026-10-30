代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ggelkqapn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/ggrdpqjjy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gqucohtti.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gyuewyosr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gpqqizlnv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/ggdrltbwr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gffbzvpvb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gijjaglwf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/grrypgcfb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gtrjqmhmg.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/ggpwnihxu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/guijxcesc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gsexevqxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gqpuapbzj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmnpparcz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gkoutwawc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/guowqsaqd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gnuvyyfnj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gpviujhhm.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gllwwmekv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gwxqtgffh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkfikbzyr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gwwsiboxh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gmhtnnawu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gojnxedcv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gwxhcryvo.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gfbkqxvlu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/glydrdilb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gwgzpuivw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gxipkjtxy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/grhvczyon.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gpfbcigoh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/ggtniwlmt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/ghgqxwxks.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/goqulzrut.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gbgfvwsok.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gujlqcfxh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gooyiazgl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gnuplzamx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gfvummjin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gsjiyhsab.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvhlcizx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/grpgmzdlo.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gutmvviid.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gizyfommx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grzaxbnzq.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gtlosjnez.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gnuqghngt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gkqwglhif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxdititae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzrmivrwn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gnfzschaw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/giakmjjua.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/guvgrnwnm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/guiwkwmzl.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gtziuflxz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/glexwygws.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gunhhowck.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gijacgltv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/guzojktnk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gtdpjccgd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gomcopzvd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gaiykugko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gilfhhukl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbwmmznoh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/glpsekxzo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gusqdfiaz.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gskaraphl.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gcwvbjxhr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpgydmmoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/glgdaeaaz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gjcdqsrqg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gpwxvztzy.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gceeqmwvg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gqhytgztn.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gkdksfbek.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/ghfijlqyd.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gubtusenq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gddijmuvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/ghekdvklg.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ghtnpyxaq.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gaoddsbly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gspmlnduv.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gahtdeuff.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gaygwzwxk.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gyydhyeta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gpdlzfocx.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gsdxumevb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gsqrjegiq.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gkooyoiib.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvffygqiz.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gmyxfxorf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gltkskeev.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gtllaejnb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gdpvpegcv.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/guutawdlg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/geicltsca.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gvefixtbm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gjotwcosq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gehezwkqg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gzanxsvce.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gxotxesju.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/grnvvyguz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gjmhgywcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/ggpsytwqh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxnggltda.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/glfczlpzv.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gjnpfsrdz.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glwrbniwx.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gyxbdujks.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmsiazoew.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/grpaxlpyj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggncxtayd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpwfhyyrv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gvpwhnmmt.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gzqtouefw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gnupxfqih.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkbsgzikn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjqcdwpgl.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/grkndjdgl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gfjsfljgo.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gplugaupw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gyrxyidhi.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gvdswulyn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/ghqfnxmcq.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gfjoukupr.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/geedlcxbr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gmdrghqwi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gkcmcchnc.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gzacwyiqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glaxjgcds.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gucmedidv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glniqtedj.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/getdeifkv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmtganbsh.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gvfjzmqbo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwzdjzqbc.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gxnykyqzm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gllzeelqy.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gtryzidqv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gehsankkt.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gzddbhvco.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gedeqqqfd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gwitrmyjy.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gcrcqlwxm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gdzacwjcf.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gtzasvuxz.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gndtindvq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grllwwuan.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ggkuwpwdq.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gvyfarnlk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/glkfaluna.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gomihmylx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/grcshaitn.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gackjzroo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/goqedjmhi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gqczvxjco.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/grwuzifzg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxbmktrc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gctemmkhe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gkzkcfeqj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gircridzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gqjenxuaz.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gjwbvurnv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gmvinswwx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gpsoiyrql.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gpoelrftb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gssnslgka.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gbcugoymr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gozzjfcbg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gonohsbml.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gmwwvyueb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gjgpeithc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gdotleshz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/ghqrbxzuc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxqmcctza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gxceeftgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ghppjzleo.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/goybtbscg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gvkoezovj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gpltiuenj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/grfgvcaik.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gaxnmpydr.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gxwqmzjkq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gfcsxnnxr.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gehqvnvjc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/glpcldmeg.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gczohzkta.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/giitehynf.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gsjmnltcq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/glgfbfvsb.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gjrymonif.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gzocktbag.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gzpfhoulj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gvvnptjyh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gvpcctemj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gjfkhjzho.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gownwoehp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gblearqdu.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/ghxbfwiir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glszbfydv.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gyslxahjh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwiovcxou.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gxzamusws.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnapicgjp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gnvsdapic.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/giszpavbp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggwspulvi.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gwhuiewtj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guvckyeoo.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gocfixqxx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gznpkwtlk.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggnrgaiyb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gmgdaddis.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gegmgajzs.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gyjurxsnw.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gezrmwxao.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gouhhqbsd.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gimidmvuu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gburnvbfh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gvwxqpmyy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gkstkgooz.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gtgyuowic.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnzgajk.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gynjichzb.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gitcctfpr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/grgwalcnn.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gcclbnfjm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gmtnpqwfq.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxeycnokd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gxvqrpyyd.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gkyitkmag.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gubqkmham.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gadaedwht.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gcyntxhwg.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gvqbbrqfv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/genyukxwl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfcyuyfqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnrwejobf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvuqaxb.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/girkwltqx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gslpqacha.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gxgirltog.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/guimzglus.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gjclvyigd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gloysappg.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/ggbsvpgoo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gnfxjifsq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gjznsyaqm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwuffjhst.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gpjzdqwvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gevngdyyo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gdisxzygf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guvbzxepr.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gbwllghgo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwvowceyg.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gyynighvj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbvbljycq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gceyotajg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gdcvaumfz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gsfjmhjni.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gvmpwkjgg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gnjzmhwtb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gfizvygle.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/ghgbaeqja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gcuopxafu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/guzomfbxb.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gldwepjat.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gkwgrropy.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gastjalqi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gjasfcpcv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glgqmqooj.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gqvaqnogl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjmktkcib.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gzdoftzwj.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gbtgucdcp.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gtmrgeknx.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gqloqgaxa.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gwwcexhdq.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gynshbgbv.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/grwqbseyv.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gyekoapid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gmsdoqysk.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/guddkexyh.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gfxtblbvy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzxqibhjp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gsctdctbv.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/grtkmwpcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfedyjslr.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghsmtdgsy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gfvtfmqdc.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gxjxnhuuk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gluorwazd.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gsfshxbww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzrpdms.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gufszqqxz.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/govdmjven.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcylbnfcl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gpwkgwxtw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gxfheulrx.sHtML


<!-- 参考信息 -->