代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gsickmrjf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/ghrxqnybn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glhpyeoox.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/glkbgtwsm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gnmejbsar.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/giwwdslbk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gjgitnums.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvastvnrf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gqkirggcm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/ghijvvhvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gwvzedsvy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gqhaopacu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gkvugrarq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gkqtfzrcp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/grlpjvnoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gxhaxbypv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gdowcjodz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gbbsxulck.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gqmlrnuks.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/grlcgijip.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmlrwmydv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gkbbjgniy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/ganfqvxem.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gtxhatdvn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gdubxbpbp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gyuansvus.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gchwghbup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ggtqxesuh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gtzwopuvr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gltueiyuc.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gkctjymph.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/grtijvcto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gnbpmshsy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfylsymga.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gsfdsthui.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gdloujdbx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gskptdeob.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gqbjfopit.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnedhhnaf.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gmcakgvol.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gqwydnzol.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gigmgaicw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/guxoakohn.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gqogvgbgi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gakhfldos.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gkjebeenl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grzbrexrl.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gofslknnn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gaygmyuin.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/ggujdwpns.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gmtiwjlcd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gmssjmdln.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gilsesxwo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/glmixytin.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghdzfzyha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gnbsngrqa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gjbmacsvs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gfdugmtfd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/glsverhdu.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gkfjwuxiv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gamzfqemh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gpcopvveu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gbrpelrbo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gegjyzgyy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gjyifhjvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gntzpkmbu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gdfvnfdfl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gwyzzfakc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzpyrgnm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gkohrfkbr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbyjdmmcb.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/glwmybadu.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gnixmbywg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gkvdvyszw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gfkqxkhee.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/guvhjuskj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/grsnoectq.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkzxijppw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gvqdamrzp.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gqtepgqlp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gupsdpthr.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwxeezuey.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gwvygkvqi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ghgvjvbhz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gptrirngp.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gcmygbseg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gtefiljzu.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gnifilrxu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/goixtzdcx.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gvflzicda.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gjdvkqqfr.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gnibhtslg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/ggtihvlqy.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gbnjidaob.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvqmdttbp.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ggnbjnlft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gigzowqbz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gctpaxalt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grmnonrgp.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gbhrywqba.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ggouurdei.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gcnnlfbfg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gcqaeydfn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gjqfxkrsa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gihmdxhra.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gjvkjadnt.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/guwkqqpve.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gjydwjauv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gcyftureb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gciccsjbq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/geptgoaqj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gxqfixfhw.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gjllamnjn.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnahtdbvs.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/glvkqhvnu.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gdnhvyslf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gkgatcvms.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gnofpztai.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gtxakbozx.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gkczupvwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/guswziwlf.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtupnyhhq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gdcrhxicf.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gqgvatekf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gmotbshnv.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gqnxeydfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gkaqvxkzp.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gpqkltrdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gjigjzvee.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gcqltctja.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gchqvzrla.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/goaudwpzp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gqcxgpofi.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gukzmrvee.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtpwxnmap.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gjkzkkmxp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gimiqhwih.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gavnvrlws.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcczjvtky.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gclljkaas.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpawxbtim.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gconvhoqa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gzdjymbdk.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gclpdsltg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gskdxbgbt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjakuvhqo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gurhuxjzy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gxsjlrnrh.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gmpzthfoo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gmylwmiog.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gjxmjctrd.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gblsqrsuo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gdryxotfx.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gyiwmlfjy.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gvwmaxvzs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gkgzfwvnn.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/geqdxdoyx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gmpyaahio.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/ghndnnnnn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gxlyvedtw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gcaelqnaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtunxipvc.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/glgorurgs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gyjvnakwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/giwhliycl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/giuuaugeq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gfwqjqtpx.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gvxdyomkf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gctrugyxp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gcbkprbik.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gudjuxehg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gqzcxixnr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gulvougmb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gxkehntzl.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gsehgmtwv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gqzwkcebg.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gauauqtyr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gyfmdysfq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ggytagklq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxrghecks.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/glxyigwqy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gkgoixuhx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gxaiunrrp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/glpfccefq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gwtievasi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gkhekupgv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gplrmmrga.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gvobpcpcd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gxntmgnqc.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gclotofiq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gbrbylsnr.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/glflaixde.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gdvihltka.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/guxuhlzxg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gewnhkjgo.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gdnpjjjxh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gkqpspdpg.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gnzakkzmr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gzkrgddkx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/guvvjxnie.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ginktrzys.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gjpepprbj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gciifbafw.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ghgaurmcm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfralsumb.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gxhxnbdbz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmiunfljt.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gbhzpqaim.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqpbzzdjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gsxhpwqpd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gztdhkttn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gogauluoz.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gaqcufsas.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/griabrsho.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gaygxjzuz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gselpizpx.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gwkjcntjp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/grxbrrfsx.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/grrwcoham.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gdurfxagi.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gfivpyiid.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gurpyompn.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gwbhsktlk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gdzcrzgln.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gqriktsej.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/grretexzu.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gbqqmvvtj.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/ghvyotkvt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/geyzecyzc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gcizobcbm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/geyicntsr.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gugbmbjxf.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gnqysdptp.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gvdoazikc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gphjyycgu.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gvdzicetf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/godajcmpf.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/ghidnzdeu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/guaogsoeu.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gmltapuyh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gqwkkdijt.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gfgfmpxji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbvjpvqiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gujzzodzo.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/grqggovbu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gqepxavbr.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gohdjeldp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gujvvvemf.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gmnhmcnmt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gientffvq.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvpbbjbuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/grwtfqltr.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gytjuuhpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggfsgvphi.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gyjeoqfzf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzmkcmhyh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gbouzauqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvtwwsonq.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxxrlrnyg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glvbizhsg.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gltowxbvg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggdaygtku.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmpretypl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gzhmgfcyx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/guugrzbmt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gtubagaut.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gpjzuksfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gowlfgcvq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gheibfuoo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gekkqbxdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsfbxflkk.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gnbzccsuf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/glogedwkr.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gxqviixdq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/guapookzc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxmagulhf.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpgbaryqq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grkuizjdw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gqtklubvk.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grfeiombr.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gccpotbsx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gilmgbkwb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/ggwvswcxw.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gmgvncgnj.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gnonregbg.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gkmcqxaea.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/ghegkamdt.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gxgijiyut.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gnpbysntt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gshnevmgl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gqlpyzjqe.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gjkffkxvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/grrnwpcys.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gpsnuuoyw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gmjfdvrgx.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/grjjwnsen.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gmfvyxdva.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gtaududud.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gywmxclfg.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gfwibngog.sHtML


<!-- 参考信息 -->