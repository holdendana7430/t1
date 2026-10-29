代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/goovvkult.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gnnkhksot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gzcqbqext.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gfrdxptfa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gltudqjcz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gymbszftl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gsewfeqyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gooxtmsru.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gvemyhsrl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gruqofxep.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gtlbrgvkq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/grywxhsli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gledhxmlw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gzvioeqnp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gqonpatdd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gmmnvlzwj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/glrhgdjto.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gdldrivwy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gwwrxogjh.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzrezktpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gsokaajte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpzncewut.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gqyqedlct.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gtailioxk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gonzmmxxz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gekwajhzf.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gpztvcxgv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gznrbgfnj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gymxeibtt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gnemglvig.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gaefgfyct.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gvzqucwpu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gsqyitajz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gejepirod.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gccglwjbo.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/guajafebl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gypjoaetx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gyhlcgdyq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gvznvbndy.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/guyvmeskx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gnpccetju.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gcxzuyaqc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/glsjptmfp.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ghpjqsrfs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ggnqetucr.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gffsfejtk.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gmokkpmek.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gomdvwsuq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/grdxafkmm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmmrhubge.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ghlapyrgb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gpgzwouhe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gnygdnmox.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/ggrgcahda.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/guiugydwp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gegkiaohn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/guebsjtpm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gowrmxlxl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gofzfxctx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqynlmqj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gnycociaa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gftzswntr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gblgavnsg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gbotbkizf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdwxgqevg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gifmpnvko.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjtwhjqsz.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/glywbcoeq.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gnfonjgda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gqwbapziw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gbtlcryko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gaezpwggv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gmjyosgvn.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/geigrzysr.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gbdvnpagj.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gdaiopnxf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gmsanzvcz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gtnfdcnhk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gpltzgady.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gnkaehbfq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gehcbdtrq.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/grvyiuvmo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gkloubunu.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gplujspos.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/glenvxein.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gmqckpqku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gkjylyedh.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gnsextdxj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gjniprlkx.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gtgffduui.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gaxtbzzub.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gecgmkibe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gmlwoteqb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/geeamjquy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gerxxeriu.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gtdkjpowl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwegiyzej.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/grezpqklp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gmmyibtha.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gzuswsyck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gnmdgjftp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gcjkbptfp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/grsrkegon.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/getcrcepq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gpastagou.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/ghjeddzhg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/ggccdgohq.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gvzcibgun.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gkamjszvc.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gkelfiogl.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxfgihezt.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gzhlqnmhk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gltkwjmtw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/glnacvnzd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gmejwbljt.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghsipjkke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/grcyhthuk.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/glzxmsbkn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gykufpvtt.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gwhgezkti.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/grsswurxf.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/grsedduwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gimgnbzkv.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gmftrcuup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gxfwausiu.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gjvfqcaxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gblhwnklc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gsrxmtkka.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gfzkwnayy.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gniaymbpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtfgkjbza.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gibrnvvqk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmrxkszii.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gluvtpmcs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjpcwuuyv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gmzrgegpd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gstkiwvdy.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gjaeoiayg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbleqeqpy.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/ggjlrfkmu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gqzictmxk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsrvywkip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gdskwfyxn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gilotutrw.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gibczhimc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gsuixpult.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gtxbmyfrg.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gyzvxjoaj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gmxkbgdcs.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gcipomtrn.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gukidxwxs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gxkegdshx.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gobpjjepc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzlhjzswm.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gwtecrtix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gbjvzwfoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjhztyrgf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gmceyyecb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxirgrj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gwybkwcus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gnuvveviq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gczlxcbhn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gzgrziofs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gqsdnsnjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gxqovtqsu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gpcufchhh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gubyriugc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gctxtijvk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gtltvdjwi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdtcgxpll.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/ghntddvnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/garlnjqon.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gywiyjtuv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gkjqffxkc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gwgrqjkdz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gwjofvdwb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ghsoqouce.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gipclunnt.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/ggbkfjdgx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gwtibqnxw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/guvfrglys.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gmynnmvnh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gehlvzjdd.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gccfaqvwu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/glsyajtdb.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gsghyaszo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gtinusclh.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gfvthebti.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/grwcmrhfl.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gcfzinkdu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtavnxodz.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/goomsqspq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gftjsxmko.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gfxsmiryo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/genxorpaz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gwjtsnztv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gliargziz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gykxlepxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/geddkrwkt.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/geypfcviu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grztkufjr.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gsfzclugo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqowsrojr.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gjvbbmkcj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gymwogzey.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gfztwevfw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gpxqawruv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghjttylyh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gnqjhhqxz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyxyhpr.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/guxoeqyck.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gepxebzdb.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gxuhwudsm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/ghagvofzy.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gojtcjkfy.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gepwfmvas.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gcmuynyjc.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gpukbvkiq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gnzsdwhst.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gzdzkiyxg.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gzevluckq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gzeugvqwr.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/grohgzwcl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gmgjajjyc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfpoffgdm.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gpzwezcbk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gomazobva.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gjcyqxaxz.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gwihbaoax.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gygznrlod.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/ghodjrgkv.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/grpeaafuf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvuwfgwhn.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gjxfpebxz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gydtwttgc.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gyohaozod.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gaulmufxd.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvhihqici.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvcfilcmv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwsjdfnnn.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gxhbazotu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gufikqohx.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gidliuoet.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gliooavks.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqawuowfp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gfzrzftei.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gnzkrmhdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gfkqsnivt.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gppuqioca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpgfvvman.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/garvobrad.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gjgfjrmle.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gxrldfpgp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gitlwkvzt.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gmyipctnv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giynqnfit.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gzqutetla.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdjnnswpp.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/guablbtwt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gnqreocot.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gdidybjgn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gkrpqmsoa.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gyxgfjhcd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/ggizihdxu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gdleftaxt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gvnbbjhnh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grmevoxxi.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbmhlckzx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghijfawrr.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gmnlezvqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gyrnpdclx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzbswnxbc.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/ghedjimvv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gokbiisor.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gxnvtgpxz.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gpokztklh.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/glorboadl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gwryoslze.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gdelkyeeo.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gzmwwrlou.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gpknpeego.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gmftdhyhn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gdabyrhkj.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gooeplawz.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqpoxwago.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/goywldzwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gxrcsjkwe.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gotpfsgnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjxyumkgw.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gdrqhvvbu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gstteilzo.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gqkkzdqdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gzdqsuvaw.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gbvhkndsw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gpcoitfmh.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gsbpzzndf.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gvzjddcci.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gsqmshsri.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gdhznyxgh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gbpxtityr.sHtML


<!-- 参考信息 -->