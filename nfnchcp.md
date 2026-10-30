代发 wailian999

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gtiogrvey.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gesardtvi.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gdzzaanxt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvrmviey.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gfupizkch.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/getbwtklc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gfipwcybh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gytookmhm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxrkhjttx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gevcpujou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/ggntmkrru.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/grlvtfwau.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gqxnbcllf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/grbxofdqx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gdjwoqpas.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gdmfschkg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gotewxmqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gfupathim.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gsxhjxind.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gbtksfjrx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjjxmmktx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gvymplghz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gaqjfnjeb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gswxruzrn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gwrkplnvm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghhcjdahr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ggpwkqogq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gpxgdcnxe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gwyaxemwc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/ggkzmkxwk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gwirjbqgx.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gceyhvfmw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/grfzackve.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gczrpomsq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gnelwsdtx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gqdanckij.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gdlkgmtgw.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gsvmkkkko.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gaououahz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gjoteffpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gsollshpj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gcrjinwnl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gsfmqavbg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gbvzdpywc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/getynuhud.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/giimvvkws.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gjaslqquy.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gzyjaaslw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gkfiibdag.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gqbemdmee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gulgpyioa.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gcayaoyld.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ggspzxviw.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/grrhuprux.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/glnyuhxjy.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/ghhmiulqv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gftmuexum.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gvqooyxxm.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/ggoizmnki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/glaqcwqkg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/glxeymhch.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gphuyzamw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/goyypidxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gdozszgar.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gabyrjxea.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gvccotspp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ggjeubjjp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/ganxvrewa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gjvfnkslq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gfwdumycd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gfqtspmfh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gjndzvsoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/ggblgceqs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gtqopyzox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gkzzrlckq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/glbfuqhbk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtmmltbzz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gipsvkdgc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gllvgoxlc.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gyuvuljro.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtxhuqzgr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gsgffopcw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gyunanrkn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gjeebvzhq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gtdzmfxxh.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghwygtwby.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gpcxnscuz.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gvdsxqzld.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gzczxuxlc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gryuobfsu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/ghwibmywx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gdxisxyvl.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwujkswfr.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gbvplvsqr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/giohgyecm.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gihtuxlez.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gwrmrrvmo.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gtrsfyyyo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gjzlyadet.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gpwolbwde.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gqoixaech.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gtmmnpzkm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gcsodrmts.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyoduhqds.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gpfhpdhzq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gfyigvper.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghecrgjws.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/glvofglkw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gklpymvyt.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/ggacfulsz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gvnvfkmwv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxjhzri.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gxhouoiwb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/geimjnztv.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gqkqqkhew.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnnvpgfvu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gffoibplq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gpujuqmnx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gfghgkcul.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gdtlnbant.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmeqsozaf.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gwdblognk.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gfacmzibh.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gykdgbvxc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gudtgxzny.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gewotoaau.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gsomerwot.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/guuavshnv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gymqctstt.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjbxtfo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/ghprlfibm.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/goiyromgx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gnscnhrfo.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gnlesemww.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gmropnyqf.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gfnozuxnl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gczyebkym.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gwszzbtut.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/guyjikocv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gtcusbdvn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gwkgefiuo.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gnqwvvrts.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwjukzcoz.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gvleqkpyv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/ggbqbqxyj.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/goopzmaen.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbtnueycm.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gqsoppwqe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvpkizrqy.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gshgdigvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gdubbydvj.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gfaspuips.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gbgynhhtl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gtwxoneyp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtgbsbajo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gfjdztiqo.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ggsnkwiop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/ggpzqqvww.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/glvazfdne.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/ggwplcdyo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gnloiehpl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtamparag.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gdcqimvzp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gorjinsaw.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gixmsedpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gsaqlpxbs.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gtvwjppnc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gtxolzked.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gwlobtkin.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gbscytffi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gizugziey.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/godofkvno.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ghjdvkuel.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gloojiwwl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gtvggixxb.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/goosohjrb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gvikvxfej.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gkcfovtbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gnzgjxlfg.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gpdwfcduq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gqjqixgdi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gkrzlfxxf.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/ghcjuzrwt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/govhangtn.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gqlesjtph.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gwswvbsnd.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ghxiruoja.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gmfuhamrr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gamcqicgu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gqvnrpuvf.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gsznvtojn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gfhwrpzvx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwxhnwvcx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/grpvedjam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gclmpwuke.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gspzuyyrl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcfcfqwdz.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/grvazyrzf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gwjmyygvh.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gijzkcwwj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gwsnlqsvw.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gwjwnyluy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/grktpqdpl.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/ghsyoscbx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gptdnqlri.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/ggvghrori.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gbxjntdxc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gyliwtfhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gusdhpukr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gzwcoicfp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gojfngwjp.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gnyxunkaj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggotpmhij.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gpgvhnnhf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gofblbgzg.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gyrgpxprb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghwxojrkh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gidqqmuap.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ghgutuoqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gexdrwewd.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/geatirgjl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ggzsyfrzy.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gucfssiro.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gwoytxddb.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gvuuxmaem.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gccadzvil.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gbpzwuznb.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/geaxiepmi.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gvpgmotop.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gzcjoqfqq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gvihguvvj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gnkgmsibf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gzdvnvbza.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gyyetdiya.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gqtwaogub.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gnauipdnu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gevtccnfz.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gkuumznxw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gppplkkod.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gkkbzgnfz.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/govothauo.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/guyxgdbin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gsrtxcudt.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gfcabysdi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfzjvwbnt.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gzxloodue.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gjgrkqmhx.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/glfaiwrwn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gropxhxps.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gkmxlvrjw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjyogxndb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gdlbreniv.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/grefccgch.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gklnfmerg.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gzrckztdc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gjdunuaje.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gxemmoqwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gqhheteen.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/ghkorqziw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gppbsopsz.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gddpbrxon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsbioggsj.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gisfvykvl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gaxtlavlj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gygvbyvdo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdkyxnkfn.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/guqirjyec.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gevhlonnn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gyuxjcqme.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjwtgsblt.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/ggdkbfgwv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gajyxsgmj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gsyusdisa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/guamcvjbp.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gdyqdyffi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/grkkoqdaa.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gzickpjdn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gxfioaaax.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnbrikako.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/grlglccze.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gsxilotub.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gdvhfdjas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/ghaqeumvg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzmzslcts.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/glbgvybhc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtnzkywkl.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gpnsgjhsw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gkvpjezhg.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gmgoqkhbp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gbisyhfwx.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gztfiegoi.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gqhmqciqf.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gxwksiewk.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/guanhmcpx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gxffvkjjs.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gsrvonvhi.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvorncx.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gaxlzthcj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gzemdeomw.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/goxthskno.sHtML


<!-- 参考信息 -->