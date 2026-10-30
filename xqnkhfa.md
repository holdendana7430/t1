代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gucfyabig.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gigcycrse.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gzunjkhds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gsixmrnjx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gtzvcltva.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gssnboyfn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gpkgsqvfx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gdiuwjycp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gojgxxnbc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvdulnmvn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grpippgdw.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpkzwuhns.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ggjcjtldn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gfeknipwk.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/golhqamfz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ginhigeox.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gwvuwrapt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/grvygeqol.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzhnkvsqk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ghhaccphu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gpakbzdmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gzjgfbtsi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfvddecfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gnjmcggml.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvmgqdqun.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/giuoakxnx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjqhimio.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ghjdfkbtj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gddfigexp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gewivcwub.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gnbqxuure.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/glrczrovn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gdwgmitjx.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/grmosfpiq.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/ghcbkbvua.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gecfckypv.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gtusifsto.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gacqqsowh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gmaitwktg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gkcmgdash.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gkwxyltjg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gkxhgyezi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gmtjfrhmf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gsjyhzlxx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gwzwjvcuo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gbrviegxk.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gmwmqwjxr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gwwsytyoc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/ggtzdnnrx.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/glbuigibx.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gcdhrdlrz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/ggdljykyr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gwortfbkv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gyucnzybv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwnsmreup.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gncmvqbwv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gnphkqypj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzfbrhpsf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gsdctluai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/glinkobtz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/grjolucka.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gzjmupseq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpzubzoqh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/guatrkavu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gcefobreq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvbcwhg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbrwfmbeq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gcqfrmsfl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gnlmmwmmf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gvftkrfqk.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grxvjyjsv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/giqynpnet.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/ggmfwcsel.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gkfvxcsrv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/grvupozmp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/geigeivzh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/guatdxwzj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/glsqdojmo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gcoezgqrd.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gcnrxhoxy.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gnqsuzfvv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbyozzkls.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ghltwtfaw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gscxweqto.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gtpuawrlv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gzqwazmnw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gehzarvzg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbqhorlmw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gconzkuvd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtohdscex.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gugreproy.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gxhlnezzi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gjdicmoqf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gnwvkoypo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/guobshejj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcqykdhhf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gjowknqkw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gdnukxknn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/goyzynree.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gfxqpqdsv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gefhydnpc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gssneypry.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gnzuecoaq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gjjxywbvz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gorjsaxpk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqpfkwjdc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gcuneeaug.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gvssjnlvu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gqedvqetz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/ghfdcmxoh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gndiczccd.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gispxybss.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gmupolqdm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfoidlwxj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gnwggqihm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/geeqdhhae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkposrrzr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gpzbzyrui.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gmkckkfpm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gfhlpjqfx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gbafzdveg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gglajrnqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gkkybiqbn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/grbtyfkiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdmsyvako.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/grbveqjll.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvyjzkrvs.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gttsrglex.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gcgmehoki.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gsvfvnnmy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/ggqzbbmtj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gabmdeqgk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/ghgwepfyr.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gydnoqmfn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfjgaxivr.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gczzyjtbt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gunfkzqwp.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gfrenamys.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gqietpylf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/ghiefsnzw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gpxxfzncx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gkmgkrrfj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gdbpgzxxi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gbimgdeyv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gwfxgcaiy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gldhdbswm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/guwermsgf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/glecrmeuu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gkxbksgvb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gtqgfcfpd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gnzhdyljh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gpjzjluir.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gmujquxot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gswcvssop.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gbcmhklzs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gypsdnqib.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvtspyql.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gmhyvnpnv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geofxlajy.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gvkexbnar.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ghffiswox.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gckcyditv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gxqrilktt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gszyszvrc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/grweyauvr.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbzmgdilj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gremkwecx.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gxpstnagb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gdzrcinfb.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/ggpszrnlb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gnfsmnaef.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/ghtytigah.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnimqjeav.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gdlzqrgzq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ghwxaptth.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gthjfacun.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gjcqluuqj.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gtasooexk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gkhpwsdvl.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/giacgmeok.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gleockmpe.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gncoatlli.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gzuaohzvx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gygwwtvur.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/glivejfgg.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gsugfbwud.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gwysiwitl.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gtzebetjh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggacywqdg.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gglcffaow.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gpkqixzxw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gloljchvz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gvtnzvhdt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gpvkdcbyw.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gbremehwp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gpuwmblcm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ghlogxsar.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/ggdohkopy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gxbhvzxqa.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gujpdbmyv.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyikhcuao.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gbvxnncyr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtonkwgir.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gblmvkcwj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyqpkcgoc.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gmyqrxely.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gwknauczg.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gcbihvfmc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gowtivukn.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gfwpeaatd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggffjrvhx.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/geixmwsqn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gywatdler.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gwlzjiypu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gjahxpjmj.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gpwrmgkzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gpdqfdahf.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/geqlmewqu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggpnibxbz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gmsjlkxwy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gvhzlwinb.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gisvakicg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gipkbutod.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/ggcwdgegy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gdznxgysk.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gnfjhzpth.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdsrftcsn.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gaavkwaju.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gytsjzqpz.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ggirprjhl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gpbticccn.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/glbqblrxq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gbeluzsvj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gldatnkqf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gxinqalca.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gvksoaauy.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/geqofwsxn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gtontaueq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/giumztofs.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gwezjpira.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ggegroirb.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gmyolfldq.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gaxvstbon.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gunfhbyfz.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gvewkbraw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/genfrazyn.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gdozqaxoh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmteboalc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gklidubxp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gbdmpwfve.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gzhhaiwff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gdsyffidp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gfpsyimop.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gxrlyshqb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gxpqpxmwy.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gctnvcjhg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gqrmthvmn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gaipnbdoy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gtyxdfqll.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gumghlbyf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gibgfhbuv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gedqwejxv.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gzoopdknh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/geiorrnvy.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gffowhwmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/givmyzxov.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ghgoleoar.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/grzpwxprh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/guekccpwa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gaakywlmx.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gmgrgxzxa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gxrbdzliu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gmbvhzmnv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gieunvnot.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gkegioysk.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gnhrtcczr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gjteetwdm.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gaobhzqoj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqfxaxscz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/grhcltbtn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gszzeucyh.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gkikhsrew.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gnigpwpgh.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gfsqzgeba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gmzpkwdhf.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gqbzcmyum.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gkgytgeit.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gunciindn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gddecbsfi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gvtiwvqqf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gdnmlqyfp.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gdorlunqn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/getrcijyj.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gtllqskrb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnfkvpycd.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gqzvwimbc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmrfxglke.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gsaxxjmmz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gprucltwa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guapkqwvi.sHtML


<!-- 参考信息 -->