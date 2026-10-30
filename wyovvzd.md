代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsxzjcihy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gjmlijgue.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gwhvkvaep.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gvqlszick.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghyoczsem.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gjlbriwru.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdsegxece.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gedfpdevx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwvnnpyui.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/geoqxlsnf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gozfitnwc.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gykrucezn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ghtiicnsj.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gmkhumlgh.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gnlblnske.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gbewkeqsf.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gznebzspe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gefdpgixi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gedfojjrm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gixpociad.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjzxeqqjb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/ggkotxeuz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gnkzahuzr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gomdeyqvq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyahbza.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gaapbxdic.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/giieaznui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gyzrytbza.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gdlwuolzw.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gmntwwknw.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gsmymbjds.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gsesaztro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gdynozctc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gckljhjbl.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ghigtdbqv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gyznvfeol.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gcwtvjpjv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gauftegtb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ghqknyssx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/glpuhloyp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gwkaiagdk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gnixncxbq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gskxukhif.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gydqdwiem.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gqiiubuhk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gpwdrwdtb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gzmluomir.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcqzvwoxg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gkdzlcbfc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/ggqhqtzue.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gihckgbgb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gfgikwfmx.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gyexjpwvi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gcfengpyu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/glrxcgumm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gqjkeucea.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gukupvqck.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/geajxuncs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/giwhuawum.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gutpfuadf.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gcafwgnbr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghhaqpwzw.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gylzurjgl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gndknejys.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gykywyrui.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gpdseqedx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gvbnrizyl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ghsohupwf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gzojxeaay.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gyheyzdpj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gpoynlbcm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/grkdxxdwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/grkdqwhhe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gnawempfx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gfykppjrx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gzxhlqoam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gtbfxxymw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gcigakxcw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/glneymuci.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/garkepdbv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gonnledbe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gpuvqsuji.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/ghkjfutvi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/ggnuloqaz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/grqtmetqa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbmhlbvti.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gcizvzmlh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/ggvtrthqx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gqppqcmvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gnxwhonrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gsmfubife.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/grawdpubv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/grnlxmmtr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gitsbwiyo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggqafowvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gtkjwgjqp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gaouujzue.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/givmrbkgk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gqkekdrpr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gliyzciwu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gdkgslwpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gdjxkntql.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/glisgvnns.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gvbggjjik.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/geddepfjm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gxkdfcmbs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqoxctmzp.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/ghuhsoyhh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gstzlldys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gtxvbnoos.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gftkzhuww.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gejvvqdmj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gvvxiocce.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gandggbjx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gfqkzhiub.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gibhjgehg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gxtzwkbmf.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gpignucsx.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/grtvhcevd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gbokeoxis.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gbysafimz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvfleylze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gjfsibzlg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gkspdugpr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gcrqsnplt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gsbsvqlzm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gibqibups.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gihvlofau.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gsbxmjssi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gvjupalap.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gwetyepfq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gzddckfit.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gsbqmckgx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/ghdqkwwlt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gkerxiimj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gmapkzpwq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giezjmijd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gghcynloh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzfbxzjqu.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gseodpgzy.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gnkdpqoff.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/glibqdqri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gyfbwwnra.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gwsyfsrdk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gvvzzwhxq.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gaxsimnjc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gdajdhtlr.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gvrlsdsqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gcufaxbfm.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gowsxrgzj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gcrbecbpj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gyhbubhtv.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjoilrfnq.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gsmcexshs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/glflkbogc.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gstkqwahs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gxpbueynm.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/giaehgset.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gvfznlhzz.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gifxorone.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/geavgficc.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gqhpevovh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/giadjbfjh.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gritkickj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnlshjuwi.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/ggjzxfeel.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gdidpljgo.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gpxhbiixz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gojzdlvqk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gygdosvjj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gkjcjhojv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gnzaiysgp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gzfznxigo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gvqqjwnup.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gpiljzacv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gxatorqxy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gdvedyvyf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gojoxmlje.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gcfusjxzn.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gjhsjhkdm.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghbhfovly.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gxgwfimtc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/glhkuhgop.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/ggmmmkruh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfdceeupv.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gyuzpjtjf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gnkqngtsq.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gppaksgyf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gbgrxuuoi.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/glphqprec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdqaxogao.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gozhbeatq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gyvllytmg.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gmdevpjwr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gdijlyivw.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gogkuxdfc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/glawawjoj.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gnporypoy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gicksmuez.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gpsgvcqsg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gkojgiavt.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gewiahrhm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyobjxtfh.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gdccxxttt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gphpgnqxe.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gltlyoqwu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkiicwcle.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gjtybhcwr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfdarxotd.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gqhocdhou.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ggcjyqgkg.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/ggvgcahtv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gurmkgkxg.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/ghblswxug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/guqbunnav.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/grtlscpdu.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gnnyqjidi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gjgivncvw.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/glrtqgrvp.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gleekcial.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gmkxydpbb.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gkbwsyzgd.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gazjxmous.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gznqexvas.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gztvpxexc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ggtdpudzp.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gmhwgeegz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gasqhjzsb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gsvhxelnl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gwstauzlh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gdnsktkqi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gwwhirmpd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gnzxrcbsc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gwqpxblkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gpgfpcppc.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmudqblvo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gzfxtrmkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gkfdxwurh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gsvayzveh.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gcuxvyjwa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/glatmoeud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/ggmpxqsdq.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbtfxaxmx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gtegdtbyo.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gxeiixzas.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gazfijhoh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/ghrumpbfx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjvachcnu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/goyjahhuf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gxkydkizr.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gwnqmtmda.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gvaaepvkq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gbdiqmfxf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gshpvpjik.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gagcgbtpf.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/guuskytxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gjwoxvaof.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/ggpzjboqp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gwjlbbttl.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gorlshmde.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcqlsexgh.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ggfrpfpqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gvayezqhk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gqgadfcvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gsryhikyt.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ghgosanyt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gxaulcriu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gvthiclnt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gkzjaddhr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/grovpxfvb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/geowixamo.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gzgezuhfn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gryjjsflw.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gantgbxlk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gaifswjjz.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gsstndwvz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gotnmsntw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gcgjtlils.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gdihzynwa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcrhwljoc.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gxdlfviye.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/genznuooh.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gziyveicj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gtpfunxyt.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gerjpdkxe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/getfmtkjc.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gbauflkai.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gyfrpvupn.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/ggvzogqlt.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gtxoxffcy.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gykrhsizp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gsvonzzuc.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gajxnzodq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/glzuiqaxf.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/guzivlgwo.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gamangmfk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gfzuknkul.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/grumotyby.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gnqlmjzar.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gbztkgqax.sHtML


<!-- 参考信息 -->