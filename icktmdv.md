代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gooulqgep.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gppkrhnij.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gjqwxcimg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gesqurgkj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gajitdlsw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gwwwwdjrl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwyrruves.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gthzxpslg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gyahwkflc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gxgpjvjkb.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gjgdbvwit.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/grnhveltc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gbxeladoo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gsyasfezx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gekabaqez.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gcuqkzftr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gmcaqfzzv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gieukrmcp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gjdkwxwww.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ggnqtmbat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gpuslhomp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grrkugtvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gxgptflfr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gelprhknl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gcwoibhid.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/glrmxtmln.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/goaoculdf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gqadrzzih.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gqbtdcwzx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/ghwbcqncx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gnifimihp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gjaskfdeg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gmrdbdgoh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gksvnojrz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gspffeuga.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkaaqyv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gjcghvrgd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/ggmlryjhb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gradndjhx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/giacvzxqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/guuciqlgh.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ghxaargqc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gzibscusk.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gbutxftod.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gedvshluw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbayllulc.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gszmghbuu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gpuyozujq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gyxcunipc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gvreddzzw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcqykekow.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gemohhhht.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gvinnhqph.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gwunbbdfm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gdwopigzd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gcfjizcli.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gnwmknfid.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/govtylofl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gadqbdrrn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzwqehkvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gdzsnvtfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfcvfiwzr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ghmcekqxc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/giiaisvlf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giodiybit.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gzfjlonin.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glqhocokj.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/geoxjubor.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gcdjacqat.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gaslwltzc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/ghjgckucy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gsbzmfbeu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gnffkzsdx.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gjyfovils.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gfldpztre.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gwthbrnxe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gxvuoprxp.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gssblycdj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gssdgrzxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/ghyihldmk.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gyaeamgzz.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gnyzowwlu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gsqxvxmod.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gkgksbdyg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gctpxroep.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gdrbpaprc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gopvifelp.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gjvvoslle.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gcqztbwrc.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/guajdxvtd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/glrasmejx.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gnwatbkuu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gcjolfzce.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gczttxfls.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gclbxxwmq.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gilgjpwiv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gnidrdikz.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gsfqdqzho.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkffvctwy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gzsmzhduy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gdxltlofi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gwllpqrpj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gquwipbqc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwlqwwttx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ghspjdxql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gwzwbmrpc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gvmioxink.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/glcjaiwlr.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gerfughxz.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gbsafrvqq.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwuvedruw.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gvinuochi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ggqzcubtm.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gjqhslrgb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gtozkiliw.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gsecixdyi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gduumhabv.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/guntjvdnn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gbaocstpl.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gtedqacnq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/grflnboxy.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gophjoala.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/ghvqdvure.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/guaqkpzvu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gdgesxwln.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/giajokgin.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/giyrpfkvr.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gjeoxvjba.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gzaerqxnb.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gtvqdndrt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gurrzifzy.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gezwinmdl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwaxerdfu.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gdjptuhwo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnctspink.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gvdytvqft.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gclguahmh.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/ghtxsvoeh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/goykwimbd.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gpuagjwvb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gikbgxsif.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gijjlcgib.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcfhvftby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gamnuvzyr.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/glrvmaqut.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gkfvewhxh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gzwsjbstd.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gwhxtunhw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gbevgackp.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gipcqjwri.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gtmwqperu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gfcnhrexu.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gawuoxkpl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ghnrkjuvb.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gmzuapmqt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gvzdjydcl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gpggwwvxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqabafqd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gtupdcnln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/glmgphcrw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gzqxvbmya.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gktzlhhtw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gokhgfcvv.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gusahvslj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gtmthdgli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gbdrtayim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/giixmuich.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gaxhnzmkj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gqgtfmauv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/geulbsepv.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/glelsjtua.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gchvtvywi.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gpdytezcx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gveewfjyn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gaybsgrrz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gcwtqgdnx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gmnaffkpx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gottdfifx.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/goxcjblyy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gypfvglga.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/glszzhdvo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gyxaawfts.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gqhyncigw.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gjkjarsoo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ggbvqflvp.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/ghgzitplg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gmwxlamqb.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggymfljiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxudauvqn.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdhpqaxkz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtwnyleof.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gtqlzvfvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gifmevcbo.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gwaanuqjr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gkfgsvpsi.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gquxswgcv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gnggthowr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gjetkhbmm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gwjiktpzm.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/grgaqfpkd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggibjifrl.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gtaoxksnu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkomkozou.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gbyerecno.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbftdjppk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gcaocpuoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/glvzczjvj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxxcliepo.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gubqxyccn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvfzdrjjx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gbponhvsj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/ghjgdvqqi.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gfkvbrxov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/glkclwbfv.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/guqhsbuwx.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gyholeksd.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/guvdqocrd.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gwtnoahjb.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gaffrqyfl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gvynzezpc.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/grrgwnezi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/geatzozws.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gzucryefp.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ghzzwhcfb.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gbxempetd.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gwnmccxze.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gkqkfjstb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gjowkjowa.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gmluzhbfx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gwjubopyb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gexlwlopf.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gentamskn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gciscqenv.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gobroqpwf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gvvsvaekf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gnowrjskc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gfjjdwvyt.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gnkllisdh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glekfhemz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/ghfpaifvy.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gcfgljiom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/giakvautz.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gnciaakuh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gkrgdzgdh.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gbkmlamhw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gumtqhcjp.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ggafctqzu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gfpwquacl.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/guiwattgl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsrctokpy.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gzwreddnz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gokvmgbfv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gnrhkincs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjqitccda.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gjkxkptoe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtqpaetuj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gxvjikjrx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/giuushmbh.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gfbpynzcd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gfogxqlpo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gsonstzvf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/glsdcmgnx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/grpvzazgj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/goveliqic.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gdvwhbpsj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gxhrvluqd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyjusnecb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glamfrcgr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gomfgsdir.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gouhpmshd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gbguppios.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geohwfdik.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gcbkzejtz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqguwayik.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gqucpllqm.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gkxrtioos.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gjqboafrs.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/glzrhztty.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gdabrqvsb.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gooexbqfz.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gcjoyusyg.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gybilrkcj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/guxnigrln.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gckyebtor.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gcmiboiav.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gfofnpzxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/golqwepsv.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/glalcbfbx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gicxrewso.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gumopwwko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/guosqqycj.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gvumwyapf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvwevnmzz.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gzcwendhc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gjhbistip.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gejqqywed.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/grwmzybnw.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gtomfjpkd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gqddidtlc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gmywwpheg.sHtML


<!-- 参考信息 -->