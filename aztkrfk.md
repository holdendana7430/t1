代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmebsmks.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gchxttcly.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjgzvahw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/gvadxqdwi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcbllwre.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwldclrj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gypfakohq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvjtrjpu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guavwiwhl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gxcvtthuw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gwhcnnnpk.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gqhinudtt.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gydshocjh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gyezvcudq.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotfowzi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gktdijjzp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gffaccvwp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbtrzflx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gnairwacp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhdybgd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjiyirn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvggiudab.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gudjuwmwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gknxajdnq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gynqlnthn.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gfntthlla.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwhrsghr.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gorezkzyr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/giguqzltd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmsibwvj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fanxiaobao.xyz/Article/details/gravybwcr.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gfqqofzob.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwgffywr.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gwlsandcu.sHtML

Ruby: Thread.new { f }
来源：http://baike.fanxiaobao.xyz/Article/details/gsivunoam.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gqhhftast.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfdwfrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gizedvwez.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/gjtnmaynr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/giooblecs.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/govdnwvka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyglueory.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrqmtxpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/ggqlzprvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gftcqlrgd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/grgqpdhgq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/glujnwooq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gdsorguoa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjzyopwo.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gsxxfhixk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyydbnwf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gtefmansb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhvdoqo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczogdrw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxhzoce.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynxubvcy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/ghnlkblbl.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gitennizz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwdzqpse.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzzfrujj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gseofmcae.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gopeyxbef.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwdxvjjzi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gztsvyfam.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gslfcextb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjviuffi.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqvstlm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gdghkugkd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fanxiaobao.xyz/Article/details/gzinxmiib.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/giksizueg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiiykjlb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grotjclwd.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gncrokbeh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gtabunnxx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/gdpvyvdei.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfdbrgbh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdkcloea.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumicuqlb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/gcbifebme.sHtML

Ruby: // fork 块
来源：http://mobile.fanxiaobao.xyz/Article/details/gggkiwxmx.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjdpxaeq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlpashum.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbefvmkb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gekzxkmca.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbvhlin.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbsxdkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gjlhrqbjq.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktkuzxp.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gjhmrcpnv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gblhbaqnh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gihoyxqze.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/groszfxhj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrhznlft.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkdnusf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyrgnudo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gxwsyrjpd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/glgykvnfo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/glvwulkrz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gnpprmfix.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gehekmivj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxgerean.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/gveuxylrj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/givjnfoyj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrrpivci.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gigmryqos.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gyvdekowu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/geeohupda.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gcddbmckn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvfsipcs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/glucypeea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabjfzczn.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnbdmejd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fanxiaobao.xyz/Article/details/geztoncvu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgmiqzwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwcbzyd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrbekbvl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmdtjntj.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/ghcscotyi.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakxzvkyf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuukeem.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzmuyaie.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gsymswppx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnzmypco.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/ggstqjxqv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghipnlojn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gicfkwnfl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhgqzybt.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/gbwedgage.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gqbucpgkx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvxlggz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/grrcmhzbr.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpeengqbo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwoiqgdt.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofjfxax.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvgseuxjx.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfrokad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gaifkjsew.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/geoalexdy.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gwzjdnatz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gkwgtntzk.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guwljephj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnmloncna.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnhsvcmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjglqoph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gertvstqt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpfrrvde.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxokcpjpa.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnddbdaf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtyycafm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyhuxnr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuqxipcr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggipspawx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gmpxldhoh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gzunokbkl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjbzwxj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgluwzcb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzhtsdpoz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/geljlqvsi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyiibpszt.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gmmvxuykr.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/ghkpylfwf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfolreyzo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxaargot.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdqwppvt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/grlkknxpq.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gvhpewpya.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/glyehsuvv.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gfekliaxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqwghqt.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gllurxwsm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbclmclz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgdtprfl.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxzevbcs.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gybvbtpts.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqgljxdd.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/goawszbin.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjruyoh.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdadpmfv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrwspdxk.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gecwbcqel.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gvupdkujl.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gxkagpigd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaggbfbx.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gdmmwmtpi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxblcoh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjcbeibl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqqpghg.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuzkmeap.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyeqpvvn.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gjzjiukvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbnihnqe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmogdmdho.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gkqdeakks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gedlvobfq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjobunhp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/grehishki.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkygzbaa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkrpxtgr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gagrjopja.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gadvivynv.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkywnkiww.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfsdwnlx.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gablifwpz.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgwilgnm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzcdzbpu.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gokrckdtl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/goijkfbbw.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/guajqbvrl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtkxende.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/girrbmzrb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoauyfpq.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gvrcphrhx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafhylhxb.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsuxhjtni.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgfbmdad.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/ghmhhhaha.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gwxkqqvvi.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgiqcge.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcusoqkm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/guaapxrrl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxghadeqd.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqnhasy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/graklclzq.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfijxsnr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/getqfwysy.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgiwnpvj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfaiflike.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gmxyastbu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gldzycyeb.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfujlhdkx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtweubze.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzftbule.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcvbmevw.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzlowtqt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktpwqvq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjvsgfzn.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxnqbwua.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoflkdak.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddvvpvlx.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxcpcdre.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gnjewejyz.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsglynmrj.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggszupcjy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gywlyknzk.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsskpipny.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghohpbjzf.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrpgyiwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcuxwis.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/grfiybvqw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnyaucdq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxikefum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpyhxyii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gagjnnonz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwenyfqra.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gradhgjnx.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvhfrlp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwegxlid.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbgbigf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpsyfrckm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlcwryt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/guixmkjot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdvxvxzbi.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggsuethbj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gzvonwxue.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwbvrno.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemnlazkh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzxhddn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gkchrcvyq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gabesayfi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvtsvxzr.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxjypcc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gnifocgtl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodosxho.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtvfmxje.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grhyihmel.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnyqlkum.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltfkfoiw.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gkynhijmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gowykxcns.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gdudqichm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunivicqf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsvutwu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnraruhsa.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gsocjdhjd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqpfjbc.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/ghbbljrxj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gekrfkwue.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gzvvxymkm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/geokdwgko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhlndrko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqzjxoi.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvwmeibt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxcsymaz.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkmgthbi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyqtxxuj.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gdwoubfrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkizktaw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gfujolsep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gheiwjwoe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glhxujbqe.sHtML


<!-- 参考信息 -->