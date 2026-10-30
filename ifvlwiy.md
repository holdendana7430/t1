代发 wailian999

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcissjzsk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gcfwccqxm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvcbdnbzw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gknhyclrh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gfbricnrg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gjfrrjfko.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gfhbscxgh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gdtmpndps.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gqfmvhqis.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gaioqebje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/geayzticl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gyisrjyqb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gbylyniwn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gzdhsslhp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gzmaambog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gjnvnawpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/ggblacnxe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gtxbelnog.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gnoslroam.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gxleypkek.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/guglhkvvc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/guwtntkqe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjthhtpcd.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gstrhxuzu.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gucvueoqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gcmhfnmlm.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/guteppney.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/glddrhaas.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gtqdsfgwt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gkhlhvrgc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gkdoojrkm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gypcxtukv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gpibuaoww.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvssljfhv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gedzlqdmv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gmfgacryo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdltmlokc.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gezzwdpbh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfyamjeor.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gtsbddmmp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/glrwmices.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gprosxfye.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gywvaouro.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gxqgtoltp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghqogtcak.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/ggwktlphm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/ggcbhrvov.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gpmfxgsxu.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gsrsjmjoq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ghmnwlcbw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gwpwodhyy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ghegwwnes.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gonxydbbp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gsxjfyzxi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gpkujrmki.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gwfbzybgy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gnwctaojx.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gzojeppfu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gbaymvbaj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gugaotqgx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gsprvudct.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glkvsxccj.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ggsgegbov.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gkafsiwai.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gtiqyxqat.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gbgqxritw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/ggqsphmot.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ggmtlaclx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gvugzjkkd.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gorqfraou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gkzhofkkv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/ghsounsxm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gkkquwhpi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gopbgnvws.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gtxxrwawf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/guuartrne.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gixpuiqsw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gkstufxqp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gxzwhnogx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gboirqgau.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grjizbubg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gypcadvtn.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gokveshqh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/goyunncsj.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gegvymalv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfinyylbw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ggqqlngae.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gsnmfqnvn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gvigqixmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gepirtjgf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gbcqxnetf.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gkcmqnwqt.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gmksifibp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbzxxpton.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gfbkxnvir.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxypugllg.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gewqytwdj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gqedovvsw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gjaqtdqzv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqmdwspix.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/giamcsjxo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/glytrsawx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdldehknl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gzqdxlrla.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gabytgocb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gjixgqmre.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/guoslmqpn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gglabqnhu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gjnvhisez.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/glaldrtbf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzyqrjkfw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gpnbzragp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gvpmodbca.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gaburudyc.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gbgotxxbp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/ghfhrttoi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gktswlkpy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gotxvgnhk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gymggjwsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gyiswrgch.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gshpptqrr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/ggidmbkug.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gbasryfsi.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gdljgsmwk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/giocgywsy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grsbjwutm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gzikvquoz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gpflpmvsg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gohsclchq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gifndwmcg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gevgejlog.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gyywfqiiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gqxdjquhn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/glhaneahm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gshijkfkh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/ggvqohjbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gakparpkb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/ghbjsdcet.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyzzeaxkj.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gwlbxgedf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gplhnhcfp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gwyzeizbx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gvjocynao.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfftfwbxx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gzvwcqdep.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gyhnkumdm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gqsmmugpp.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gjzojzjwk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gwlxdenrv.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/goyhfntlb.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gcrnxvqiv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjqvewq.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gvjhsjicc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gaaicqscu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gvagurdac.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gpdhiugly.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gdmtppwel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gqbvuzcyk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gmcpohjxw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/glxdpdguh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/griqyceww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gvwfqqgyo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gwejbmrlb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gbqjpzmxy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gsbdatrpy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gyotmapzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gfryaasme.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/ghhaptfyy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gliufqrcc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gjplssccw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxbbsonzs.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwvigec.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/guaxkckaf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/goeqhllox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ghfbgunej.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gfyyzynfp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gctpktuvb.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmizakwzh.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gvpwiihwy.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gyfiunqqf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghkzaumxm.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gtbwekyyb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gksvysgfu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gxcoemioj.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gyxrwfbax.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/ghxvwvcwq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gqeumeuwk.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/ghojsttba.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzifuujol.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gqketsvhc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gbecargrw.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gnqrvosue.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gxukgczzr.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gpfscenbd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gnhdsabcn.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gzekjhhcu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbpxsdluv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gvxyfoqxc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gcnkmwcrm.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/grysymfhk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gievrmhkt.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gpagjriwu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvlavcvkg.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gnrquiulp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gjeytgpsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/ggzxmugwi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gqofnencs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfkobbsev.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gcamhirvs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/grayazgpj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gtypwngea.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gxfdsafyl.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghudaddqb.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/guoxqgebt.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guowabptx.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gkezgiflh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/geftdcxzw.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gmneswzup.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gecwjexsd.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gerbsvfyx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gixdlutka.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gqmsiwblw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/glxnfdwpc.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gbmwqimqo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gzrjzlsrv.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ghymobigu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzmoghdrz.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gtlxrvtwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gfgigwefn.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gxrxysksz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsyqbppqt.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gverbmpga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gbwglybns.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gyzxnrsvj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gohauoxbm.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gunjkkfmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glnpugnnm.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gdreznyho.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvafbzhfh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gisxtrwsj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcforozrk.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/grlarevul.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/grxxasklk.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/guicgjbno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/giumwyrhk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/goiqbuteq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvaanvwol.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gaxzwvuer.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gkfkqivcv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gzwsgxlif.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/grrwtqkoq.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gcicapovl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnshgcl.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/grphkhsfs.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/ggdhlmxmp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gmaknvtmt.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/giwmoewke.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzfobnyvr.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gmxzmxjsv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/giuygckys.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/ginktayoq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gdyzzbteh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gluvymznr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gvrhheout.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ghnwtzhqm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gcsmubrlf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkrjhbllu.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gwnvztysq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/guykgzift.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gfxswhgsx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gjhzgzwxk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gvplumfof.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/grxyckmwl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/ggfmngohp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gnwhottns.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/glhaqldjf.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxzfqyhmw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gzvrcybqy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gsstkexiv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqanukqlz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gamyeeozw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/galbtmxwm.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gqmeftaal.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gfwmzmmri.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gaasbbhew.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gaauoovlk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gzuegejie.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gjzfraedi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gjyvxuubm.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gdfyvwyzt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gxixdusyv.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/guehhcgpw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/grolstfmg.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxtwifldq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/guowtbmmc.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/goeetpvtr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gytvifxmr.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gsrbhwfge.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/grarajwmy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gchhpagjs.sHtML


<!-- 参考信息 -->