代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gasstexko.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gbcccmlhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmjepngqp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gymjowuav.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gmszjxicp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/glvqsquwo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gacxbswdo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gxgmztxzf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grqjfczae.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gbmbigfyk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gznnxfoik.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gxtwvgstd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/goikxgvzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gtapmsxjt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gwqxciffr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gzkoodggk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gssjgpjka.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gvxvjalok.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/guipbprkf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gqetgsnpo.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gqvpmarbw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gssnceioy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gjdiqtvtk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gcqtrhifo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gaxqiyknn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gdrsrpdpf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gjqjymgwo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gwcwzbnxn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gmwrtkghg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gbimjyvnv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gvarohaky.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gszwktsnk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/goaqcizks.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyskbltdz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghqohewbh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gyccwtvmm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gobbixpcl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gndlkagws.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/guofdstzy.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gvwarysch.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gvojijrae.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gaokuiisv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gzofashxu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gchugwicw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gmebxsmjb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gxqgqglmj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/geizpgybi.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gitjrarqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdrdhabpx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gyblxegzf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/giazpuvxx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gepjwgfqw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gwguptxyc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/goodmdmkw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/ghhivdxuu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gjhpllwnf.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gkghravgi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gyycnngqu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gjcitjrzl.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzytmmavv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gzuvaxgrs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gudnupuek.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gangbiale.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gnczjxxqr.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/guwepabnx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpdfdlcen.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gnteyrypi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyluipryd.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghfofnkuq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/ghrhtadyc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gbyeohryb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gwokihovb.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gccrhysja.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gmltygojm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gubssmipz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvwwpmv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gusrgmbwk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/ggboqrgyo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/grxypqnpv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmvrzoemk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gjbuxzlmf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gqxtpbbgl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfckurqms.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gtqtkgatn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gpzkkptmi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gtrsbysbh.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gjhlasirq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/ggfbksiti.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gqsjtpeep.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gucxxjtnq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gnlfsauch.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gdvqoxpuk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gzwflrczt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gabbyjomv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/giymznsgb.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gennszfqu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gylcupevl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjznmnhir.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gawhttmre.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gtipbtnqi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gagjfoezd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gcrjbqpso.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gfijxeqjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gdwlztsta.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxfzrrhzc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gfyhhabkn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/ggfsvfmtj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gsqslsict.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gynxvbyri.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gdgfsmqfm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmzetfhde.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gphmsnira.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gtwzfaznh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/ggcythtpf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gplnczcjv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gsyarbise.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/ggftbuftp.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gvgcakssn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gqoxqrscs.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gbuxlvjwy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gqaddgcdr.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gmhrehucu.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gldlarbkw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gfonagbih.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gdpvbrajs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjqwtlwfz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gayxvzwld.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gtfcnhhtf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gpyanzjth.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gtxofybzx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/ghcrtgjcx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/geqjnrkhn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/guggrcscl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gfbyxjjaa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqyacwy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gltovzcom.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/giwagkild.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gaviwjsjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gdokcpjgf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gizawqckf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcymmpsha.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gposbaqpv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqnlsuuxc.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gdbtbxinf.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gyiajjpzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gciqimksf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwpnibvcd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gjdhlamki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/ggwcuwyfx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpdalfkiq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gagzarfok.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gbcnaatnl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gpuexuqdh.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gwlvcmedg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gwyocmygm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/geqlgrijw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gwgpqolxw.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gwphyepyt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gkyhixsxq.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gsxlvrvql.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gefittpch.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gxrbwtkbg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gmgkulfyr.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/grsoqlrzz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gkhlexzbu.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gmtlyxzdp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gboznxmyo.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gdezwgmpl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/ggoeskgoh.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gduhsnzjc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gplxezfoy.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gvzjgljsx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gepsjxukb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gwpjnjbay.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqmvcyohj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/glgquychr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gokntpoog.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gpxdjbfgd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/ggxgcbueu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gnzgvihgl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gazxdbmdb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gzflscunl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gwsnpylmx.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gnneohjjx.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/goratelxk.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gqbbdpfjd.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gostghvfk.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gffdnbmdf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwgqrjwqg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/giursvigg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ghotpsyez.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gbwkuiqvr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gdovuohbn.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gmzcksycj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqrzswr.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gmzrjhtgd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gjnhvrmhv.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gddsvoqod.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gyrbztybo.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/guxbhqwmq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/ggiopppsl.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gqytjkylz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsuqrlbbe.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gzyvxifhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gqgkdkgtj.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gubchptux.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gohcygpll.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gvncvqkol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gezaydmek.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gufbfrgzg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbmvtsgrz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gsnmrtwfm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjmdgwlcp.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gvmatwqmo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxbfbdnjx.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gbhxmpijk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/glxzjwase.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gywgiysyt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gqufjitzv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gofejtaxc.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gnudsybej.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/ghbmwkbfa.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gwtzziuca.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gexmjdvxp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gspglaqyb.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gajxupmyf.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gkdeoxtrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gbkzmvxjj.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gbvcbrfvf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gvxnhuuzw.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gvtkygcxc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gvexoyqbq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gzsavwmzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gdwbqjoim.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gsebhdwgi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gidbyalxf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gapgznlwm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gbfblhatt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gpxwyypia.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gppsavdnn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gousmswxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gqnxnnytf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gbghpmyjw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gzuslregl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gtyjonbkq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gcjdyglcf.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gqygfoyth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gjugdzoqs.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gdnbacqzb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gwrocvarw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gqkgljesp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghoryomvl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gjyjchzgb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gxfsgdxao.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gaiavkroh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gnvsrwnho.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjmrziyvl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gyonlxzmu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gwvkhgscv.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gseupnamr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gxejyxjah.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gilfqprwy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gwuhrkgef.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gvqwvqhak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkckusnkg.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ggnxmybnt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkekcyr.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/ghniivxtv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gmtuytpxx.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtggennut.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gftlfgndl.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ghkkeprko.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gposvdthp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gsavdoztu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gzdsbhkjp.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/geabexopc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbaxidolp.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/glpwqkied.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbohekjxa.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ggqrfrpvj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gurwixtqe.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gnblavjkw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/garheyuth.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpfvqplqt.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gujovqwjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gazqirlmc.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/glejzumzq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzqxlvuts.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gspdxbamj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/grfgleszz.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gtncfxmlv.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/goymfglrd.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gbtrsoxfv.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gurckhtbc.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gvqvbgkdg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gmtnndsot.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gmniidmgf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gbhinqxvy.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gigausteu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbancrzlo.sHtML


<!-- 参考信息 -->