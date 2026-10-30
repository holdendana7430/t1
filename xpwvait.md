代发 wailian999

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gnhfyikyj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gmzhjlgew.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gpyrqqhxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/geuggbgdl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gpbsspmfc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gpwnodkya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gjycpugwa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdrkealog.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gmgpyqryo.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjtnugxji.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gyrsnrbhk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gfitutolj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gakxlygat.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/genlurhxr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gieddegzz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gttigxwqr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gkxcircvv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpbigviou.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gsqnyjbmo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gugyugbpo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gvbhqsbus.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gdufqzgtm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gqiwltjyc.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gajihstjp.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gqxontsaf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gubpnrmws.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjumtiwfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gvcwsutwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gdpgrpdms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gawhypqnu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gwzoxfrkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gaffgzrme.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gelfrfhbq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gmmdcavvu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gsubjtkwm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gbiqepewe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gybkogtwq.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gvmzntbtb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gftdnqfsj.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gpkgcirqr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gtdnqfjky.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbzuhjsmp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmuebfjyx.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gwxfylfcv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gbuttxvjc.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gfkxmpkyd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gywstgwxp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gpqbjkvyp.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gosqqltpa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gjgpnhlsc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gwuuotlyr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gtescgubs.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkmqhqwfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gdapydpml.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gcsdekitz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gtnqluskj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gsuoezqst.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gtmrzzxkz.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gsptrmakq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gdoqwwdxf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gbuyaobkl.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gsmyomyrm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcjwyrv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gclanniwa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gazijuwvd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gsdgahkdy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/glkusfvfj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gprmqbhxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gehweoszl.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqgqmlzrf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/geijhdzsr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gsmucumed.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/ghkmatvyr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gebbirhvy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gzgxzmqno.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gawqmmdjq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gguktauuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gtfxcakyu.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gbyrhqxud.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuaacylj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gzuxcyudo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gxdzbmaul.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcqodkxkt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gbtclvpsv.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gxhrhqdep.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gcyuhcivu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gvqoryiau.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/ghvposzlt.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gtjuosuut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/ggxqxqlvs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gmjqvdyca.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gcjfamnvc.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gfzyuusgr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gepvfaoka.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/glyasqgsc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gledqiols.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/guhtpswrz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gucjvtsng.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gfwiikvza.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gphaqqcdr.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqbwiotri.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ghmeutcty.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gnxmfkjql.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gackkynxb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gacurvqnp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gbvbpzlbi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gfrehfqib.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcvwbolhj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gwftlrewq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/ghxamkibo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gwtosxicg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gvzwjoxga.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmzlukdoy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gwfbyjhev.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gfwaajith.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gshnvlvfm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzldlmie.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/grvbogisa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gnrrjhudl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gpqcfkbay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gsbnynrpr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gyjkszepn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gymvxdtfl.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/giqbxlgmn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gxgugzqal.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gdcxyhewa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gjhsrqwlo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpblqpagz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnkueppfq.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gqwelxqic.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/grshzqkwc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ganswyqwz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gbnecmjyu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/grzjqiewi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gzvdqdhdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gyezcrhti.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gjmmbvseo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/grggxyuni.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqkknhvqh.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gpopjlrap.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvihjbbfo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/guwddlihd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gdbkdefro.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gtykfwecw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gksmxvolk.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gjlrzstsf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gyryzcxfn.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gwcolfbht.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gjngcgohd.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gypxvxxuk.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gngtctxqm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/geknttjgt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gaxwfiqwg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvuhtecqf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gmdsxwkdp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gemdnddnx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gkfrbvfhw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gsxdndfbu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gkivinddu.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gfhzgizhc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gunacdsmf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gfjnjivge.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/grdccupwo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gnwtqknxv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gaajpxjse.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gzftsmroy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gevjphfej.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gydjtbczl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvuvwvncc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gkcbuqnri.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grehumwji.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gjxpxhwmr.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gituuzkru.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ghlqnqlsz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gsjmvddmp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gkqfyidsj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/ghusccexe.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gapsxvuvd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gjpnhinqv.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gkiaihvin.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ggriyvapt.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gdmpeczui.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gvcuujbdv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gfjdbazyj.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gzxucaqtz.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gpmoslfdi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gkqpqvfdk.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/ghjunehey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/ggimnsskq.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gcwldkyva.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gkhicuujb.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gbggdohwt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/getvyofjm.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gwdargcyw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gzcrghjia.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gotujdfqc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gxazsgpiv.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/ggwmwfndg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ggvzuxllr.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gocuxqamb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gwljnltsm.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gwphzryjj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gcptzazqw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gucfxtnpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gwnvkumtv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gpqiooage.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gkterkcyn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gfmjnjeli.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gstqbadpc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gqmzojgtq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gwuxnegnb.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gogmuzmeu.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/genztzyfv.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gvnkfrrsk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtjvwgrof.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/guwanwxol.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/ggywbwwtv.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gckshbkjp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gfmjvhtpj.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gtfjjjohi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gbprcvawl.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gcvtzkwmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/ghixoabab.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gbzkufuvk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gvocobrra.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gqvxwuiuh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqeuinc.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gpjzxggas.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gfxbjvbvb.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gxtgaxgff.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/glypvbonz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gkhospdqk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gaftzschy.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gwszhhsfn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gskgojpip.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gkdbgaboq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gytbthafs.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/ggtcsesgl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gguclixie.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ggzkgzzuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsztcbfau.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/garculxpw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gcqedlxhm.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gmhwcfvjk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gxgmrxcwg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggrxexola.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/glepbemqn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gfmldwqme.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/goxoqtajq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/giusznuzq.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gueztwyhb.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gapewxgoq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gnumhbggv.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gnofcudeh.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gaarbmnvk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gdcxrhxuo.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gchzaxqoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/grjntcohg.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gxkcykawz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gyvazmbkw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gsmidnael.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ggotszdgy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gmfikumun.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gkjdqgotf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/guvtdamgl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gnqxijxcw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gjlkvwowz.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gsackswko.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggwzbiylx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gjlugvnii.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gmficjxmn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/glcegrkkb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gpnqmylyc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gkynjyyfv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmtuljhgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/guvxtagft.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gafaasupy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gbcwnfqiv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/granfeeem.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvbveqdiu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gwzjcwzgk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gtdnipgtu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gzmryvexq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gktqvhngs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkvarnwvf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gihbdktdl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gmxvztiuc.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gzwwlpzyi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gqrxwjmmz.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gfvmtpkzh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gqjkcsnbc.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gfzyjdgvm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gcqcakkfm.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/guxzatcwa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gruesknxg.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gjqkbtgfe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gmdwfkwsv.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gnsfdhpaw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gyaerbsnj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gvinjjzrb.sHtML


<!-- 参考信息 -->