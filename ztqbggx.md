代发 wailian999

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoispgkz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gazvczoio.sHtML

C#:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gknwbovod.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfubwwroo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gxapampkq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gqtimfsip.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gajndojqt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gpjhqbmyn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/grjnyrvsn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqudtjdwy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gbiggdjaq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/goesvrirm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxnfaln.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gfsxeerce.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggkuqqdlb.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxescmy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacgnejfm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gikbnpmdb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/gskvdpzug.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/geoycffig.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gksvdssge.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclyjgbll.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gagsfxgkm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrmzozsh.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmjfjzps.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsutaqqz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvklgiki.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsmbyfef.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gxkctgbuw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/grwhmiaqp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gnterwvmd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbhddzbl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxtybosn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fanxiaobao.xyz/Article/details/gumkbuanz.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggfkeskfm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grblvnspa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/glqsvdwyg.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvfqjdjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjstbqd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gozpoyekg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxlliuh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmplssqcw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbmuwdou.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/glggolaje.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gknrfhdca.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybhzizwt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbycpjqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfanjgsv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmcunwkl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxtahyd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqnlmti.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/grzrxrkoi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gidshvfni.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/grtckltbs.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/grpikbkvp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfsftdsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/grkjlfphh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuriaetr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdfbark.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadsdvsbd.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjuoqkqy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcvvtdti.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/ghjibixkl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gkhdneqxx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgbrakjj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnaxuvdr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gvsrqsysz.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxgzujvr.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gkesuaxwt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gayqgnmpa.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvnmguzyu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmalqeamg.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gduugkbfd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqcknfvf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxeksbrb.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktptneo.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfeavvi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmgvwfh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/giafhyfrx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwbzcnm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdlekqr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/gdngdvmsz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdmvudmm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gomyslclk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gjxmkxlns.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyfpqghp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gisavrxcu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcmzceqx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkvsvtszx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/gmwkxpcnt.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsztroeeu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrwiibte.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/ghvsoornf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gdooluwci.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccmtzulm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmrirtxo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/gauxiksht.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaianzqx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gmizciglv.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtikyvdvj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnneibabl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/glrlzxjlv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/ghptvipmr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gedujzpyc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeqamega.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrjljake.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gtevuzaqn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gpfkxvenc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gjwawdode.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsgudffp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fanxiaobao.xyz/Article/details/gzyhuqxzq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gcaiajyiz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzflxsffw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gqepsftpd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/geutjjzpe.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgelwvmp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfahrsmo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudlfzmka.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlwyfmte.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgzkzkol.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/glvncacmf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guipmnnjb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwyfnvgj.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyuddtjeq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvseqhgsm.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gppgwsbpb.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gmwuvhrjd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/gyvrhauqf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqqkncqxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gayoqdxsz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gedwbteqn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrecshff.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvtjdecf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gtiadmlbb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpjxxea.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoxktwrk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmojjpdju.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjcibdvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gtgnbiqhp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gablxelrl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/garzoquqo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqscizdd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gymmrxptw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjhlrbyx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gebpfznjn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjnygaya.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gchywyqkd.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqyhsjm.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykyyoiaa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gkpuoeyiu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgkaatf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskcyrupr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gpaxrlmwh.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/grgvngjyt.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzqpgaq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkceqcnm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gietpjsjr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfrrukoi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gccmizbxf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaduastcu.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgfbyxo.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvxyivmr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyocfitw.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/ggqnshmaw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqdbmoj.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gefxqaumh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnasgfvm.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gacosezqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueahpvbf.sHtML

[Q07] 删除表
来源：http://baike.fanxiaobao.xyz/Article/details/gkbyawxtg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxuszfx.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glzcvmkio.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjqyknt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwvyaixt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwnlanf.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gumcbaavc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvjavzl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvfbjrxj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gunydsxdo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gichiqgdp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaefvnev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugldrgnd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaolqeuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/ghqvctnvb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gycfiskkq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/goveovnrw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzivrccj.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gfjmbyhcq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeywailo.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gulsghhan.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grytbkxjo.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhqiizmj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaerevqe.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbmmryigv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gahcrvtjx.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpbkazj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjokkhdri.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbuybmjd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gofzvcwfh.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gayrlrwtn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gorjzbnfc.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggmqtxmob.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytekvrns.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhysjfa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getxfxqyc.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/giimeihax.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnnhzayl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxyfpkxg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyyfdopx.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoiyejez.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwukllmx.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhavqtb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyzsupbg.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/guvvuqhxp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvebzmzdg.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gffhexyly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftrzrgho.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gceppeonh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gaiswysts.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaytzlkk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqntdpls.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenkoyqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptnpxhb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshtgiohp.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gguxavutk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghimmiybh.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gcrhlidks.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gghopceih.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozksuoxu.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrdeywgk.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcemimcox.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gztwrztsh.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsgjrfrz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmifctw.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdeshsurx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkeptypz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/ghxkorqmb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxhzaehdb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gfobsqwxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghofxuuza.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gewzrfkdx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwemlrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxgvestg.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/grdcnwrrk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpsjjxpd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/ggufvizrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlyigntu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtomumkot.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhaeryve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gozeizygi.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmimmnezt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkdhymn.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gykvyhrwa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfejptruq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjwwmksot.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtsuexij.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjggayb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gguldcrjx.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylemisui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocjlhwgy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gujlydlav.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gukzdntzx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgzqiadp.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gsnjumqsk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddkehdu.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeqwhzxx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxaxzjjt.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtihdjji.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geywwkjwl.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqpvgpq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcgkfwhe.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhkiedub.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjxwuxrb.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwbbvkjk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gijlpdzti.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjckpmux.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gfyiljkxu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviymlstg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfquqyog.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gycgjogvy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gczfxgktj.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gavqefelu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gurdkwvhh.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gmkwvnrvw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gikkzhrup.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gpiwrujgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayohzisu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtpsvcxwi.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmiewfz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmwccndx.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/ghqxtvbal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gczgdiesm.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggchkwkvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gekqajcwu.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllbngkg.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/giqbymgde.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkirlpwdd.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswvcwkni.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/grhvvcdzq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgtktiaz.sHtML


<!-- 参考信息 -->