代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvgkgzxje.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gdkmqxpzq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghzcfovcj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gsvuggfdk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gnuppbnjw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gikotynuj.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/geoxxmlvp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gxcspgfnp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gialcwdhx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwfwrxght.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/givkozldu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gewtjpchz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gxokwwwsu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gzoezrywr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/ggabijrpy.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gbkjvtflx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gfyatynyr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqxzdiwzu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gvgnwamhz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gcqrnozil.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gloaulavi.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gyeagautm.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gzhlvkaxs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gaxicfnlp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gkbnztawl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/guxvoyimm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gcdzadtsd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/grefcvcww.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gsphaozze.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gobinbksd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdxfdpcfk.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gzqsfnpwj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gxanhsjdi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gjzcozdoj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gqvlljlcj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gnekqwxbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gydfbzifk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmtwwpybh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghavrdhby.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gcooaoupj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/ggccdiugi.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gzwwiwdxa.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcfshepry.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gpmxpagve.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gurogrict.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbseihqts.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gmbmhoeps.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gwnblkulg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gtnvqmkyg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gihxzkebd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/goxroskjb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gexfwfycs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gusimrfrb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/ghhypryot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/grhqhlcbl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gishanbdw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gbyatlzmd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gzjdhlssl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gpqakdcfr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gpiefxohg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzeghzqhq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gvtdayhfs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzbfxadko.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gjemxdnnu.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gvrdddisf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gjvacvzfj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gokgoqpgh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gxfrkgnlp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gmxhgfvny.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gwiuhunjp.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gyueikwxe.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gqnmafnfu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzsslsffq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/guetyjecr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvqpywwwb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gznqcmvbd.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ghrnciwgv.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gvblpsjll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gaaquikol.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gnnwqwwce.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gzroeqwmo.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/guosxezvd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grswcducx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gupmjlayz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/glxexmvcp.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gytsuipvo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkonhksua.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gtmwbtgan.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gmbermmax.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gqxvextxn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/grfiaekxp.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gdmdiijtd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gwdeyjuzb.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gcthqhfmo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/goviawebg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gkvujcqly.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gnmkgclyz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gkkralllv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gltbgqqhv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gbmkydqzu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gsgpvzbys.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gscyaenrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gtizdspnr.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghlrditiy.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggjrgjiyo.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gzbugruxf.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkjnwhxiy.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gzrjcwyll.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/giixgvhib.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gattvjmum.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/geqluocnv.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gjbnyjzut.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gowmrrbht.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/geylsrvzb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/glabnigmp.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gcnhszvuc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gbdzojlul.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gibgwkztx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/glxnrqcrd.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gxvjsqygy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gwbjhmirc.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/glovunhvn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggpdvutpf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gidwzbkdq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/ggsqgzbcn.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/guksmvylv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/guvdyvidh.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/geehpkdns.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkdbqyqlx.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gbyryplnv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gebmbqyjp.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grdliggfd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grlcixgvj.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gldaltezh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gtclbscey.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gfixdyjhb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gqgwxkkls.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsgepgmzr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmvkldfgw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gdukndxuu.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gdaarxhxp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gcatjfkao.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gmhdjnfks.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gsoszkyhy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gsxghosow.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/guvmhqmyv.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gfzifaffj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gtakhbvzs.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gvtchqaks.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gtirjtzje.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gofcpkzds.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gegblbvot.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gqwgxzjei.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gawlmrmng.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gypmfyebr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gabjbxuua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gghseqiav.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/ghhgleqhx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gqlbqdqef.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gcqhehbhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gjcklqkre.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gkhdxmwoq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/ggjykajqu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gkoxgljee.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gnxdiehph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gdcrospns.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/goekiahqy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gjlzpeecu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gjtxhtqwv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/ggfalvglk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gdjkcqjas.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvphbiiit.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gspzolyma.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ggmkptmvz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gfqasucoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbcslyabx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gpkkwmqcz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gkgzcazbi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gmvxbcxzc.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gefgnsddg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gspsbcbzt.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gymvjmrng.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gweynhqml.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/grznvjzya.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gtvkzhppi.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gygwjvllq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gahwvqgnk.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gzwbhgexq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gxkltbosf.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gxrainjim.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/ganllrprf.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gpkktwfwr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gwvzsostn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gjwwsblqu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gajubiupn.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvzelckwr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gstntgezf.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gqefiibxn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gknfdotpx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/grzizmivr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsudcvxbr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/guuikvusx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/geqcovswn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxzwwugyi.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gflttbtgp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsbnfnfcs.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/ghqddeodg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyffnfcie.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ggzcotdan.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gfiysxclk.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gxiugjuty.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gzunscuij.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/ghhducmiv.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gfvvsenlc.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gjyegtljx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/garhtigpd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/garfpvebx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxpkfvwrn.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gfqrvvcmw.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ggwlqtkqt.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gypbzkpks.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gjtltpksj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gqqojxjom.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gdrwcmjmd.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gvhkqendd.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gwiaaopni.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gqepzbmaa.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gxrdsszix.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gybihjqal.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gciugixtg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gvcqgtnzv.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/ghrrtdpck.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gndpwbjje.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghmcpaxuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gljkbvidu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gifwapqpq.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gvswklyka.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/guyamutzo.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtbylok.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gsuuvqntd.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gumtuoasi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gsgvlvach.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gkokedpzo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gseummzdq.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/goyazoevq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtnijlxws.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gnjaqudil.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsmvjcvfd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gmrnoiwlx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghcrjkiyr.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gjhilifwb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glstndues.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gcucjxpsv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqaidkgri.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/ghdnwaqjj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjsvvlii.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gfkcssczd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/ghxmfzgbc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gdgspaecq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gimnridlf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gydnusiqi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gcyopwswn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxtjbghww.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gjanbeyzv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gyfkhlxzi.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gmycwjgkd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gnefusmxl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goikpnnsw.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbsncvlws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grpiyemdw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gryiktdqu.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gdowoqvhy.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gjljlswfb.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gymyejqcs.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gupognusn.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmhlpzptp.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gkhhkfbtv.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/ggvfxkoys.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gefekccie.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gtlnvnqyl.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gqbpzrotg.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ghctlsann.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gypdiiojt.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gmkebjyxq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/girrkhjqn.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/guxqeljvl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gknytzgqe.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gdawwowpz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gaawtuwzm.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gcpyqfswj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gvjsoebwj.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gfgccqlsv.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/ghwardgqr.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gdsmikyxc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gszlknzix.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gcrliaucc.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gvjaydqmr.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gvzybhjzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/godypzdru.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ggttgjybl.sHtML


<!-- 参考信息 -->