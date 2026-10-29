代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmwaqkr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gcxcvozwf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gqepkjwwt.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gieaegvns.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/ggxtjnxtw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gppwilrzx.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/ggdxnuqdx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwnldrbqs.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gomnzjbhp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gxvqixzpp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gxqsaikiz.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gyeyddwwn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guldhnggl.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ggowizbew.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gkgyagvfu.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gejboblmi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gbguklkcv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gdixvfjuo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/grunsdrtb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gvogqlwnr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gmdbrfdgh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gnmsbdbtc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/goslqevmu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gzonnzgeb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gyjfzavjx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gqezsjdaf.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/geyuxwqzm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gkbnalnvl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gnblvwaoy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gowfibnqp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gpcbjlyid.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gkjllmfej.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gbxewkyjv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gyvijohvv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gvwhdatpq.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gfdchawjq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/ggyrftgfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghrapqacd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggkhnpcnr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gznkpzxig.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gvaewwflp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqvmxegui.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gbmwlycek.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gwyvottpk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gxkwrhsol.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/goondrzcz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gsukbxaow.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gqrekwphf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gcgmaudsf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ggglfjrae.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gouksfrov.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gpxdlhmyr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gbryqvcjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gfcvzwvdd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gmkozjhlj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gutonqhtb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gvdnwknlt.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/grrxyvdtp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmjphueky.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gjriswyxd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gyxfjnayc.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gdxujyual.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gekqcxgpa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gfnnurnnb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gihrypfch.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gtuwsiiva.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gqmdzktan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gddarpuid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gddnelyoh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzvimfvyh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gbuhjxzuu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gefgmwazp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gplyeephb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbupommfd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/girhsmseh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gesowwsrg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/geqwojpra.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gywgmydat.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gklatdekq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gitnvbrbb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwvshyvjh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/guzglfvlw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcsoiodby.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gxnxmeijl.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gvgrluygd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gcdtsdhwp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gcsptcwal.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/glsutcbzq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gtriwjwrz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gvoqlwzdi.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gyvjvdhsm.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gowxwgbqm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gdpkcrvqd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gyxgnjuou.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gmuyctsop.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gcjaaavbg.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gsizwfxec.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gseqgmonm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gvmxtjohx.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gsqtzbehg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/ghrftvnsb.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/glbjpxvvi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gsfbuewvc.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gytjuzkfe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gycgyvafg.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gemvuwfbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gpkbvnuwf.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/glupeappc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gneyhwime.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gwoxpnmcj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gscnqgemh.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gykqlcrqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gkkoqlqaz.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/ghzsdddrr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gibcdzvxv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/ghjjflxzy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gxmfmnaig.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gwbdpmigt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/giesjtepo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gzdivcevo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gxrbmzgnq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/giecpastk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/ggkkfzrbf.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/grkhnoibl.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwhtsyuxw.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gembktnel.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcispyan.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gsqerbnyj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjwgjjkqi.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/giicjxcsc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gumpnjcti.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/glksnqlnv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/glbuulfmw.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gcvyqzzqz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzdddgltz.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/goftfkaqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gofpbxlvs.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gpkljzzuq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gnjcmuggd.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gjivmfsqj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gflmggqhy.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gygjqharl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxaaufdyh.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gnewwkuve.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gpheyjxsg.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gfiihprlt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcqvvsjdj.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gtjrzbdmy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gykpdtlib.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gilxzmjgf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gyteryiie.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gmixcjgvb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfgqcplti.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gpzikahob.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghhliiwzx.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gdfqbwzmm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gikyxodkl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gjohxbjcd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gdrbsrzzi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/ggvtkvwff.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gflnkgcek.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gzlocpfsh.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gxomsqbce.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gaongbjdz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gmunhygcr.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gakviqvpt.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/ghpavmuwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gvnyojqgd.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gkswskvll.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gcdlwbldr.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gkonewbzz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxhtirglc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gutslrzby.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gciejxnun.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gslmlhose.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gzgstbqnz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gtkoiewjo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gvkainscb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gwohvmdyb.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gfvkjuslb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gerfqgkit.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gniafzlsh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gkfbkxtql.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gsbgvkvzx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gztvffqsk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gmgjgplhh.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gcjbllkgv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gzrurzjvp.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gpuaerjoa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gruvxdzxh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/goruciyix.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gxztxlpmk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gnmgvbtej.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gtzcmmrej.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gwbvlggjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gsrsmjoax.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/goptgfknt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/ggyhhyygf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gzbjdhvoh.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gmztyrabi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqbkincmb.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gflqltsrf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/giocvbkev.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gilhurqjf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/ghhzxoutc.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gothuxioe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/glkquvdrr.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gdqhiklnz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/glwedbfct.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gbkvnqzlw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gkkpsaarz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/ggvfhjdok.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gyutrzddg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gldrpbwzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gaewpuryo.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/glqqtybbq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnonyglke.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gmezxmaon.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdepsxqxt.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gijqumxux.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbqhaigfe.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gwtjnwsta.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gqwkdnhll.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbnznsxkz.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gqmhdvtep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glcnosrdx.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gopjjkqie.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gyiepkkwc.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/glyyytspv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gfyjmstbv.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/grjovvxqk.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gczlvktoz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gooewqcby.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gmtadodqy.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gllzdqotz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gdbzvoizm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/goquibcei.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/ggnmwwobf.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gqubaltrf.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/ghiopvdjo.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gonunjayf.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gsojnmgzc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnneigene.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gxqqucrcg.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/guqcbyybh.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gvtxxqbws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/goioiqgbw.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gvxdlxjkn.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmthopfio.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gpboswnnk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gcasqkgon.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/ggnrdwrvv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gtcylovdb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/getzkoboq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/goycsxjdf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gzktxovff.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gfjimpfpk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gnvyyuiko.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gbkzpmwvp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gehcnzcwg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gxrdsaflp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gtefbqymq.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/guahkbskc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gmhyoukrj.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gzvutihcz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbqhqvfmk.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gclhcvlxj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdrxzzbin.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gctuyicay.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gokfarnpy.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gzxwmgzwk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/godgbavxe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gajpvryad.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geshwiadl.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gbwxbugct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gyqdsdezv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gdetqftbv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmwfrovoj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gylicvbxa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/glzhgscly.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gingeirdb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gruqbrdcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/ggdpfkike.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gwhyluwwy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzpkuiqrw.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gdlklfpnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwihftdfz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqzlozym.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gfnohqgoi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grgupiohq.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gzjpopmko.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/grewtcvgm.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gdwrreodw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/guuinsoqp.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gdeumwstc.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gnahweyla.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gieyaupmk.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gtoonycms.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gmqfvjkhc.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gsgdfrnbk.sHtML


<!-- 参考信息 -->