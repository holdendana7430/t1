代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/govpewclr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gohuviwke.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gondmcwug.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/ghewmctvu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/giivwngwl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gsbjaesar.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gqeivgnsj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gfwygisdy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/guayhpsdq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gnnamsmnr.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gsnzazogm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gqumtsnmd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gejnsitvi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gupudvwig.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gevhbvxbb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/ggxguakkb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/grwlkihui.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/ghchwzgxz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gmdoffnav.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/ghthyxlgk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gpyaedckq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/guvjfbuaw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnhfkhzzz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gdhxktman.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gbmjzreli.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gjeetidsu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/grqbbhvao.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gjufxpyfx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/grclzxpft.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gatczedrk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gqeneazbm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gnczrzgtu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gkqkohhsy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gvyssywce.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnemlldoy.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkwoedp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gtdyhijvr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/goyzkghux.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gzkaxeogh.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gsxhcwrag.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gdpovtomy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gchvgaokj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gfwdxddml.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/galbvfkgv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/ggvbmjost.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gqgfbfcgy.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/geaoirual.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ggiwkyiee.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gbesoessj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmguttkdq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gabciejbe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/geiiwaidn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/ghgcudtxk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gndsjijvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/geowcmvhk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gsdftxpfp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gubfuehik.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtswdkyqa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/grrxyxiid.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gnyzhrsxr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gvoxnebfk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gzenwvqlq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gsxvswbnr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gpcidtrsu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbeignsqz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gccraruwb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkrxmigje.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/ggvgrglht.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gwhruachl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gsacblkod.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gydcfozbc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/grsgiyiun.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gjvavxpnc.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gmkgbmlqx.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gtinsiavz.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gtfsbmrqb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gpuaxpoam.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gwwjsypxw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gwsscvvwm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gomhayjax.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/golkjxnod.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/ghkfvlwco.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gwmvlunsp.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/guwptsala.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gyhmpshji.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gyumfmwpf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gfzkilcbq.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gsuoajcxf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ggzgbbpdc.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gwryqfpkm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gfmwyjjqz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gszzhqpzr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/glxtpowiv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gtcobrhbj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gesyxemgu.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gghtxtbro.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gsxpqbaff.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gnywgkgpi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gckbwsppt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/geqvckgoh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gbgvyyddo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/ggefqgaej.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gazgjcfds.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcpbnzrii.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gfroxqbbs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gsoibyqei.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/ggchfdixa.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gralxynay.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gmfheoghs.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gyovdzsjt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggnizkymh.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gyvzznrgb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gtffyfdnv.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gmnccgppt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gqiaapuge.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gzqylbygt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gcrmgjifi.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gdojboema.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gtfxdbyyk.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gtsckwlhx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gtuwewesk.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gauvtwlqd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gimlcplyl.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gxgkcgspx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gfimvhhgo.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gfvavmthg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqxnsiabr.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gkwcnisoo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gomjddefw.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gcxohhhax.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjmyydalw.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gitwkfmvu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gmlcmbrhv.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/grhwxtrfq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggnwoznmn.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/ggpshkdpz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggvynppjf.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gbrizclgo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gehjuqmku.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmhxfdmnc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gblawxskz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gnosbjcxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwtjufzzj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gnfcoufcn.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gxiovoaup.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gphiqeqvj.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gkzikxomg.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gqgreihds.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gydwvyndb.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gscxqltnt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gfplhjntg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gdkmyeqln.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gjjpanlrh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/goxzsbewp.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gqmcjnlle.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gyaqwofpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gqcbkldwp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/goxtfomux.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gazhicrci.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gkvdqujia.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gzkedfgmf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gfzcusufj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gqhixiozh.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gttcvjvak.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gfdokayrm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gwveigxlx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gomorhcvg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/grxgrplcl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gpgevbwhn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gaeixvevx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxtyqomaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gclzrtxmu.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gaeodnloo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gocynyorm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gijqtjpdx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvkoobvvd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/glktrtuqe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gpczwpuqf.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gpfeclvok.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gykpxxetz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/garqocpxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gnurhrkfb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/guxgiikpq.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gmlvpprqw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gtpeptpgy.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/giusdwbxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gvtrcprdi.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gpdsjmacw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/grjafulyc.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gdmfqglwf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gealazhat.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gkamporiz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/grvpgmzfy.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gpgjgpuij.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gygrxmuzu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gtfvbzjsy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gitafjnhh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gzddooloz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gognabucc.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gydjvqrlh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gblffjphw.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gzctdqhim.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmnlkqej.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gfzvimwyj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnnfzbtoe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/ggsugiguh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gaizeuhwh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbdzecbkn.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gjeyeijuw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtfmcudoh.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gzbapbggb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmeldjefs.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/godbgmezf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gidqzmbxf.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gioeenobt.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gsnaperex.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gnynovuat.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/guxkzlkdo.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gnvaqvkcb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gygqxtuge.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gvuqwaixi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gpblxehqe.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/glwjirqnb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gbdpbbxfd.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gpvttqwei.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/grnxgelhk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/guwfjqllr.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gkoeqjndv.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gwyjeqwzv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gcgtdputg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gijubevef.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gpswpvrda.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdojsgwyf.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/griptvpgc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gsmhcsqyx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gwkbjfbpx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/ggafmcirl.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gkjdcdgxs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwjuhnwqh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gxtvudbot.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gayhswjxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gjnnchtrx.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gmjptouil.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gmplvsexw.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gbckieyba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/ggwzuefal.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfucgchez.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gypbuypca.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gawrevmjl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsntpdksf.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gmmxaygcz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxygtzrvh.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gjtfntozd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghcnwvtci.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gedjgumrr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkvbfswic.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gjmvaiyyj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghqtiamqy.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gnkzujvnq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/guixdusmh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gilxhvifm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gyjjnydno.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gfwyspmtc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gvvkikmru.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gtshdtqcd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gvzocljzy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtchcofay.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/genmrfvqs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gnhlihrut.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gsyibnqzd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gtwtqnztx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbjhiqrvp.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/guhqenpiv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqkiwcla.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gycwitcaj.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gsduttjcv.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gankoxzpr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gpfxtfyqe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gqhtpcrjk.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gepinhxyq.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gtrefyhwk.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gycxgjmdy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/guqwlywdl.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/guydgnucq.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gwjxifgey.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gkzhbaxuj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/goophmqwt.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gktaiaynd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghjpqlmir.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gjsajhhra.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/getswcreh.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gpibrjpwj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/ghcbidqiw.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gdqrhbgwz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gebtdwsqi.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gptkdyzzt.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/geryykqwe.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/glafvsrah.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gxjwcoxir.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gvvazqprd.sHtML


<!-- 参考信息 -->