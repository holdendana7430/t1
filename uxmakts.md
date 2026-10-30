代发 wailian999

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gxshxbrmb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gdpgqnskj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gtlntwuui.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/giunwwikk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gydpednze.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gxjuwgxit.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gqspozgun.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gpddtovlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gsghtzafm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gbszsinbu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/ghjkctpwl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gzuaajfgm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gocsmigxk.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gevxkdxtj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/grrobkaxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gclmdiuif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gltohkzrw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gqjcmkoua.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/giuzxybyi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzzbqnc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gxbuyqdeo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gzgutswbt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gbfvajfip.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gdquqjdpp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gwtfhowyy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbhjtlwgm.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gkvlwrwjf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/giinihfuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/greasxrqg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/goehhgsak.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gzquwvwuo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghjhulyae.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glfbabavx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gdisfegfc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoaucxba.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gizyfwlqg.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gkkebsynn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/ggnfhilcm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gvubmdabv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gdpwprwrm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gkafzrooc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/grtqmpxvm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/glvhlscoc.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gbblsagaw.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gnbixespo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvaczkfmz.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gezxgzyjc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmkkrynbt.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gsvjotape.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gqpfsnozh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gchdagcml.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gskvpzqoi.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gsdxjidsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gsxowfkfv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gsjrnlvur.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gjosqxnvl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/guvkycbki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/ggrwvmzhs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gbuwloydw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/geqnfjxen.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gmeisamxn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gwhymaseo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ggkayidze.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gbroocqwi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqitgxij.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gfcjzjybu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/geloylbyi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gntgvaqqz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gzezemjla.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gufwoguqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/glhtynobe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gtcbowinq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/ggtueyejx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gqsvhqnyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gbcteysrx.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gqlyosqyd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gahqgdeic.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gouokqetx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gvsrbtqdw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvsqtlocp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gwhjphxqg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gctxvothd.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gaeuhcdbc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gnfvdryqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gcvatkzzr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gxthvohyg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gbymbqneh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gjrmriycu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gwqxcamof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/giqfampat.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/guufpsmac.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/ghxubqvyi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gunsvcsse.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gzpicnmvh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gznhafutx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/guxtxtcwm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/golychfkf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gymkmkvop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnyvjkbeq.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gvcekboql.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/guyxinjgt.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gcytrzuxm.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gfcogswwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gvzihwjbu.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gkhhbemtm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdkoysypp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/guecaoobi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/grmuudinu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gtmdchoca.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gqaggwrun.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/ggshjptly.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gsqvpzmfm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gimwaucsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gtenfqgwz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gmxpcvjog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gmqfieicl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gpsrjhrme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gqldlqnki.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/ghzknusme.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gbezsbugi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gijcniqke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gpscsgbtt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goutgahvu.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gnzbkjqnk.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gxenswoub.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gouepapbl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gebxthdsa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gpcjyvtet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gmkvkrgyl.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gztbfqfek.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gtalhxwox.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/ggbqhbdry.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/grfebrcgp.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gxpyixyeb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gjlqysdzp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gjdnqqqul.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gottvwteb.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gpwdjbhao.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/ggixflkyw.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/golewscdf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gspogpevw.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gkmtueypp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/glropfxdm.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/ggwssbdwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggvjcoorv.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gqdkmqokv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gvepubwae.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gnpzbiudd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/grwnijtlx.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gydlunemy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtiytzyzu.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gtuukaicz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gklnvolxn.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gysmipubd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gffolmrry.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gstbysakf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gjyulhnai.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gtyfptxfa.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gsttplqsk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/guiztziaj.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gwsjyucze.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gbtwzynvf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/giqlbsdng.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gzmtraxcz.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gfudjaveq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grrsqdpbs.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvjlolkdt.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gqhqcythd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/geaqakukk.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gbgmqiyde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/goypaaqye.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gqiaxlmun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gcnlhivcz.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gheckdaah.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/ghynwgyxk.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gnrfekoda.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gpejmesnj.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gphxonmsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gujzonzqt.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gdjhwhkiv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gyhhowuwb.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/giulvbcdl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggjquzrin.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gfoomiqgy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gjizmlkgl.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gmiftlbyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guielbbgh.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gixndjmtq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/guzaqftyr.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/graacuimo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkfddgqqs.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gewwaabym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guuuxskug.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gsgmoyquv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gflquxmns.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gncfcbxbu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/glvhzpjim.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gvkfueuzo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwjhfeoob.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gqjposbzo.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ghcguxfim.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/glvhpemir.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gtlsqrxnr.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/ghugxjdak.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gyildrycu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwflhsi.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gxshxbkni.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gblpdkwfu.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/giworxzcs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gkeqpuvzo.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gfdybrufz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gszzzqois.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gckmlbfvz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gzvnjhcxq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gbuiamkds.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gmipguhth.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/golhcpakp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gpiqhsozy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gqrgpflff.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gdowuloze.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gpqhgaasc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/golokldog.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gpshdziav.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gyfbexvuo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gbobxryys.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/geeplyfpi.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gczkaayef.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gjndkgriw.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmlvqgzgm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/ggefvlaoz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/ghflcjtnx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gtempccxd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gwzzvqwut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gnjmuiqqw.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gguydvlgr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqyuloqc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gnnfubixc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gbiubojek.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghxoqowgi.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gofdmaiyj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/guxzxxgeo.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gcwynfrty.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gqpwemitn.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gofeottpv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gymplxaph.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gsqhrmece.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ghroomkhg.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gazcgeboy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/glabhryto.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gjlyjgrbs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gcncpzhws.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gcfgtpjxl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gajncuvum.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/glmuckbgf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjsbqvyvq.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gddwivoxe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gkaigbftm.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gpcvxqmfm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdpsgowoy.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gjlddpxed.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guvzpxzue.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gaaxgeicm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gzgluegxs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggmsknzyb.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gwkugzyyc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gshoxlvfd.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/geyjshmmy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gqmltkiqw.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gebzayxab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gpvwghljh.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gkvibhxko.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ggghfjfkw.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/glkxzrwvb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gxnokorww.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gwhpxbtgj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/giaksortm.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gmpjxfoyk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gmyevmlyk.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gzrkeybsr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/ggxxcufnv.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gesylzszx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gzjjdiozt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gikxhodqs.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/grqnmnxre.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/geimeerqe.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gelienggz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/giecrulrv.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gaupfojjl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmsxwuhvf.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/glnkuywnb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gffwjzeqe.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gjzijwsst.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gzggtqsot.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gdixyjvjj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfyhirfws.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gxmydkcgg.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ggfssznuz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/grdomktxr.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/guouwynlr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gskbgdsnp.sHtML


<!-- 参考信息 -->