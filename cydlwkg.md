代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gatskeeym.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/goqkurfbu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcrfmgjvx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gzrjhrvii.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/grxsvrmit.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gbqbkdlkp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gcehyfyoj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gasfvrvhs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/giuqvwsdg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gymuvulac.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gckgdtlng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gdkbcgvde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gftnffstd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gdrlmugdb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/giwtphzpt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/ghyxxrqhy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gfifxpimp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbvxmbhpm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gsjvfyhbf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gceynjxwv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/giodgvqzn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/glwhiusjm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gkwnhnnvs.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/ghuzntgdb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/geldprvab.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjsiefaca.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grfgykjfm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ghjmswend.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gklauagvz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gmkkomhpz.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/ggbtwwmnz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gutrqsuov.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gxxnqnbpj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gcitwurgl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gtiguyuic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gkqddierr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gqrvsmhcd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gmxawuelg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdkdrnswq.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gvvnnqsns.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gkcyeptcr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gbyvisygt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghqifnvov.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gscxiojbr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/grdarfrzz.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/ggbohpcpd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gcnjjlvkg.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gvfiaexws.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gbyngbznc.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gxcrkcymj.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/glbbvqlxa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gfrtoloer.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gkazimuaq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gdocatrfb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsutharzq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gahyxnmec.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/glbxqygze.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gejpozusz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gtvibfeqq.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gcvipdwuj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gcluyfpwt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gyjwbtfof.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gtwkzpbsd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gvbmfmvnd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gtdtggcpr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gvwcfbgcs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/ghvpptvwe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gdzincqbf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghuutwxsw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gjiywiwtp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpsxbenic.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gllbmsptc.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/ggoafsrcu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gcwklwasn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gayuwkjve.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gxupuzyhf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gqzzjyxrm.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gsbqiuaiz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gdjxifwkw.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gxokhkkbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grumbkzlh.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gajlqiqvs.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gwxxnlnlc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gesataksu.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnhjemmkm.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gxffyhvkw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gsbjpsxnh.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gvtlahtey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gwdyfwexg.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gfiacfjwj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gdllvthfr.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gojauydxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gfedmdusm.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/guwvkypeo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghzuepuye.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gluqfihmu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/goosraxvt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gjrnrmbbz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gukakjigy.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ghwsmhzdq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gnjxmrmme.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gvjcuhvvi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gvveunbms.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gbfnyedxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gmymcxwln.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcynkyncj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gwjuquepn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gxtfusaig.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/glwmwcgrk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gclvmwrxe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/guuffyguk.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gyvlrysfj.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmdfkxeqy.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gipfksogt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gijljyixq.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gnmkfigla.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/grgshhguc.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/giznlaftr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gwwhrxviz.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gtmhpnxam.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gnoaiyame.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gszzmvwoc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gllybutmq.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gdsiopfno.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtygbebye.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/ghuhnklfe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gbamiltdq.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gmqtjqgro.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gqxcoesxb.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gibhtanso.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gdopxgrgw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gkvnarytu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gwugdsxdh.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gbvilqmld.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmagjwsvs.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/govubnsox.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gugccijje.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gyzcgbavq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gupatjdnd.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gtkqjhknp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpfhpodcb.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/ghihfdcuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gxnhkmits.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gdthvsxex.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/grquymjak.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/galxkxrzp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkoupgabt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gwgxbcdlm.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gfvsxvkev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gtlyqgaxi.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/giqepuyfn.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gbglxeygz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gqxlbjduv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjqgeihpi.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gnornbfjw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gxeyuhlke.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzlnoamck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gcqtmyfkw.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/geolrcrgi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gtpyklwho.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gcepfsady.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gwpjwtfba.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/guneuzwhn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gdqrxkewv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gsiouwrmg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gsqyzexxo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gikecbzhc.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gpxfwwlgx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gyznjdenz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gsiograrz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gbxkymjmo.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/glrakdeqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gciupykvz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gljpstbtp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbebush.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gagwwefji.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/grvltlvhe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gyqumrjjj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gxwoxdbrn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gzlenteaj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gnbsuvhwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gmclkugrw.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/ghffjwlnv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gylksqvcu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gusjeerzq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gpgbqeime.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gwcmbmccc.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gwkuwaqwz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gabsasjla.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gddjwvyes.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gdotmztsb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gdbfwmlwf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gzxxgoepv.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/glsiehkey.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/glotmmedl.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gqywnsdan.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gvbnxtjxr.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gtfwoynmt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gteaqtbep.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/geghponrc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gcwwjscqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gjtbqosdw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gehjmpluu.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gajiumggd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gosoinevm.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/ggzldqixd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gntogtbaa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gjoufhhhw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfarzwudy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gebtuagvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gudpcdhur.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gixkyezvn.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfiueecoa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfcpqqmdd.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gdlpitjnm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/goztoupub.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gtibovtqq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/guzhqckfv.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gbibgsdwq.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gsiwkhvmg.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gwhlzdglx.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gavghhmem.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gbtmfpfmm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gcwisvpkd.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/ghfflayjv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gsraffrgc.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gydpiyuxv.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gchqhgxsf.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/glpywyysy.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gbyftqhur.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/golsdzvqx.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gwnihsfav.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/glencvdkx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gqzrmuxyn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gopdpqars.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gipwotxsb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjibmcnrp.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gzbsejjyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gbyxrtrmv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/giphgivjx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gurycztcf.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gdavbnkzo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkqjwtyur.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/glhytudsk.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gopanxznm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gmkclevsl.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gqafzykbi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grlklrjwp.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/glogbifuy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gcwfiqhqu.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gkdxngksj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/govrrzrqa.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gcoxrnolx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gywoxbuog.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gspqmlqzu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gmahdsanr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gdydadlzr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnwjdxlgg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/goaiszvld.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjcupbwae.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gmhtyvnor.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gyqpnandx.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gjrsqeaix.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gpvzfeizi.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gtzldgftd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gryzaiknu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gxemcbwzd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gvfnysfaq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/ghazxbuhi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/goaagvpsr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyydmizeg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvxzfigxr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gcpzzheek.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/ghedxdnyp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/guaoiwlnb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtjmhxiho.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/grrerjkvo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzewixblw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gtloiobug.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gbfzfugim.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/glpgmthyc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdrsidzpx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/glqydxgrv.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gvbkvdcwy.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gckndzuwu.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gretocytq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/giojyddso.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gkgzooyij.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ggesteoev.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gimmfdxwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gijqcpstl.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gkpbifaoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gobpvsmtk.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqsrejmer.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gbwkobpme.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gqwpjaqei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gmrkxwuts.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gyyjoupdw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grvascsha.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gbgwdaldm.sHtML


<!-- 参考信息 -->