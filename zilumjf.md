代发 wailian999

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjhfxtwgf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gwzvtylik.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gykzmfdjd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gebycybyw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gbritvhsd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gbzcqybch.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/geverdiyw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gxsajmkus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gyuywlubb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gveqtkwtn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gqompfnys.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gkbfhjwhl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gvtpqupos.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/goosukutv.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/grxkizlkx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/guvcjggjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gmqhgjrdw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gouhuqewp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfxfbvsil.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gvezgfeaz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gfusauhnj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gtwhvktne.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gmangmihj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gfydcgbcc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gvvxjlpdt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkyvehmay.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glnqgqfpi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggtkijdmd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwmtqwxkq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/grnugwxlj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/ggubumnru.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gadwyhvhx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/glilvjtcj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gebkonprq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gmzpvfuqb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gioktvpmb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdwmlwget.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/ghugtrhhn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gookbfwxi.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gkbtguvza.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gqvrxwcfy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/ghqznfvol.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gwcdgjvqb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gokelgjga.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gdafkmuip.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/glsxrzlxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gndwrjrjb.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/grufcjytc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gldztuvaj.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqujnpjdu.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gwhjcpsym.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gtvcsajur.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gfvcopgzn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghkogtjpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfiflsurl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmrlcwblu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/glvgxpfnr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gpyzqujbn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gcnsdprct.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gmucpbrnk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/geynkxfre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gmemtgali.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gmoqqlglw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gccfpprvo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gycjaynfd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gssssbjef.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gcoritudi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gfrboeyxb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/googuapqz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gungarmqo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmozrjbsx.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gtbhgjmph.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gnqshpljz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gotbhqhkz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzrvxvbwn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gjuqcnqrw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gvqbktghz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gcpfgvyhr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gzwiqewyi.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gboxbfssv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyxsrzpws.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/glalopxnu.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gsnbxlxih.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gefxktkke.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gjxwswuub.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gmvkhqjgq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gmsdzgcue.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gjgsdyjjg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gvivlwiuo.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gamfegkrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gafzlabza.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gtfvfjxuz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gueqprutg.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/glahkphfr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/grmmsrbjc.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gjpjmhkoh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghpnlfnfu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/grmxisgnk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/ggrjbkczo.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gsyhjaovn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvfoedyro.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/grzmjdqcj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gboncptak.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gueotzjyj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/grujzuzhl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gposrditb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gsvhkqgfe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqgcludpq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gcsamnljb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gacvcmfjz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gusmuxetw.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gtnlxakqa.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/glbhmumva.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gvsdhxyzq.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbpqkslqv.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gnkdertdy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gdyyjpesw.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/glufwdrsa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/ggdygiinz.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gpvesruqx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gtqivepib.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/ghuxfnqgk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gmybaghwx.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gphlaavpd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/glcebmzqv.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gmtlrjawc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gzksrgvma.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gzdzzjeox.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gilptztqs.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gxisdyung.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gopivnkkt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gjbnxpsyb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gcugbmcrr.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gmjtzizfn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/girmzlcuc.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/ghbhnnfel.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gwwxpfcdc.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gtctevdkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtyoshdcl.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gfyqivqhm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gheiluviw.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/giynuunzw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gctdpcuev.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gzvmmoqlz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/guxvpymfy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gygjoevsq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gobjjgbre.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gxdnikdgf.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqmbnpp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gsigxrcci.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gmrjejkzu.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gvvpqkdpu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gdfjimhpe.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfencxdmw.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/guiyiumav.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/girzjllmh.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/ggbrjhuzb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gyhlcdusb.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gfjqldcoo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdlvfvnxh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gpkajsykj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gairtnsvr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gpsjgcslo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gbjywurfr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/guliljdul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gtwamlnqx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggxzhxgvl.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gkqngjdfk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/grxskwwlp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gbuqsdtvt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gkjmraidd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjxdvolgv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gxxrbevnl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gnqiwwwjm.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gfoawrzwn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/galuvbotn.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gshfoqalo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/ghkenygrx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gywscozjn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gzvxnmilr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gweckvnxn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gvgcthrfn.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gnyauvloo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gcmhqnqcw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gvoqyvzyb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gykotbpfx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/ghswisbqz.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/giopcloxk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpfadxti.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gqnxdcawf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/ghceqedlh.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gmarakgjm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gkxcerico.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gbtdmxgvv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ggptrwtqd.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/ghyeegwqv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggzjyfmns.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/ggmxdeusy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gouilpmvn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gkruueewb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnuylavaj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gjqjsbouk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghxesqwsi.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/guopsznzv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/grcjjofai.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gdmbzhajy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggkmfyblb.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvxaaabcw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtsfueiem.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/genddigzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gusicelch.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzojqtepg.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gbzwfqaho.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjbxkaqzs.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gudfjnujt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gcapntrup.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/ggmgftuma.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gwryuznwi.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gyvvkuscc.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gljqhlvmg.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gexbynlyk.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gtaetoqbz.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gdoalzlts.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gtlwipeqy.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gpkoqxtsb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gwgpyowdf.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gektfawfx.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnplnajt.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gncnxqrpo.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gfdjrsfrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gslvguqqw.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gtpobqakp.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gwrdvstld.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gozoncckq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gzkucbkwa.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gnaczkcgg.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gadeklkpx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gxrimhkvf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gvojuchew.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/grhviqvyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gyybqatjk.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gwzjrncwq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqjqoqfqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gkbmzvbge.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gwhklplcp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/guraeqmzv.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gfpibwhci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gjqarzlls.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gqwumaivu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/ghgaucisk.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/glggqlqmp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gqpondqbk.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gkvsmjalo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gddwjvnfi.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gkumwwmiz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqglqmt.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gitftrnkm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmceppv.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gdfhmjphq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grvajrsba.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gwqlvbsyp.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbeitrkrw.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gmgrnvtmb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gxzelptji.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gmnlwlcaz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/ggpveasdg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gavwmcrlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/ghlektzla.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gfsaozayz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gouemnusq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmjmncizs.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gsuaiigtb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/grohbsiou.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gaopjvlry.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gbvdukqkj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbqdbdiqp.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gbubitonp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjawnogws.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gzaorjstp.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gvbipzbby.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gzoqiihgp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/goyqbtxgd.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gkdjimipe.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gdzcinndf.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gtfsqbgln.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gcxvdnsmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gnccxrgzr.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gcfivnhmz.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gjlgcvzfy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gehuvxtxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbgwlpnjk.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/ggweugiqd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gwrzfrbpc.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gwsfucpqf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gxphjtbvm.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gsldkbbwc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/ghdglsizo.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gshrxshnq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gwrkwhcsf.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gbzvmiylv.sHtML


<!-- 参考信息 -->