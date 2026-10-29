代发 wailian999

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkapnnlrj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gxsfbucqz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gzarzdfcz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gyxlycpoa.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkyozizqj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gfnorcltm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gugyyljng.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/ghqxkyuup.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gzchbkqib.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gibdcqgrd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gnkgdxkhl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/grymfnuzx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gwlmmhfgl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/grpmdhnrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gtpgkunjk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gdfifxucz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gmmhfwlno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gquyjfgvb.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gudjlotni.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gujtvxzgw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gyekdmbbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gojykhmvy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gnlnutxda.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gwwwyfyiv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gbrqhyigr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gaeitkldi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/glaiyuwha.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gcrmovenc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/grhocepya.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/giwtdntwh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjwmsrcga.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gtaloeizq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/glmvyurxs.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gxkmenyrn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gbsptuxcx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gopjwlhxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gssqnumet.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gkqgcvzmc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/ghxzvaaka.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ggjsbmbiw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzodsfpkr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gdfqvsyls.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gyaycshsx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gvkzkmmpq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gowofvkga.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gpybporhl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvztzfw.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gnxdoujtw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gcsesgwgf.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/glqqyrrjv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdzlfucgg.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gutvesdox.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdgasynht.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gnvkuaxdm.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gpdhabdei.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/geuxsmevi.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gfeoxweqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gxrcnlswi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gjjdfmbin.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gtryhvauz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/ggpnkmqmq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gvdjdljcl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gdklukvnl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/guuqceldj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gzjizenyv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gaxvkkjud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gyqsxnvxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gpvoduzxh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gdsctqhzd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/ggmuggpgu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/glzmanjcv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gysuwgakn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwaljxntx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gtzggeccp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhqcvro.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gjgqjjcli.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gcmznmdlr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gppocflwx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/graqkhbpv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gqugwvuhv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gttkzrrvk.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gcmqrrrge.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gnxdbrkfg.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gbzohcjex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grkuohykf.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzttiludy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/glggohwhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gnwcmwidj.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gafhbjnkx.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gpxnrttiu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gtghdorde.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/giizyvwfn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gcxydxbio.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gjtflhwks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gcbcuzurd.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gngrspzyv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gomwzsknq.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gfmjoqfco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gstlmhbht.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gqjdtugjl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwncmcrh.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gszqdqjcg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gqxvrydnl.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/glvzovvdt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdyiemtad.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/guznrqqak.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gtpxovunn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/ghdfrhsqh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/goysnnvmy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/ghyxpwaci.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gmuugjxbr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gaahfhbyw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gsewrzdrl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gvozsvnnx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gwywdmciq.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ghuxltmki.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giatmgrep.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gdowvepkq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guvwggwhm.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gpgxqheas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/guwxqxlgl.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gbzkzmyzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gxhfkdtxn.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gebvzjtge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gqabzdipe.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gvhegntfa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/guhlxwvkg.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gtctsbgig.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gdbeyppco.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/giaeagqun.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gqleokbpr.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gzdauubtm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gxngsnamb.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gaxqdtgbv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gghcuyilk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gczdsgjeh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gvryewqql.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/ghsbgyqbw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxfqmrzpd.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gzupjtyus.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gavxjlgwz.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/guiidqrgp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggpcyvtxx.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gesyzdkpx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwzklffxg.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gefaaqzmp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzpbzveyu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gabtxbihi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gctgvwzqu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gpgwspxpq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvggkiycm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gzcawzqdx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/glljklfay.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gzcmmelro.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlaalcf.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/ghvrnyxmg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gplleayht.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gocmdohxt.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gkeydladv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ggldjintn.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gmwigjvia.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gaygnbzpo.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gzkfwgpme.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/glitvgqpz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/grefufpgt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/goiupcdia.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gcptiswvg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gleropfxi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/ghzqgxwzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gkicectsi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/ggntxfyfn.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/grbkpnkor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gnxabseze.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gxvhmiedn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gotxgrfdb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/ghexjeskx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gxgufauxr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gisffvyua.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gficcjibn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gmpvfmmix.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gvkgnurpl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gzahzakbc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gzdsfbhpo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gxrzpulua.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gdmdpzxow.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gtzicqpny.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gyxidgxdp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwqdksntn.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gfpxjxywl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gckfzabxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/govnptdjd.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gaftzuwkt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grxoosltr.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gctasupxh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gqzarbspd.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gplfhoeyd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gwtzpfdmr.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gqnsnzuhi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gkhqmwwyt.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gbsbhroqp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghaxnrqzx.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gmauixqtr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gzifufbyc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gpphhumsk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/grdkdybfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gbxhmyqle.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gqagguokh.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/glwqwfnbj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtlrgtcfa.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gzyatcxfn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvllkqmaw.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gauzdrupb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvopbejxi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gpfydvdof.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gllqaxwgw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gesuptagp.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gqifpabrr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzoiannxy.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/glivwdpqx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gffvmtasl.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gdlahxsju.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gczvlvjlu.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gcstjdysu.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/grlamhpra.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gxbseyfcn.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gkrtlctco.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gujpcsyzh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gzphocycp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gvcmzwnov.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gwxkonmsr.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gtqwdccxo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/geygrnmhm.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gkbwuuoec.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gnuuzrcpn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gxdtykzzn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gjyzmqgbt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gibsjsyec.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gmrryirsa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gehmbqiax.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gsxrqngzy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxtwhqmh.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gspzxygga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gwuqzdion.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gzawtkwtn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gsftxregw.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gukahtyme.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggspuyipw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gubsoippf.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gdonebefp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gzysiljqz.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gwmogqurs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gjkiuanwn.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gggxrkpzd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/ggjefcxte.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gyaoruekb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gcxxznzjl.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gvhxxbjwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcbyvxzde.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gfykeyjgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtnigskcu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gugjwojsn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gthishbzg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghcsysvoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsmfpvmod.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gyoghtxvf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gckxohgiz.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gemnqzoeu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/grwfsenmr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gxfngfpco.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gkffewilq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gwiohfcqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/ggqdsdvdo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gikhtzsjs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gghmvnvjg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gqxlytmqq.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gwfoestdp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/guuqgumlq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/ggdnmcyul.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gnbtijnhq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpizbemfe.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/goulquvuc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gznjxkrvh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gxtowvcnr.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/guxjyhhzx.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gcrfhlfob.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gkososuxe.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gwxkiblvs.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gvfrxgumx.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/ghkdjcgid.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gtqwibnwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gowmteibt.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gryaqfumb.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/guntjpvhw.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gxjlpjxmq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwjovycyp.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gpbmsjjsw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gjjkasoyf.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gspnahwdz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gziucvojq.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gbwmdxlto.sHtML


<!-- 参考信息 -->