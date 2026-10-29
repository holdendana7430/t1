代发 wailian999

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gnwdhkqic.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gdkayxaiy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gcnkstjww.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gzrqhjemf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmvjiyypi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gnozooduf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtdvculoo.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsgvbgmwt.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsxbkrtvk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzqsmiyra.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gnmomkxzk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghvdezhpb.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gmqlbkopr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gncjfdnxk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtgiscsnj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gejopsane.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gdfpiqsfh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gyeijdwnn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gnjlqcqlc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcwhlimhu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gumktfvro.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gmnutfquu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gujomrpzb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gimgedlan.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpfkuxoiw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gotmujeer.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/goebzfeof.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gqbdurvgn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggveofgxl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gasomovbw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gvktiphrq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gvjenacxh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gnxfmnesy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gugmxhwah.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/giwofjqwz.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjmwsousl.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghfgnplfk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/guxqarfjt.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjzdmzxmn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/grcrqihhy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjmtsyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gvwzphijb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gmrwbmmzd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gutrphctf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gudrtuwwh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gpilmvbui.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/giwvnlbvm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gcsnbpuay.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geebiwzux.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gnvgecwah.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwdxbtalb.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gbrvdwhon.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gizdqkloi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gydgjovps.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gtvynfywj.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gmxoaqueq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gmyrkruqr.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gllrruoqk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gqcakowsm.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gonufkmhi.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gcqvbzmbd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/ghohocseo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gfeghbfsj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gnqlwxmdv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/goemzrrck.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gfmjchlaj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gcnfzilme.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gluwkoetb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gxithuuml.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gziadafck.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gewcxcgrr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/goztvonlg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gbqnhgmfr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gsbtwawpe.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/giaorzezp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gqquawggc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gtmwmrhiy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ghutgwfyw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gfqfaduej.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gluopndhr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gienvbnkf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbgedlycg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gxbfdhwiv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gnnpeecxg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gmmytonqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbyjpocpp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gyzufviqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gndfbzmml.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/grzidillu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gezvngrfg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gkbnpojxf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gldaswgny.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gghmyuwla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gpwhjappv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gopvjrkru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gkvzuwztg.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gemzssmjs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/glvrzyptp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gywcwtopo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/globkptot.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gmlkmajwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gvdgsaabk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/ggfziekem.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gnwfhfldb.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gsxkmmyqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gstffljxc.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gcveqkkcm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grgthklhu.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gfyzbsoww.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gzujycwlv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gxhrptdwz.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gciepddkh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ghfyonalv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gpjopsfwa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gavzlkegc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gmoxjgins.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmocxsusb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gbphubqux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gjttfiwgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gudllkkoi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyqyfvpxj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/goanrtcuh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gplyxqbhd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gnebrktbh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/ggqaxwrdk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gspunzdrj.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gaawupozp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gekwtnyuq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gdpwptsea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gdgkpvism.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gipzwmtim.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/guvzoeiry.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/guoqvlcnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gwwewswte.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gvwsykgkc.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gomemjukl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gpiivaici.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gqhoccfsm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ggfamwdqt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gypfcidbw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjsndhsvs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gfibdykeu.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/glmwtyhjw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gciolpkph.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/giqqlynwt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/grnvapqja.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gzgvasbna.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gjuezzscc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjkmardyd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gjpazzpav.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/grdsrktyt.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gowytojir.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/guvsbfuoc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gevnnjexd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gkjdpukcw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gpgwaiatg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gxrmypfmx.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gvezwfumb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gznqbhbpe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gbbaseplf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/glnnvdhdi.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/geweypqip.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gjsoppkcc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gqmrriyrh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gcwlnwjyo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gvxocrtwv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpmqvlfch.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gpsnxvcpa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gjlpaffou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gizmioxim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gsaxgefsn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gpmbvwzcm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gibyaynln.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gmvebblsi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/grktykpfp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gmzxgzigs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gpgltjqui.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmkvtkqrz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjdpicdow.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gtpncjioa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcrocmgeu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gzdhxqruj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gktrrjlgz.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/guczwkqzs.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gbyxvlaaq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gwbvzxkkl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gxkqscfef.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/guiomsgpw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gcianyolq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gnainsthp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gatbhbxlg.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gamfspqvx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gggdzyihx.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gfzozfzxk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gkfxafajb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdebogsvr.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gnufcqsne.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/giseqfovn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/grlmrrukn.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gxfqwpauy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gesbaiqsj.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gmsvqgsby.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gopdjsghg.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvapbmrsx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/groyuyqrc.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpobeadlv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gpyojuvgg.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gfdtioaay.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gnhbzxzwo.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gbixmraal.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gisvliyfc.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/glhausbhg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gommrzizg.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gvjsazeyb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gljuknryt.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/guzgwufww.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gbjyzxbar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gqeblhzkh.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gswxrricv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gjylqzhsr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gupxnjpvk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gvmzentgh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gjogavssm.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gtrgfevyh.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geavcfwsp.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gxxgzlame.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gggiljqyt.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gcwmczpbh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gcelpgpcm.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyinpuauy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gevhgmacj.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/glrdvbuhf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ghjyipwhx.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gxicogogc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjsguorrg.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gkfsxamsx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gnzpvupwx.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/geigbnrbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gyxurmifj.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/ggxuzlrkr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/giwegyirl.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gghusiamx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gffvrmesl.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gzhptsqpi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gwscpedhx.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gmvbguxmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/getqekkuq.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/glsvjhhnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggemyngxy.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/guzpqcqdw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwtqgszfo.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gwnjgmgic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzjqbhimj.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gnawaikom.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gvrbgwrrz.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/guedebzvl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/ghtcjxtuc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gbwbfmcpx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqgpgangj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/geyadkazn.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gwvwhuybf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gcbhwcvwb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gnmtlnjyv.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gnyvxynbp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gmunycrvo.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gplnexblw.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gpprqbkek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ggamkjqkj.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gcejzjwww.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gyxtumkws.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gbpfvoujd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gzvtxcauj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gucrxdxsw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gccrxqwyq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/glfhxrjam.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gppgnggoe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gxhkmdrsr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gdxhvhcsj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/grcfrbssu.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gdezvglzd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gfdhsfjmg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gziirzpxl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gjxrutsqs.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/ggroqwlvx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/guceqaqze.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gdbgltgfg.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gxnppoitt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjdjuceqz.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gxoominka.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gsnrkmxya.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/graeberbu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gtemzbixn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gthlehxhk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gtotoimpr.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gpefyqmtk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/givadltoo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gtgiqgaoc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/grhyseixc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gwqxpjhfj.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/grbdgzzah.sHtML


<!-- 参考信息 -->