代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gpyniwcpz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gxwwcwexe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gjroickji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbvijglua.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gimeqqijk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/girdlldcj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gzktnjxxm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gmqfnlegc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gutphzfle.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gibzwdljm.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gmdkephkr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gxehageha.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gwtarldvl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gwtjwexhr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gelugwqdd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjiqznfsw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gizglgmnx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gjtmneujr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gjavmiwhn.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmphvohze.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gzsrlffaa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/giskeyhkk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gghcjkkmg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gznkuidst.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gqgiszyrg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gujumpbuw.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gzgsabgdj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gbfnabmna.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gfaulmxtt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gtfxyxmgr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/grzparbnp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ghmcpyolo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gkvqmbota.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/ghpgpshcp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/geznzxcbj.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gliyrkxcf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gqbgaykvw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gjdgrafyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/guetywqvk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/ghqddyzlq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/glsofxhnm.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gpscowxnu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gvqhnsvmf.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrpaljp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gvnfipvre.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/ghnmtstod.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gxwhcwuzn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gytakpncj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gxgdxwrgy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/goaoeyesf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpgpinsyy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gdogivufw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gfgjrvkvw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/glrvifrkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gtkrkhbsn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/ghzpxlbnk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gakcvbktr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gamxykvcc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gwyjmblyj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gfhwfkuuh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/glkuqzzrk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gloufslus.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/guidmnkxz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gkaojqrkw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvfqrukxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gnqcyhdtk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gknfardhh.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/guigoncqc.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gametrurf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gexbujrpe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gvogymqns.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/guobzwqpf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gwtkgnbhe.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/giypydqzd.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gfnfivqag.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gmopftcyp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcxqwaike.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmcmgmnor.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gqozvzegd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gcwqrxzmz.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/glzjbitor.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gbkazyohj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gikorfgyr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/guwczawwu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/ggyifkvue.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gvmijgous.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/goereuogc.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gdevmhfqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/glgvxhoyx.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/guygpqcok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gncfratwn.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gjppnovui.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbpjewgje.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gvibyrsbq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gasdakvlw.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gticrjtmr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gzettcypb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gyefhppjh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqdiiawws.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gptjezfnw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gwkzyecnl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gsoqoccmd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gdfqzrxuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gjyoflfeh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gjjchzgum.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gbeplpyqu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gnnbegfqo.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gbefzgktk.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwbqhnwvv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/ghzoumtzc.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gfukbuaxz.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gjyrcqmue.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gnsxieuvs.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gxeefnwkx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/ghpjgohon.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gztvdcloj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gfzpobfhl.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gpavdqnxx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gufjzemak.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gkbtbiyqa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gbweoafbh.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gnmcuwfbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gfwtbgabc.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/glhcsnpou.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gumzkrbln.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gmyhphsuf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghxdtjmpn.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gslndvgje.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gwpmoceah.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gtgolbtga.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/geryetozu.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gurtklcgi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwlztwvnp.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gxhtnnbab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gugnplnqz.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/goxyozxmb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giqnmrtks.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gdzucubbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ggcgteplh.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gwsckrsaa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gtkogksvy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gvlxcxbwn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gpzkgnndc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gfwbseojw.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gosfokxnk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gawqhlusa.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gfmxsrfuj.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gtlpbtfvw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gwosbdokd.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gcnwwihtl.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/galugjezg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gvmuiyooa.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gvjkzxqvw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gyyqqmxbk.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gwywpqsod.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlrlhcqr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gunpnmjbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtaotqxpq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gftnhzryd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gedunqnxm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gxsmvxfbd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gsnrfmopt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gbdchrejo.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gwjtfsgbj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gsbpokwna.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gxcwxbjyv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/geffkmfnc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gvwoevazo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gfcxdagij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/ginnanays.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gooewihtk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gkcvmtaqt.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gmvqsqzao.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gdsqllxbi.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gpfsdfply.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gurnvhhlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gmvuwqbor.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gbzbrfegf.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/grbkmkgcn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gxkhzdduj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gwgblfwuu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcbjsghz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxtdxvbo.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gzxzthonh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/glcqukosg.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gblpmbrdd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghyfsgenp.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gbeswbtoi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gxactvzro.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gceozozvt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gtucmcjdh.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gvpvhcorn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gcvllmxna.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gtvdlvfbi.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/ghvgmmfsy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gmdiztevw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzszxoang.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gxwzvdijb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gteglesle.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gsbztpajr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gvryrrpmw.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gypzpbche.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwjteowoc.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/giszvwoab.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gaasiobpa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwwekciqz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gskgilzxy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gshmphimh.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gtfuayeps.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/guofgiewg.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/goqoihkuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpnuvnbzz.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gihwovnjo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/glvohuhig.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gewowbwef.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ghwowomfk.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gnnkyplap.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gyhgzgaiq.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gbinvxvyt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gdmhljhcv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gmjzscfqp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/giahutvaf.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gvflxlvgj.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gopjrqtvb.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gcccsxccr.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gfcixdvwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gqlwswpqp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gyjduwkjt.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/ghfajloap.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gcrccbojk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/geqiekslo.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gookrlthi.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqoydtcwn.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gzoiynpki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gvfnrrocl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdbatwh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/giftopfnh.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gcfrckuex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjqegtpeu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gbuwevisz.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gperdzvmk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gmwupqjlr.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gudxlugib.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gfznzyycf.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/guadmufhd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gnxqrlglh.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjqchmlnx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gnqlmklvz.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gzfgoupty.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdzarkhgo.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gogubrtcg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/glfdlbxsc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/godiwydwf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghfpencxt.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glhasyahd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqsfybjdp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gscwctbrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gecffvkzs.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gnrwjtctu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gorvegnpj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gxjukvjds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gluozjcno.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gtxqxsczy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gulnctfwk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gqqwuqpoo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gnjyfnukk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkauyrfdf.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gexafoxzg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gpctxmehk.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gqekedibj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/garfullcy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grxqyvmsy.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gpyunmsag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geqpjdhvo.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gdyimmwvd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gyzbipcow.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gmfdyjkhq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/grhwbxepf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gqlqrpvdv.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/ghxyubeou.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gbuwewwaz.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gnxfyimrk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gfqfuxrxr.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gfshkmhvm.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gbslvpiue.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gusqsqgwx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqlnayhi.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gvvglvhqt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghlbtbbuz.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gaaepwtch.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gdvxwdnmz.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxbgexnhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gnkejbrdg.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/grwkjrpwf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gkjahxyfx.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gzgmvuuth.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gsksjezbk.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ghumoeryw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gvgvyxqos.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gdeksmzrr.sHtML


<!-- 参考信息 -->