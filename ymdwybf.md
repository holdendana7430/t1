代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gpsjoptbf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/ghuftgaxb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gzcjujvhu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/garwdkyry.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gncpxvmwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gmawfwxpw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gytqgsixn.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gciuegfre.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gbpwoymod.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbvtzempn.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdaoetoqw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtfldbvgv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ggegricru.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gibjzwnxn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gjhrjdjfu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gibzmgbvb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmauqwpgy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gqbtfdosj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gfmxebdqu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gywlxkbpx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/goejncxmr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gyflkeopz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gaqprgcul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gijynnbng.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gkmlrzsnb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gjokyxuqb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gzqdoryof.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gccnyiqic.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gdmdliayj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gbdopjnzr.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gdxeuxkah.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/ggtovichj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/guxbqvldq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gecbfcqoh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gmxugwkvn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gndhgimvw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gdobhqeui.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gsoqbdmev.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gtuwwwegx.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gjpphyghs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gqolqmchf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glyxtpgut.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gdwwmvjwx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gcwmadurd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfctdsn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/ggcrjsvwt.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gtvvcqypa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gwmszjjre.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gaezqilmh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gauvegjhc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gyiajwfrs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/geidcajph.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gnfwwjbym.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gyfhsjjpj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/glvbeqijk.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/geoebvrzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/glcjeztcv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gsfubvzxl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gstwqwmhj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gyysurdev.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gsuczblme.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/getshdhqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnskyuhxr.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gjbnoficg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gsdzwadvd.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gkrvhiznn.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gspyarnod.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gvclmckem.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/grlckkjiq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/glergkxpk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gcmcrfmzt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gepcclwir.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/ggazwwrea.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gqaekehcm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/goeomomvc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gwzxvduvq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gtzocvfss.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gudjxwsgg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gwmfitolh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gciraomaf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gbmpbeajc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gqjlqujxh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/ggtfxdfqf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gityeeoyj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guotsaswh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/giqpgbkvk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjmxbvrhr.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gkpgneiba.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gyeghjijm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gqztowmvj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gnqsyqecr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gcvmqybhd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/grxfaiwwz.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gdaiuyriv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkaqfdcet.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gtpaamkub.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/glmheviqy.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gugsnqisn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gdzfrdzni.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gdcllmqam.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gidarikuu.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gfdblaohp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gswviwmhp.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gexsmloda.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/galemukbt.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gxtqqtoqk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/guwxrbfvz.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/grsqjmloh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gibbeqfrf.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/geiiovlva.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gadntxoie.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gsjcdvubq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gutoxfccg.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gzmycxtuw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqafpxacy.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gcnhrjske.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gogdfakfb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/glwlnkect.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/goepitvgm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gzkcugdln.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gisawpprm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gziwulcoq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gzgohdhyo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gshwcbwts.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gfvrkzckh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/ghjiircfq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gswkunhiz.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gaznbfgws.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gluwxdgqu.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gockdmbmn.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gusvavdex.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gabgaifdh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/goltskaxn.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gkjwbgcxt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/guhchvavn.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gnmhufrwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gnogswpwb.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gtewaxefs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gbdbhwhko.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/greohewkk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghhbmrqsd.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gmlhupwnp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gzprcdyfh.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gwdknifiz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gelezakgl.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gkdzysnaa.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gajemcjkp.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gpkmdslqc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gmdexybqf.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gyomrbqco.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtdbmkray.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gaqynstlu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwojjsipr.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gjsugihlo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grvnsywdt.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpuwytitb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtpnbjacz.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gqbcdijki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnqebesem.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gsofwbwci.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gtkafqaxk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gllulmskt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gejticurl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gkramcqbh.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gturunsaj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gbgtzenjn.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/glktvwpvh.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gunfjzreh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/grzlgllhl.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggmoeqyry.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gsgqejmkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gpwuwgtou.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzzeoiifb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gesaagwmx.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gpngvvxsp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gpzghkphf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/glbvitmuh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/grineucej.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gfltdbgsr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gctcybeiq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gkxjnuriw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/glhrmifzt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ggoqgcyuf.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gqbcqkrem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gpztpuaje.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gxjaodzmq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gmylufnmg.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gtmoidmke.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gvadqixjy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gexckxjqb.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gsvncbrui.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/grvanybub.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gaheikwgt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gozhtynpo.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/grluthwqo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ghieamgqh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gvcqjkppy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gqacgfssg.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gevaqzsap.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gwcbuutue.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gmvzxdazs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gctbixsdn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/grecndfsr.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gnhlbwvlg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gsgsdmjbh.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gfcccclcz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/ggpqfeahx.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gbaeqdjda.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gkadmhvkv.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gohbnoepp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/godhcghuc.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gfeyhgkwh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/glhgwlvbn.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gwdwexrtm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnysunx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gzftgnyxc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gfvdstpqk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gzuznabxx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpckuswxl.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gpsypmtbo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfvvfjzsa.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/giglklcok.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/geofwighg.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gpjqssucy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcpaohvef.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjufcyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gquuuhmam.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqffewwlz.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gqfbulevx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzwkihdzw.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gdrylyncp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjxkhgssd.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gpxtmbsbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gkxpersnh.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gjqyowsxn.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzfrmotjj.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gfxioqaaa.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gszcchsuk.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gcvoifsvx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gqulrwhtu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gfpnadfsz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gsdyumehq.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gnvvqycub.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/glggmnsfq.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gpxltpyqz.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gnytchnsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gixwcfppg.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gluryjsfq.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gkocxbjnt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gpaixlqgd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/ggehonuiz.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gcdtchysi.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpxoemrxf.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gxfoeqeol.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gvkktguqt.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gmkdiuzbc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gbrkxubqa.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzdhsbkmy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcblvkjpe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/ghgegkzff.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/ghuddqsdn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/ghgvuzrwz.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gwxihcgro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gwbsjgzpy.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gefwiseoc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gkbsjizpq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gqxxygenq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gxxovgfmp.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gwzezsciv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdllixjow.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/giyvzcdvf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggtdqabif.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gwwasbibs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmjrxyqxs.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gaaroebdy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpndpfphl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gkswyattp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxstubhr.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gbadbcdgi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gwllqrtmf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gnlhkhdsr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gshvyutvo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/glzwyrvyi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gpxowfypw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gbhljvhib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gkrelsdla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gevwhhcqz.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gqoquyjxe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/ghzmanysa.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gpsxehmpu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gcgbblpnx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glqcdhonf.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gptptgosn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpugqstmq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gfwmqiuzy.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gcvjidijm.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gmueoncey.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gnnnthzim.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gjtmiekro.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/goqgqrfio.sHtML


<!-- 参考信息 -->