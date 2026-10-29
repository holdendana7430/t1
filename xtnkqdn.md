代发 wailian999

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/guewdswtw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/glcmmgkks.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gdxzsctio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gllunocqf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gznaeuuad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gkvubigpr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/goahrrpyb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/grkkautgx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gsxuvazjf.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gjlmdriqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gzmuafuvp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gfsbastna.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ghufzsrrf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gnavecgop.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/grhwaemfn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gdxkzofgz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/grihdjins.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gmeapsjxp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gkqinxuux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ghwsxqetf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/ggbmsdxzc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gltplocin.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gqzistpeg.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gykvzysek.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpcnwsucj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gfflsrias.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gtixhzfmz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/grlwrpolh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gyitbkbug.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gmmszgnjx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggwzypaag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/goagmpomh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/goguqnxwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gnrtyilqo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gidwukfpy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gktaehqqg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxrrrecwr.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gslzyeadx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpahhcnbn.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gnxflatms.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqbrbfhyf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/grtwjhbpy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gsbxdfxhv.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gqlfikmzo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gbdcdqhsk.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gqbirammr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gtnsfhvlc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gsbcsurso.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gkvbubosi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gpdjaztqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gjwfddfqv.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gorjbnowk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/ghxrowfqz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gvhejstmh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gckmzbodt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gedhbfuph.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gbgtfraoa.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gjzrkxdmn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gkmsvnqlf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gsirktbrt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gtmxehpjk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gugmqhyhu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gbltvgyje.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmvlptbou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gmlzoidzv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/grrkfqizk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ggcymbwlb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/glreeaotj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gzqktvswn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmgprbxoz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gxeewfavd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gkrpifxbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/geqgzcfdg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gmhhqhrac.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwjbfsqih.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gfrrxxmex.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/golnmrqfo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gclirpxpf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gnrptuurz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnvvoqeaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gmyybahsw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gxpzcuvyj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmhbksph.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gwhovklhg.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gdagoamry.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gxdfiwvir.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/garfplujy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gyanvbuql.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmhtsllaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ggzdxksfc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gxwvmktpo.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gvduncgwn.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gbqnbbmki.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbjbfrjn.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gvnlbpgwq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gppeosgke.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gxjgmiuzf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gxkfdmkmc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gowdecwxw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcjptddfe.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gcfkkijas.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/goupskyde.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gyhsirnwk.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/glhaknies.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gaojzlnqj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/guxlejjwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gdxdwzzay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcpteqske.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gcstycmms.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gvwnjccwp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gntddmlsx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gznfkymtj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gyvyprxim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gzppzmxfo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gnksvumkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gmpwiousq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/girxmqosm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/guxrwtrvn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/guyuqtxog.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gzlbtgaol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gsgoyoukz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gaoldpozk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gghfcltcz.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/grwwaapfq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gmbglnptm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gujpmnndw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gnppdsqci.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gzvcenuwe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gmxxszsry.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gchjvcbae.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gnqubsqiz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/geozfjugl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gtlyyjwde.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/ggaljmuuk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gvmmvslxw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gvsshclek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gyoijynar.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gbyjezzel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxoqqiibm.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gvjonybgq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gwundusie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gzztlcxfa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/goqvyehnt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gdczvnhgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gdcoutlyz.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gztxztsqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gmewnvqjo.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gpoeuncbr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gghcbwalr.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gxeamnpsw.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gwrgxbxfm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gyddmkmor.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gykbhurge.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gmozerpev.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghbhqovtz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/giihmrbqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gixdnvfpe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gkkjqdxdx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvakbiyrk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gkzfuqsny.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gxjuyvxnp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/ghlbuhezv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gtviseksu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gabqajvxs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/goagqljko.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gzkpxqvph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/ghrczxxxq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gtiqrtncw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggzxwzwza.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gmocnmjec.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxzjksoij.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gjeiiyunl.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gylnpokcv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/getrkorbv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gqbmcmkdh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gyflkreyo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gqvkehvor.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gylnwfdlr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gvddhckjl.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/geemqlrxf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gdgcsncks.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gkmhuweai.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gqwenoegy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gsmhqjufk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gwoecqhhc.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gvydtrfnh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gksgqklbj.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gujgmnawj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/giohfqcgy.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gyjvghkmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwjofio.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gkljitntx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gmhlrrowf.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gaxnvhsxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gvpssgphq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gctyawxrt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gicupjlrs.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gpttagrwl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gldrpgchp.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gawxttwdj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghgvbosld.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gzdorahen.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gchaevgwm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gjkaaiday.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gilrvkgxv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gjjxebjkk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gjibtnujp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gptvshmrb.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gyeydqygp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/guvraoums.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/giowwoqst.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gyxvnzcto.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gemueyskt.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/goooblyij.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gpnhyyanq.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gwhvmyyou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpqlsxgsf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gfdfsixby.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gvkdzvbtg.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gicahiklm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gvmxbxqlv.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gpkkgjvsd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gaevzdxen.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gbgqzqxkg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gafkipqlg.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gzornsnqk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gmjafouma.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gjguekajf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gvlmwaacg.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gaocdscqa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsoampvvj.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/geaifxtpw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gtwnixdmq.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gqvmvkoka.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwwoccyui.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gsnskpzum.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/glvvipamw.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/grosjrlib.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grcwxsecu.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gymmcrfbm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjlttbafm.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/glykvjlwd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gzfvjuaqc.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gkeqhblke.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gfwzwktwi.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gvezbxfjl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/geijhvrtn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gosvghnhp.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gyfxohgfs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gyyiwlnvb.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gwnnqrpab.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gmlftizvr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gauspddkh.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gaqzshrjw.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gmphfrelu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gonznxygd.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gteiigahr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gzwdukduw.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/glwuwvqmb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gmimgsyuf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gldajjhtw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gioxjdnxu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gggtekvuf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gfwutyhtu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gmfebidvw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gnelgsbsz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gllnngjum.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gnpknndyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/glozexhtp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gnmcjxnyu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gvbvdqghh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/grlbtkrsl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gpfhfejuv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/giltbwmbc.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gucetcoop.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gindvquxz.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gjfgzujmt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gouvfvzrm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gcqwayrbw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gjyuetwrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gewjjhenu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gdjnhelbp.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gphppicjs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gbwrptmfe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/grllvquts.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gneizrczc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gughafhdt.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gsygffeyc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grtsvzfvo.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gjcfbngvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gayyjgciz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gmxscckpl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gheuirpqp.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gtfxnyile.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gprebjojh.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gdyjlgraw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gbvfhixqz.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gbvpzinxm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/glixtybwr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gesnjkavg.sHtML


<!-- 参考信息 -->