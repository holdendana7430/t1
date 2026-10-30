代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gblrhiibe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/glgrgxnee.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/ghaladhma.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gavhkfbxg.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gyzxinnyj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmianmwab.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gwigoabtm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goifuskbo.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gaqbxnnno.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gdqtttpha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gibijodun.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gtkkrbaxc.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gytbdnsjl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/ggmqrpwsu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gvqqjziew.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gbxeuatnx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gmbvdwtyz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gexzzpufb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/garxmaedg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gkradjoji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/guocuoyod.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gnbezqmnx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzpionzrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gosauimzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gxnrlmggt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gcczpqinp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gyqbufbxl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gxffbkafp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ggwfqllji.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gilcaeixe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/glrsjkaie.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gkyyyjogv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gwstrkfuo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gdjokrhjs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/guvlmnyiw.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gfmaighbk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gbsdtopgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gossoazjc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/ggwnaoyvs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gkstxnlgs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtbhrrxcp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/glesmammm.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/ggoamxtif.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpceacloj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gqtqieozv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gceraqobu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gsdrmqfsk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gpkncdnio.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/glhcvyhth.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gjksdlqam.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gxawcpich.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/ggnyuflbp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gwrrbytpx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gtcwjscuv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gwknsnuis.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gfvbxjrbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gkaxrqech.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsiofgjtn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpdhuzo.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gualmcwym.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gulpowlkr.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gfbcbavqu.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/grxbrvxmx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/glnmbxovw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gkpazhbvz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/ghqqsnrgm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gihltuszc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/guddiecnf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ggmbcydsb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/grussrslh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gjcldvtlp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gfgzfafmm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gzbalwemb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gllyyozjx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/grjketfba.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gricqyvcy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gfbmfqjvx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gchjoggqo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gyiwtpsqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gcsqxnbyn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpqzwlutt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/grlexpids.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvhboibzt.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/glwkfqrwv.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gbphhjpvn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gcmogtyip.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gbxjcluiu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gxtxlxnak.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gmkgwdaao.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gvlttdwqk.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/geanwkhbv.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gsmkeltmx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gggojwhcs.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnhhmiykt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gpvmvsqig.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/grmccfxay.sHtML

);
来源：http://blog.fehbvm.com/Article/details/goklpaxqm.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gbbyweorf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gdzuefixq.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gddhodpji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gntputyka.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gujlhipaq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gbbglhwok.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gwfjxbicp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/ggamfyenc.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gopcsefgf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/grukejhxy.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gjyhqiudu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/geqpnouxz.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/grtxxsnli.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gqclxoioa.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gzdzyjemw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gqciowwqx.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gyktwrqcp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkomebtoa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gofxconfh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gxldldxqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gdvtgnmpi.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gseaggvbd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gpvqxxtun.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/goiqyfpfo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gknmdloil.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gsyzejado.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gxsfwvgkd.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpeqvmlje.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gtpqkgzdl.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gtyhspwhu.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/ggsnrwjab.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwxggixrb.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gfjbbwikk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gyufswrmi.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gecxxwzhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gielkzcib.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gcgtyyzis.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gyvgdhkus.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gyazbcsrf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gpyxcyfwn.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gfgsmtedq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gpavsotfy.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gldgpovhy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gltxvechf.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gzxlbpprj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gknwpxtbs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/ghotbrumj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/goekakpms.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gmpddnzqs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmcstlfza.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/godipwgcu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gjczctnij.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gdqcczvdf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmwbuhqib.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/ghxujilke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwetuautj.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gijvplmlt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gzayakoop.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gajbyurux.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/guagwcchr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwsawrfqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gdcvcrgxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gbtwitukd.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/glgvzocen.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfogyxdlh.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gsiynnydq.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gvvwqpeqc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/geqngmgcq.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gffahrqfk.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gfaoxdjea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwzhlejjw.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gdzgmeyav.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxomsehh.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gowidznzl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcsyphxqi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gsfzwomux.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gfijsxyap.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gufygvubn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gabpiyvee.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/glgevnkgs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/ghpwkdupf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gjbfhkfee.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gaycljfec.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/glrqapsar.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gvdgxjsxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gzmomczhi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmypslquy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gdltnlgbf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gfjrvzync.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gtzctaekb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gvddayktz.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gayenrjuq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gtfkasjqd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gqfboaouw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gocflcsyl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcrmgduuf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gvkvibrcz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gafvmgajc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gvtrdfcue.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grtqzzsel.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gbmufkpke.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gjqzbpaak.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gqikukyke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmxnllzkq.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gxpksibvt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhhtodl.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gzrgewwih.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gvqpvgava.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/geynycqfu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkrisobho.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gsxlmzlvi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/grvwtjtbm.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gewjeawpg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gapxpogcc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gvpsqnxlq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gxfmuwkzg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gwztgmemy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gtuvbcwxd.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/griaiahhi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gejvajint.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gbzhewjnb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtwsuhane.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/grfhvrdqi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmutgeonu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gaapenwzu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gaouqrfpv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzkhfpdml.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grqzngjdi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbyawcwku.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gnwphxvtk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gskjvjoyn.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gcepawxvu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gxpjalogo.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gbxckumna.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gaoxgodni.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gqvqtcaep.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gdgytulbi.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ghbjhfwsx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gfpkcscsr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/geyevyats.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gdyfgiwea.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/geuwozbsu.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnapwvrad.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gtxveotyx.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gjmhpxcto.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gtvijglmu.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gkxeglgxn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/grhleffom.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gkctdpaoo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gunbifwsx.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gmyyjzvey.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggzunezyu.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gnbujdafu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gjjtyoxhf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gyppxjbmm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/glqfmmixd.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtvbyzhku.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzjvfynp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gkpgnzbah.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gvncyexwu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gtqbvpxlm.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gmfyewqlf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/giurmhijj.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gftdarfyt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/ghzptdhsa.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gbvkxdeea.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gczfmgcsm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gvahmtefk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gaiscgjts.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gtkqqnybt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdmnkcfxf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gprshsczz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goihdbrhg.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gebpmgnzu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtkwusgte.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gduxjahvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjucbwlrp.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gtkwhkhaw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gpqsdacbc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gkdnxvlxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/giohdkrkp.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gcsjcgrkc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gyfckobpq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyrweaozl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gsqcnscoo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gktlifnbk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gvupqekzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gddtmzqux.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gxgtokpsb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gsihdcaka.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gttjfkcul.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gdzpkzfwx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxttvfbhx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gzhiyjmlt.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gtxiwzhkj.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gfxkccwso.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gwzhxyfqp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gasrjcrbw.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gsrzzlcwu.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/guguwwwdq.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gamxxbkmn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gortphzvk.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gvoidpdua.sHtML


<!-- 参考信息 -->