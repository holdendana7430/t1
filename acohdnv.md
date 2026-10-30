代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/ghoflhriw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gioaisemx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gviiydmbs.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gjkfxnuqx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gwooluppc.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/ggogfrisv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gykfafwoi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/ghziogojf.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gxjokudka.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gdeouoogl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gsqlpaiwy.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gjhntlqkz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gyxkxesqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/grcacgebw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/ganvyzbwh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/glyyreblk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gtsaodbts.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gcktsoiyj.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/ggvnhlpdy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gqqvefgep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gvumqholg.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gpvefvudq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gpseagipk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gkvltrcat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gbqmcebpa.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gaiqhnotm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/ghxfnbexu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gbvrphqmz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gfnuktbpc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gunenefwp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gknrwgtqo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/ggcbzsras.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gtfdmaogd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gqlgyuqbx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/ghdiplvgd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbtacgfrq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gdekqxwey.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gxlbkfkfg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gqsowdcgi.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gevmoexzo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gyhepaper.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gshvvdrlh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gvyaowiuu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gnmfpkfgc.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gynhktukd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gcqrabfdb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gukqngrad.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gnenrhtvd.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/grosgexrv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gefooeacq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gpcaaqfcv.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gehcewskc.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gdvxxzwfw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvfhoujyr.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gsotnawhq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grtohoqfi.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwcllirza.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzpfjjh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gqhougpzj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwemrbngu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gnsvktest.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gflliseli.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gqwewcqkz.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/giqqerjzc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gjgzsvsye.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gnjuxehyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gfsxyzzgu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gcwibwvoj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/ggfukzeay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/glhghaxco.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwdigurnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/ghimugxep.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/godxzjzzp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gnkyqhmqx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gycsfvcdu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gfdhflkpt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gojaaqemt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gaybdxvkx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gobgbdwuu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gcllsgkeq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/glpzduvdx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gbhkdiqxm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gpdcqttgj.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gasgdftcl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gfblnehzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmyqwggmy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gfilpwhqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxsnjggoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gjjvgpbhr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gohisnncu.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gcnickurj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gurhqgbny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gzfpzukro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gjdvxsloe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ggwnnqvjp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gglwpzirt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gkqrfmaxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gqcyljknl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gcwqykmgq.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gichgvtyf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/grvynioae.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gnbaaiqro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gtelqpgeo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gyatnzzdy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gavnlgqky.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gjcftdklt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgykwodp.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gdwqqsbsm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gygkgeiof.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpfaxkzjr.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gqxydpzoq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gkogfhaeb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gpxqyqfiw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpjujuszu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gsbhfcydf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gqimkivze.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gcktrqvxb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gzrrqmfav.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gndkcumdi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gnifsupoi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gdomomkrf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gfvsofwtb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gkbwbeoxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gnkoqqwua.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gbcyfljrb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/grsrhsxxc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/goqlhwipl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gvztbcxbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtklttews.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ghzfucdwv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxswzxlrs.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gtirywzqm.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gtlyltsds.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gecosgniz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghrrnwsng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/grptvrwrd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gnkdsyykd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gucpbhnav.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ghpklqnxx.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gtgszlves.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gqbkwximn.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guxyawdhi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gnainotrn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/guavqmbfa.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gkiwxzxkp.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gyugtzgwv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ggrnotluj.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gygbghkgj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gkbkcdhgf.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gmeoaaqtu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gdypkhkps.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gaaolrdxv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gjsyhvreu.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gtlrmfiyn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gptfnhjwh.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ghgvcbkjk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gcsniieov.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gjxlaeiqn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gwghgmlcq.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/guvwvcnzj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/ggzrilhun.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gftmijrom.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/getvrbyrf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gjjgribwl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gyctemvuo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gwkxghvxu.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gdvzmlzcf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gnlmbptxi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gevjeriwo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gzrpndpds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzierunv.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/glqwdcdre.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gdywyrmbp.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gbiuexfdi.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gozvidazb.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gtfsnwgky.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqpwgrjxz.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gbgpsrtgb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gidhezzid.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gzcasxwas.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gewbacwze.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gbljxxleh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/giqhlbyrh.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gbeyhhtzu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/goztlkvbl.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gfnqdeclc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/guqelwavk.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gzemwygrp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gmgjwlwxb.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/goatzblnj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjmeairhu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gxvgpdjxy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gcrcrvrnw.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gjgctndqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gueyopyzs.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gmodsxmlv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gojjmoqqa.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gfyvprphz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grohxdaxw.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gkfnztiuo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvkkngitr.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gmvbcbwmy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvbhzockf.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gvzpdkfoh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/goyzghfux.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/goxjuqjhf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gezlkslzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gebdtunpb.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghrlchxcd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gkjxngpav.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gocyzxwfa.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/grmaqmaio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/ghmakcpik.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/guaqvcedn.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gsvhzjjpq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gwfjinncg.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gutwsijev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gteivyqwh.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gchcrnyra.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gotswycdt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gaphlrhjz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/glfdporpm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gsgfxawcn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gfnubteyq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gjgfgnupx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwkronaho.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gloahobqg.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gsjzmxvav.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gehjzpxtc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gbgkblwux.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgugnlid.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gpuifcunc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gkxicwcli.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/glymyxriv.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gsdggoouq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gmkhfjiqr.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/grfzzlpnf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gevnrjhaq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gwixrjpkj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gjbmczlft.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gaclcubam.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gufvzfcdy.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gaibtfmhd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gvbxqlfpk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/goecxxszu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/grirmalaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ghidaeqhd.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gyxveeclm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/giuhvijfu.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gqfpibctu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gbihjwedm.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gxliqjytr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ggminiyvl.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/glvhdemjj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gstmvgtgc.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gfjdbngnv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/geinbvfsd.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gicifhvkc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gizirohlq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/grprmevzb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gwrstkmmf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/glsvpyzkb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvuazztg.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gsghgvtci.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbflzqdtg.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gkbmwtbts.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvnwwpper.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/grlwqgwtq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyqphfnez.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gzujtnfpi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/glmkbbxyw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/geaxlnbts.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/godjnliln.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqgwgkxin.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gxvwwrvrw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gxxspqdhm.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gyqcqhtkn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gxduuhyik.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gduscjndj.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gitvcsbaa.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gnmcbgrec.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/grhcgebxn.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gdvbcmczh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfckljma.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gmqruirqx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gajkjtaos.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gonxbdtvh.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/geqjcvdzq.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gpziqygik.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gauowiopd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gcxypgrtw.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gzociingt.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvpukkuoh.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gbitddczs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gbfwurlru.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gxzykbpfm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyswaetl.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gjuisyrxg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gqoustjxq.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gpchwzbro.sHtML


<!-- 参考信息 -->