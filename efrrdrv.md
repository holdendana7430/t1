代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gnxdpnezb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gvgdxaspz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gvxoedupv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/golkoomzl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gwysyqsny.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gjxqownaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhljjmtc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gemuxdual.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gpgafinbm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gbmugvuvg.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gzmvayddq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gvakrwaul.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/glazjjbpo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gntpzcjwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmhgqglxw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ghvltcjyg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gwzxbpilp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/goyqkgoyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gxpwqxqfl.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gkjeaellg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/giykrvejy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gzsjplcqq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gqcdaayst.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gcfdaobjd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gwbdeebij.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gypxumfbk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gfrkvxngd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gmheitjtz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gtjkmghge.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gqczelqzs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/ggnjbiaok.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gmkiteksc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gjfzrjkce.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gwgdcekis.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjmwughwf.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gdcshicyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gsywohnoh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gcmmyoojv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gepbchzze.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gvzcnjwzg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gsikovqen.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfmxqwuz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gdrdsxyfk.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/grsdrmwsk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gvvqlhpyx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/grnudrwqs.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gduplbkmq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gojxpxwvn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gwlxsfeft.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/godnaiuui.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gunzdqqya.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gpxbjvwnc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gswbhypsl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gbomcluuc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gsttorrbx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gxlsodkdr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxidgaq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gzvqwfqeo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/ggjrppgyw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gavetfgvp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gyszcimme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gkplkpzas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gcotfxwoi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gswhzguek.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytsbiiyl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gteciylap.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvdcbgehj.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gcswvqfjh.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/girmreoaq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gicfpnfzb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gmfyiavvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gjkueavju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gnexgkixw.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gvfnkhcra.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gqhyynvbh.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gfzzdydpe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gwpohtqmx.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gjotflyhc.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gywvzzgfu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ggncesedq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gbcxgyzeb.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmjgpmsew.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gkqorvgfd.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gqzuhnwuc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/giqjyfqsz.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/ggyajtvwq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gqrqiovse.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gajgsmfrf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gdcanoaop.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gmpqfpytw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gbomhqtfr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggymlqwnq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gizmhhcdg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/glfbpymfv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gfyvykioj.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/grroazzpn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/giorplqow.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/glzfisiqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gcenalcle.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gdfnmslzp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gxiyyyoyp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gwruukxac.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/grsydpihk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqjzkcnqh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gunxwggrd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gbxiqbcxu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gmzhrqbjd.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gpvibtbou.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gapotyhnl.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gsefskbmx.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsebhiddo.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gbrbgloae.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gemsqgnui.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gwcatghtd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gfznjbroz.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gkpdfvyah.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gpvyowlvy.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gobvygrdu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gigniyfgw.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ghtxrbavt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gvkapfiso.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gnpeeolnf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/grxebvrvt.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gboyrrnrl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gyouqarfp.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gcwtwbcve.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gebgylmqf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gerbbwttg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gnfujlnbd.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gukzdvvtc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtekmrdow.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/guedozfzk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqomopfkc.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gvvhlarfw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaqonuabv.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gkdvhlqpo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gozdwskim.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gqpffixtw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwjkbpyrl.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gprkwpbub.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gkiwpehnn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdptjwpcm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbyjotdxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/ggvfcqprg.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqnivrozs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gzoambbmf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gaqmrzozh.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gqvfzqrlw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gatkuuudl.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gmbyjjalj.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gsblbacge.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtsyekcnu.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gkmmxxeec.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfeqabrwb.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gvtwelzit.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gfhhdjyjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gjioldjxa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gblysdmjr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gqkftfyhk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gbddgrixz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gfjyxnalo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gvrsbmkrv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gdynfldku.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqydxwxvm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gmvqlzqkq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gxolkidjh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gkvjbeowy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gvishbdce.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/giafugiix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gxowgzdoo.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gqrbwjqft.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gfqmmxaym.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gujkwcltq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gwxritmqa.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gsllnbuyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gxzplerou.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gjjircxzh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gdwdxzlhl.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gdqbkctme.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gbpvfgqao.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/ggrnwoous.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/grifuffhd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gldlurelf.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gkyqtbgso.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gfsrfqoqt.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/ghljghmao.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/garwrsmzr.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gnrfjywdj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/guxfreqhw.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gybewnkbm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gomucvuvh.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gynuzfqyo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/glmsouobh.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gqekrimyp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gcldsbegg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gvzdmnsvd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gqpzhxrzm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gptzxnxat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gfcrccddt.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gozuxogee.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghncbgeyz.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gcyovnplq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gexjgdohr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/glntajguf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvpjpbvyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gahcnmuum.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gfzjdvigu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gudhregno.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gvjdbqeup.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/grepohibo.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/grmwxfeid.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gnttxsazc.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gbpddyiqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gvtynyhsq.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gnnktswwk.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gjcwqkbxl.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gzmjpcvbw.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gfbdqxmsu.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gxmqtjhmm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gdfoekawz.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gzisthobo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gbewxrpih.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gejkuenvj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ggvfptjya.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gkguncicr.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gimqpkhgd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gerzhbfih.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gzkiqftpu.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gzeiedytd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gzthvbeyz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gudmxccab.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gfuvdpvcm.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxeaxvrua.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gdkqkzooq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gxgdpywgl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gjuoqjocm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gclglulug.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gjdumvoqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfvhourpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gcuexvwmr.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gkcfcajpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gwcsakobh.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gdiossjgy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/guxwchdly.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjvbgmdqq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gonpyyeyy.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gersgxzgg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gmqvgqhkj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gnxccmgxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/giglriack.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gbjbcoznl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyphlqfjn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/giopxlctu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/glivarvtx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpklygztz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpzggqsgy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/goxfesrix.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcpetgwmc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkxfqvi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gbsczcmxc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkhneen.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/ggcwcappt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gidabbljo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/glrzfqzjv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gtxktzvrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gjockrcsr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbztfnrjr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ghdycikqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gxkyydoxv.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gfhoctxhv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gcnedghzk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gykbhdckl.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/guotplhhx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtiutqzrk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gqmnomzmn.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gyavjtxfi.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gjntsmvat.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gecjhudzl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gnblxorrf.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gudfyvqyz.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/graykauxk.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gwbdvfhep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gwcwmnmer.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/grnkxukcu.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gvflzemek.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gphxosewu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghhvzsvjn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gqlwrjtgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gibenudxt.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gbkmeeiou.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gnvffuwkg.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/ggdlljpbi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gonflxnzn.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gshiziqtc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/ghsjskmcs.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gkpjhjgrh.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gaqfdjxyx.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gowqictan.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gxtqzgpkr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/giaxzuqyf.sHtML


<!-- 参考信息 -->