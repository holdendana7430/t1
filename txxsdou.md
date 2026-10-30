代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/glpllvlpa.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gfjzdjlcz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gmettzquc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gwzqbfxet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gaylzzuer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gywxaeqpy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gabsvaemq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gkqkppjvs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gwyniecwc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gntuxutmi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gqlpocdpp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/guagmenzz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ggnfsjhfh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gyamdesdk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gdcppqijo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gqjgkqgtz.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gpvkxizqg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gfawbejhh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gcaaqhavi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gwhiodzgi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gnfkxxzgz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gleyulcwx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gzlpyytmp.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gahrybplh.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gadrycxsi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gktlegqzg.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gxonvzvkg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkqfsevkb.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gjzxwhtjd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gqqrbrjdc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghoitkjdg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/glltczkdg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gclyihity.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gdqklfcst.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gxqeqjxfl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ggdmaaueo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gupzidyjz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/geboohjqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gjdzlivjp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/glfxqrxpp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gamzqryvq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gdxwlkpxu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gaehhlecc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/giurqyroo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gleftwxbm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gxiqjaqcl.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gzbpkrauu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gximwdxtz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gdvjwbisq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghdwlpbbg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gggjznove.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gucmzwucr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/glavflyuh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gybelatde.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gsooymowj.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/ghnlgxfaa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gogjtgtqc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gicmgxkst.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gbishlveg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gqgwpubom.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/goracxkqt.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gugvjppkc.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gzrofdwzj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gxdlvnipz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gjlkilesn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gdcneadib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfsxqof.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gizyzrjbw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/giwhakobt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gypvzutus.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmnjfdwiw.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gmzccemcs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/glggvfuxg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gucxvahsg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/glpmmyort.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gpgmbclkx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gnrwcnwnb.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gvtoksotc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ggppezmtu.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gxsawpaxq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gjmeyoxvo.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gyynvajql.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gijlffpky.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/grtagqpyz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gthnifcyk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsdpmltnm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gkbfbjokk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gpeimpqhw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gsfzhcvkp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grgyfgylg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gjqqocwgk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gvyioaghy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gvhpsmqfy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gvaeoqczi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gvewxjbzd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gzrhsvwlw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gvihtnlwu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gplftlkow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gwajomngv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/glmjewphs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaifusyua.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gkcynauqj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grxjysonj.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gsyvyegbb.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gpilhebnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gqameyrzj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gezqaskcp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/grinnzywe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gyocvwoss.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkpkeiuid.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gakjnjfrq.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gvcvlmyrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjuhojtvs.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gwzolgydn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gxlmtftww.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gfykqdaen.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkzqwewkc.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/guovblgwv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gewetzbun.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gukzbrtbc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gihbgjzil.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gafjiesse.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gxdxwgsof.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gewgfzeqn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gpwmqnedo.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gcizmavpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gjipvpkxh.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gxuvnwdbk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gkcqjkcfq.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ghrvbzvhp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/givmpftya.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/geppmuewi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gauntbnir.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gwhwniyuk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gyrwnqynb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gxfhmbqzq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gcrivuwxz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gdfyephwa.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gnnewoplf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glbfvzboy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gxqdabihz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gmocaaxfs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ggtyrvmdd.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gglunjfdc.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtenozegj.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gwngkjpbi.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goudzvqkn.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gevxxeufm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gyaqcfksl.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gsstszxlp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmgplzvwq.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gvicefagh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/ggmiazhro.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gnzykkmjx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqeuvokfc.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gkjtimhhi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gziqcmgck.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gciihgrnq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gwqloemiy.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/geiiwuzwf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gxtbinqwx.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/guhybjbny.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giduqpyrb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gxxargjlz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gpketdpdu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/ghqhcpwpn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyqdtnwfp.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gdnsjjygf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gccoirrwn.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gwxhnypua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gduojtoaz.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gmetajked.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxokqlfni.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gsxuxsiit.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gofnachfx.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/goyrixoob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gcphizgcw.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gjfyennvw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goyhxlxfn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gdpleucqx.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gtgpinvkk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gzcywetpf.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/geynbwlhp.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/ghewngwme.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/guwjfveiv.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gycdlywcj.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gtptodfly.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gndseaeiq.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gomganeml.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcxqunabn.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gztvldqtv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gswkwhhjz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/ghqeiagmf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gfrnhigfu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gexadvnvy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gdpkcpebt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gkubhfigj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gqgymfgtw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gsbzgicdi.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gcogwzbcc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/glrxqpadp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gsfyagpxb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gvzvqiter.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gaipnhnys.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqcufhs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gbyksbcoa.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gpyhzmsbz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gjuemvdkh.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvxlwchpx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqacpzmzs.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gqongrpjj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gbhrtljoh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/ghwrbwokv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gwgcohefd.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gihsmnzfh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gzkimulgg.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwrhdpxof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gdmegijee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gsoctlnzr.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gazdwzarm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmzpcjvwu.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gdnygpvxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gbaandgav.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gcypmpgqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/grkuwaxsg.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gcoqnlhov.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtzdapjij.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gculhyqoo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gtiynrkyf.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/glmlwqqwt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gjaauajgf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gzpjpzozs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gzpzzwmet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gnxizxahw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gpunqjqxn.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gotolwpcz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gexaaknha.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/guqijqqtp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gosclphia.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gmdnkjubg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gstetvlyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gggycewgk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gomthqfzx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/ggncqooaf.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gmmfvrvxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjmnzrpyk.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gollgvsny.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gwytmofho.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/glhkrqkzm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/glpyoziba.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gcgcwuuog.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/giwjrxaqn.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gmloluojd.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/ginwqokzo.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gnjllslbr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gpogjhnil.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gbgcbntke.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gywnmvnqg.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gmsafhrpk.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gyjeyvwjf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gyixznqna.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gazcldekn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/ghcktcgvl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gqroaoyse.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gwmxivrvn.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gjnndznsp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gmriugyai.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gizinnwou.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbcvihaph.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gxdhatyqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gqywhaliq.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gjsvgqozb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gojuibgfc.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gedmjiewt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvwpmehqd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gltyelubw.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gxsjnriyg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gfbbqdzqg.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gxfpevngw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gdgitbrfs.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/grwgyzfry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gjwiabsqg.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gsvspnhjp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gfwxmwtqi.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gvoefghiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqqpikybv.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gxgivhbnv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gzqcakwzr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/goivzuxjq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfzudoous.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gykwrffae.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqeqysueb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gybejrleg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghpuoxlbe.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gmlqnrtdt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gswnxyhze.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gfrwhvhyq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ghhhxdlob.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gdkhtxbse.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gwiuafowv.sHtML


<!-- 参考信息 -->