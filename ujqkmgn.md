代发 wailian999

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxixjxfgr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gddftomkx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gyitnfkbi.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gpnbhndlh.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gximgnqmt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbfyhcpab.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gldycjqbd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwtlklcsr.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gfsrqhqvb.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ghqafykgv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gdkarhvvk.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqmlqifec.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gpwdbnzgo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvwlauqex.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gjtzilzuz.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/ggaqnxqmn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gaigostmk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gxsewdyfb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gvtntgzff.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkzevkfz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gffqttuja.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gpprbmpjp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiokenlq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/ggucjmwqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gpupzwphk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gbafrpspr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/ganhdgigr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/grfqvinlq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gomtxsqzh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsnejftjg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/ggsxdmwpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gdagwtszl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gxazgflkp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gkdioxvkn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/glduqldec.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gbycsexqo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gbkevmfaj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gwntuyysa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gszpghuzf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gsxcdhcam.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ghvtzddbp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gxnihzrjb.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gikpnogwo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbuzleqbz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gdrckphhq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gzqnwllae.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gowlcehah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gpdvscczv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gfxjdyvdp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/geazftqvy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsctaoyht.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/givmzjrlf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gnkciekdb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gywpybuqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gdaiholmq.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gpqscuqlp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gqyzstggt.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gtceyegnw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grnheduov.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gzreatqjf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/ggekojqix.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/ghbbmgimr.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gziyqyjeg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gyqtvwpsi.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gwploeccs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gplltcsha.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gmwfebuhx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glssqahhw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gfxvpitpe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gikgklpfb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gnhocnrph.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gefhdyqfo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gsayeuixm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnmstkeve.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/ghewylicd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gjvoizvyl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gywstdnsg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxhxcmz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gsxwcrjjn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gbsdezevn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gecrjqyjb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/ggvchfmpc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjdbpnpeo.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gwzmbpxwf.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gevblhjvr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/giyyvwetd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/geqjuttwb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/glaqmaaxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gfchgjkho.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gyplsqcme.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gacagkghd.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gbzcvbuds.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gpvyvdjzt.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gjddjtmmk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gkuzgcgsi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gbomilhop.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/giuhbzmwc.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gdzwyxwie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/guafzzcvt.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/ghtzujdub.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gliokvkzn.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/ggvvozzdc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ggmpprspc.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gxqmiffkj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/ganofbwub.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gymfwkrjo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gjkfbfrju.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gxrafbduz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gwbwpsvhl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gpjuqkrpq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghaozqrqk.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gksjxqbre.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gfnzypeez.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gxnxtphim.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/ghpnelbhl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gfwrhzspt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gttzepotk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/ggtxifppf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/giwkyxljj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/grpeubsav.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gmawiuroh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gbwzompng.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gomgcusyb.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gdcnotugq.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggayqxnmm.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/givsczrsx.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghrwzqcdf.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ggshvuutg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmzvtxwol.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/grcqhrhgl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/grrquoxqo.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gcbopuljx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gpwycozhr.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gdmvhdzuo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gvotagbph.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gltktsaro.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gjqwxwdnt.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gejbzzkip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gozcranjx.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gctehijqu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/ghhvaxhqp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/glixuhmlc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcrasyxkm.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gogisefvu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gezahdukr.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gtocbtzoa.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkbisxasa.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gxtkebhsg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gcrimqfdb.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gsnfuuhnm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghrnhtlwv.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gdihkoqmm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxgrfyjki.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gliaqfkkq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/givwglptr.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gqtykoajn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gcvwukybx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gafputmlu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdljegfxf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gfhomenkn.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gkbjeqmwz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gdomtetkp.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gepmiecqi.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggabnapoa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gubvqxbat.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/guedkxprj.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gzzsrvzhk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdtcuczyv.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gpzuzzass.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gkxxmfdzt.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/grorticoj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gaeejxbfu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gonlkmybm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gkexytxhv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gcvrwawol.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gikdqqwca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gdpmfbjdk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gbdfuakok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/ggteguxlm.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gyeyabthm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gblcrwibs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/ggfgbreic.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gxvfbbpyo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gkayczcqr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gsebwhdel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/ggpkurmsi.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gsvhoglat.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gyquqmbix.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gokrhawho.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gulriwymz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gjhfswoyo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gikyvdzkk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gbvcgzkbb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gknyzltgu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjcrmqitz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gplcupkfa.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gxkkqmcoc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/ghstvdtwd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/ggqcoofse.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gbonzqbao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gddcpthpg.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/goclhmstj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjjckckfn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnqbxgzgg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhltpvux.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gtocltfif.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gucxzhsgv.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gfpnppzad.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gdrngjpae.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gpwvgezfn.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gkiakoysy.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/guykcpyxx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ghsevqbch.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/glpahlmac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gfdlczdbc.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/grdqgojcl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gksiwmglc.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gepckemqi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gebzztuxj.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gfxwdmcnt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcwqylnqr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gtrlmqhsd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gpoagwirj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfuhsuewz.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gsdzcywug.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gksyptqhe.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gqsauwdxg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gaxvgvvsy.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gvegnxowl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gmgzqjqje.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gtomzcozv.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gmvoindzv.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gvgiukeno.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gmnxopfay.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/ggunioirz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gtmghcfzg.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gyagcltjh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gstkkqinn.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gbqfsavgl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gulsbmvql.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/giobdqoll.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gnaoszjmm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gwfloudmh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/ggzawphhp.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/glvtalygs.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gmphymfix.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gnwbefcio.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gkkhxnyep.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcpupoxyw.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gqmqemydb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/ggxhyxymj.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gsylnqzsl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gwgqgoxow.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gmxwqtmxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grohwnfzz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/glqboxmyh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/ghioflzte.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/glklpafty.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gkgglnzci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/grlhootji.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gigtzsamz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/ggnkphfkp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gfapnnkkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gauemdjkj.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gcrnrevqb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpivehljj.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gwgxngacv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grazohxzz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gfaqvswiv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gklhxnxog.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gnhkihlnt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goxdfpzqc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gvnxzgqpt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gywbuqcst.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gifgcchne.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gbjmwduqd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gcdrsnybg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gcefvuinv.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gczzkiuvb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gsdbvehsr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/ggtempodq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/ggqyofxrt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gngbijdaf.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gdyevibws.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gcbhhzgig.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gndgxoicz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/ggxynjoyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goqstsadw.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gqokfhykj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gglcxeeee.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gucsuxqtj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfuucnx.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gbekpyoas.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gkxaehcyo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/goathyxqs.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gjqzuiyck.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/guvhexukt.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gkjvvvevt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gthdzyiss.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gwrcdkfwf.sHtML


<!-- 参考信息 -->