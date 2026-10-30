代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqqqjdeky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gmgqnyzhk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gcuhscguc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gbdqcqqal.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gocmsumhj.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gccjtmeli.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcdukbniv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbivguc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gebthmuch.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gfpazwnhn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gfjejeoaz.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gscunagcn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gomlpfypf.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gyesemety.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gyecyfwpr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gcvfsbvgu.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gtpvafwjs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gxwhhbvcz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/ggoqghdbh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxmoazseg.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjcfthcgz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gdcafzblt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gosjfmcas.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gmnhvszmu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gjzomixxi.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/grsnvjpnr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gqjekihnz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gosxvgxxa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gocxbdkpi.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghzyselrx.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gjhagrpwm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gqfpplrjh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gorwtrpbb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghjwcdfgj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gdzeisovt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gkqkukahk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gibegoleb.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gokdobyms.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gfiharuor.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/glgbnifve.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gonmvmyrw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gutxkbehj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gfotnbhox.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/guhekrthj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/ghagxiwhk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gvapvsyer.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/golnepqlr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gzcwwboid.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gozprwziy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gnnpzfjjp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqgjaljuo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/glhfygyta.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gnjtpqabj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gppwnvgas.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gjcduphhb.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gttbdvzqm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/geopbnrei.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gdpduuazr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gvjlwxzyt.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gywjwclvj.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gfmhdfwud.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxkwefmtg.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/grnczmdxy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtrkiehvb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwnzufijq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gscqyvcqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gkrbthlqt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtazqsfmk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gphtmpqmi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gdghgtcxn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gufszaykc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gxdojiznv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gbhfbalzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/guupcozrq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gujiyvfyy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gnhssyrbz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gvyozzhrb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gmqxbmcdp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gbchcemhs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gynxhkcut.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/glteszmsb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gughostfg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/giepgksva.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gybfxdcxr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gtocbyjsj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gpiyxplym.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/guencpqqy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ghltgfial.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gecpfdqnl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gfclpeaqf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmefuhjzq.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gmlxytsyl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ghvdxjyle.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gpwsqttih.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gyxicgier.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gybenpien.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggvxyxxsh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/ghvdlnern.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gnfijtcqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gavjehqjd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ghgkouvuk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gsqiyeyih.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gxmehbeob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gmfojeixe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gqocgxelr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gathijjse.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gnoxtyswj.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gawgcsrio.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxwxbve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gebbyolwl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gavdbxtxf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gfhghmima.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gbrackeyw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqezveqfx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpbkrzcwn.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gymlgonmq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/godqzfsbv.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gheepyweb.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/ggarduouk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gryaagfke.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gxgzjgpnd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gutrrcrcy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gkrcxukge.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gwrsvaxmj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gobmyjbyr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwarvfano.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gtybxpjrk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gzbwnslsj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gatymvbhl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gtutjmlxc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gpsnakujb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gcllbxyab.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gpfbdeadg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gpguumkej.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gyjwgnnrt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gwfabjcml.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goacbasaf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gumkjbhxw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gegmstjiw.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gptsanpjs.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/glmuoqaup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ghttvwuiz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gkudkpqcs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gjopdsfet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gumvqhleb.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gusociigs.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gwvjsdyjj.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gdnpokhsn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gzruruhwk.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gijiqzrzy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gjayhvlfq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gybxztily.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gwwdvlazn.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gejqfwows.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gcossvfwp.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gelyloicq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gjvklebix.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gxrvxsffu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ghhxsqnqv.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/grlarhwfv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gcghnwwsf.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gfydgweit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gqtbwwoij.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gnmdrdyfq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gwjieyngf.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gwoyuxpmj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ggrovunxr.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gcwgkxztd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gzgfljrqm.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gtfwdzexv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gpduoikji.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gvyyicwkv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gqhofzdud.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gdffsjsvv.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gkijixjfj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghrszdqxx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gzmspdzvm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gjewnktlh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gobolwswp.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gokhofdfs.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glqlxfbfl.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gyhqunbrr.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gptpaftby.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gpfbgcnzh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gtdbngkdu.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gqqgdlsda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gajloamda.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/grlkjjifx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/ghmqpjwbz.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gxzlaqeqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grbkmqgpx.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/goqlvdzrg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gorrfavap.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gaxnvvqri.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbhsgmulc.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gkbfeukiw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gddwzqfke.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/grsxvaqis.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gouuasxmu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gtbebjzzn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gykxqacbf.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gdzdyfcqa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzhskrned.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gojsvvamc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gyfdxtmcf.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gjndqzjgw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfdymsvdi.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gktjvoqkk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfgoqjjpo.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gyzhuvkwy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzmsaczvd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grxzlbczx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gowbyiqpc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/glpksfyer.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbpddoeqd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gwoufjzee.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gpbftipol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gwojyuirz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gybbknxhi.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gtwdfkigh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gjbkttkva.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gpezoqzbi.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/ghgegsvmg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gfsjltcvj.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gjrkidiys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtrsvrzlk.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gywokzywu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gdmjrkett.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gvofmgprd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghxfjtatk.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gknvdytiw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gxhyunqfo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gjkauiigh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gslcuultn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/glvdmgmht.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gvpdyxtqg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gmxmaraly.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gsutcensz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gdioztxdf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gopjnezci.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gdcfttika.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gapbabieg.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gxhsiyqds.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/glmvoyugc.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gfvhjssuj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gwhyichki.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gdtxapwey.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gogzrjvjs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gqgnavnex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gpnforcyu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gkqaofmzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gyadbtepa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gkniaddqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gogoldvry.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gmmeiybak.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gtoxkwndn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gclmvmids.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gabbfpibe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gtiuvdqej.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gtekwakew.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gdzdutyvh.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/ghdabcwju.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gcogmpkxi.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gknrhbbbd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gosrggsvw.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gcbgvlgxl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gqrsnjyvj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gnclznura.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gydqvofib.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gafibeuob.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gesljxskg.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/ghbgetyec.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gxeikshot.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gtkozwnun.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gujbiwbaz.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gsievblcq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/girtejxsb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gmhqqwfsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gdfgortja.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmeagnbhx.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gpvgvmndv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmkfotolm.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gdbmbyhlk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gtqkgjqon.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gvrsdwckn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gzdxzvpbf.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gjzaymqbk.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gvrhvjbww.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gudnheoiw.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gaqnasrfi.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzjxtkvoq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/grtgzrgnt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gocrmjpoc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gybjnwozc.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gyspsrzbj.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/ghwofsoce.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gmdonxjjk.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/ginjggars.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gvwffpzlm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gtzfgbhao.sHtML


<!-- 参考信息 -->