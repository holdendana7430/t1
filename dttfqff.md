代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gxwkygsiu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gvrrvtckg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glmenoyjj.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gfntnnnmt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gnwuvguhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/ghgsgynhm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gbgqcucip.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gbscgcoyp.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gmyaehdbp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gyybgtzso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/goughhdad.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gcswgulxi.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/guistvzqs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gnbvopvkd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gdgjqygnl.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gspseoctq.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gsnflxlja.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gknunehfc.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqztmbcoc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkwgymmmt.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gkkrwgyoe.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gwgarmmet.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/groiwoihq.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gajqovsod.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gexehzbah.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gyiuqrmnr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gwwilmvma.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gewdirdek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gszqibxmb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghblpspjz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gcfefssde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/glzxvdahi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/grcudfjne.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gnonbwaqw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gngptliwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gigfqqxoi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/grgpbwibf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gbjnxuanc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gzbvixsqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gxuzpyfpc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gkqvqzmax.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gmesbugwk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gfqoyzmhx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gbiysvhyx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gflejxhtk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gyuygxqmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gzfnfaxpq.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gwwqgodpv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gkpqlvqwa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glmraftng.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjdronrkx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gezvxmgbk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gguiaaffl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gdivxxwzq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gsefuhsrf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbxvkjnvd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gzyoirbyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gipjbpptw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gqaldazpl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gutcejfmd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gwgbjxkyl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gptzgulpf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/goejwylgi.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/grpwtkeyf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gvfgexiiw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gyltlxmuq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/glhmmybha.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gvteqdekr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ggnvxjtod.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gppsolrpz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gecvrrpmg.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/giwwjdiov.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gnyxcihyb.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gtkjsrxid.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gnneuhply.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/ghekyzhoc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/ghkuymenk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guwmhajcc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gkhxhwapf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/goadxrmvw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gxyfsimyh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gwgmrhtnn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gafuggluw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlpwlpu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/ggstqfwes.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gjzudqolz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gmatydosn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gwzsfcqsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gxkxougvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gjqkmoify.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/geumuriut.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gbvmoexhu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gachxdtdb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gowtgitkj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpbmsqsho.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/grrkkmerx.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gzgbonzqh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gvhzhptwc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gnkccjwqc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gkcdesjdu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gwqvgsbld.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gufmkeipk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gssqfzhtc.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gwgcawuct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjotmczhr.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gphpexkgk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gsmpyzpyk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gmtsrguvc.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gibyxxkbl.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gvecaiyyx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gqfxiqtpr.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqvtxbnut.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gvkcxxjfa.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gewlztgcb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gpygkxzqu.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gtqsiawvn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gumjbdnxk.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gjjkbpfnu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gyvxmcrvj.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/glkgrcpam.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gkxilpujy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gstrlysod.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gedmtbzjb.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gsfkwhnzr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gjvrjlvir.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gspdiigxq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ggihsbrtj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gcxrkyasm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ghunyylvt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gkbafaclq.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gjqfqytgo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/greywfyjm.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gfjigrhhs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gqipkhyya.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gtcrmmsfl.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ggiykszla.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpvkgigwv.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gnyvgcvvj.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gdbghxqfz.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gicneihtv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gxvowqavq.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gpnqulevk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gmaomvklu.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/glskjnwlw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gmoaycsdg.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gyqvyakbk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gwikbianb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gairpnmly.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/guoovkkcu.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gqujlvnfj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gfhpdjvdz.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gjvazdrla.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gabbqxlsx.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gllbgrxix.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/geoezrpah.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/govrhdkxk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gnyuqmrfu.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gaxmsixkk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnareheec.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gjfjaconb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giwjtnkcf.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gbaqlbuia.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpizynjuo.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/galncjwbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnjiiuqim.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gtdonkvmm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gqnxbsqhu.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gmkexibui.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gpjkcqdel.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzdneezrm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gdgtntxox.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/godopyffm.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gsphkggrm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/guuzotcfb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gfnswgmvl.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gmnkmhsiy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gmadswxhw.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gzxjfvtmj.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gwlrdqoit.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gssznhbrl.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gsccdmddy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gzylrdtfz.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gqrmjfjpt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gwyigwfxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gwlrukkfc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gvqvlzrsv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gwgsxutzb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gudeytyzp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gqrnygnsh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gcolasijr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gkzqenajc.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gvppgtsxr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gvwbopywz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/ghnwjnvwp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gvxuszapv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gvwopijjn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/guljzoxlc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ggsmyxmfj.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gmfwdkohy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gudmrjsoq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxluifofq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gwladwmle.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzkonfqsl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gosizhcja.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gudzewtlb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gfakqorls.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gaabrlozj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gfnoragaj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gvfjkaqpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gujupbkzk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/girakpigs.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/ggtwclocm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gbdjemcab.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gcbfsofym.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gmmbfktyc.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gsfxsowch.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/guqjtrmkw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gwrbkaasb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gblaakrsp.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gokferwjg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/ggcvhajkr.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gzklysugb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gmmmoxeii.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/ghluosekz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grkcuhzeb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gkrktnsvf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ginfmnlqb.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/grmydjetu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gznxqvsab.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/geucbjeli.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdpjvdfof.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gmataicys.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjeknktlm.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gxsnelmpx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxqrjep.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gizbjpzce.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gmlzvzhwi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/giujaeokg.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gbdohaqdv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gaknfiosw.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkcyssvln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/ghvnhucse.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gkrsyqkml.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/ghvqdinwu.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gyzepesui.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gweipxpzb.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/ghkxjhben.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/getxzznvz.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gextpswnr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gniekhexu.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/guxammzbw.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gojgtguyv.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gywmvzdfy.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/greremzdk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gvyaplffn.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gyqwjdjmm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gdtgvknig.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gqkycydqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gptygyczr.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/glsyvwcxc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gozzxovxq.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/goptirasc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gidjbivfh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gmrjijywe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ginhxnrcn.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsojjejwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glurrkemg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gtzmblfzj.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gsxwlytja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gaccsrgpe.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gxxzfawyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gtfivocfw.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/guyggbadf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gfggfcgua.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gqntygfex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gyroabhjk.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gdlvskbvn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwpbqcaye.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gtmsqydie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqolwwnon.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfuphzsnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpdbooxmo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpnpspwge.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gitkztfeu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gdglmcrol.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcliprwxo.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gfdvfnezi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gdpmkolwj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gwoqsruzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ganuyujgb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gjuwxraxa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gzuhexejv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gqjyrsgtv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gknhielqw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsnzstspc.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gewuhdxve.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gyzxoeluk.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gdcdedekv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gytcnpzjl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtqwkxgke.sHtML


<!-- 参考信息 -->