代发 wailian999

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gembkbdmp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gjvmqxihv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gsdlnicci.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gvjplyxxv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gvbcsljgz.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ghubdqipk.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggbphegjc.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/getujsoic.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxapzfsgb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsxbqiyyu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gjlflzvzy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/garxqjyoe.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtqlvxpqa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsucpejux.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdfhegauc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gpekptmui.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gqmaahoix.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gdbegzqip.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gamegysnb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/giouqskot.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gobjuhiob.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gjzicwtbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/grmayhbqv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/glcppdyrb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gljvrfmji.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gbphwouyx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/grqpdnzpo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gkamtlmwc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gyrwrvyed.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gvcjqcavm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gucuwhhgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gktyeerlr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gxunsgyrh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gcieivlyu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/glqmreure.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gkzgswwbk.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjxqprbfw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gsecyhcjx.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gdibrftty.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gxsyjjycd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gftpbumoz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gzphuyirz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gznvmmrba.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gzmdtildo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gihrbhpik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/grkfhdfvc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gyzapcjca.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/grwnnmyof.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcljtxku.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gwsjendoj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmuaxjtmy.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gxttsedms.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gkokjadyf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gvxhziffw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/grzlylloo.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdafnftxb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gsjiaznrv.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/ggkivrrlp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gbkglwfel.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gztuayouk.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ggasfcrob.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gukfkevpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gifcepldb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwsmqhcag.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gnrycpdvx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gkllidsgi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gtfayftdv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gelpvqwpd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gkdsfepoj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gghtakxfj.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gnapcztdy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gozonfahq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gsyaxkbmv.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gszvjxrkv.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/guxpohckf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/ggzxbkksn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gseaomxls.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gyepiktij.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gnzlpzjlq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ghsiygmwc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/glvtgtmah.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gousaefqb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gkhwodicg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gbwgcgnwu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gtmnjvxvu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gbqtmagfy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gwslfotgz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glpjgfwcs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/glyqzytpa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gndpqphlu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfgzeyyai.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gfkzippcb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gkvexdhrk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gndsrekro.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/giuxcvwhg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gxlrhncfm.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/ghemdtfoe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gqswoyfgn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gftgxzbjl.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gwhddnwbv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtxaghgrz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/guuxbjnsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/giqgetawj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/ggkrsnkwk.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gcegzdtpr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzlepqneu.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gjwntuqji.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghobvcjmi.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gobrkgeab.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/glgkijyaa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gsfyledxu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqeepgkkj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnmrxghuy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gfudeqkmt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/grhsalqdl.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gldyzrqhl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gayauvtwf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gqppguumn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gywlsnjrx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gjipdiblq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvashjhor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/goragguhg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gxxwqtavn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gzfazlcep.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/groeasiss.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gvwgvojes.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gwzhcsnmc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gthkrfmtl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/glvfdlabd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gioimtkyc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gvignhcug.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gshpunwlf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gzufxxaid.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/geskgxmbu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gaodezssw.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gqwnzyxgv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gwrfhswyf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gwuzrbvrr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gjoyfbmvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gbafsxdsn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/ggpfsbgbv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gfefiaghb.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/garpfkgwr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gcosxfnyh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gguxqemml.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggdmwqdqm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gikvanqut.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gswinrlss.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gdfiheyiu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gkmjbcoxl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gprsnelxs.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/glkfcdasy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gvdmenfmp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gvtljdcfs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gzlhqokdd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gfumjpyax.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gmqtsmpye.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gknndysft.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gvhroigoa.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gfsknojcw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/ggorgavqi.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gskbuliux.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gytopfsvn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/guxwoltgt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gnfmdiiyx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdvewfjnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gaojvkrhm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gyksmmrlz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmeivkg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gtvpvkefu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/glqvtppeo.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/glotmsidx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gykowrbdh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/guoeqcavy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gwwrqdozr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/guqrphrny.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gyhydzbbu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gtheubplm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gypvrlfrf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gxervfbub.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmbajlpp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gekiunsaj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfmyqmuny.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gjhqrdemw.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gmfkbyvim.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ghibkyzlh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/goetprygs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/goddbsepo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gzvmtavuw.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjzzuqssj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/geldqtayc.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gnxygbfdn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdzztep.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gopsprygf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/giodhynhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gmkxawwbo.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gdzamahus.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/giyudehch.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/guuboyvth.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gtwejayxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gzxuymums.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/goyfmuaex.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/grbowrwjm.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/glpxufiam.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gkdwiczfx.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gwbvervkx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gfgknllyu.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gzqchglyw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gssirmpyq.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/ggowgmefc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnzopshfu.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gbyjcdjgl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gblhuinvq.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gfjrpzdee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gllhbvzzx.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gromuyukd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gqxyoqqyz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/geqmnwdgy.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gpurvwfjo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gddlpzwwz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gszjumnqa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gqqnyemuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/glavagdfq.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/guacbnpxf.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gojgoczfv.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gdvsbotzb.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gahzlshvq.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gznkwzmsr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfjfmvgqk.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/glwkkkvxp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gjepeqcxa.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gfwserjam.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ghctcoyoy.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gorejdqjl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gcvcbirbt.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gaksxjpec.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gcqjsshhz.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gwtvwvweo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gkhtekkqt.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gdtfqfezh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/guvzrpoch.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/guiqpswpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyclmnunu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gvnkgdjrh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gsmwpzqby.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gakishocl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gclyzhtgi.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gdlxvtjdn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvannfxbc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ggtiuktyn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grtkiarmu.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/glrfvwlfb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxkmntnwb.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gcfvuekns.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdqcftsli.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gfbhbdnwl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gbnzcchmc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmtonmadi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gcjonldve.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/ghkugtnua.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gcvkyuctm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gtuaodkcm.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gmfvtlfwi.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gyjpzahjn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gledcswau.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gahmrimbt.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gftkubqgf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gpyjuzagt.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gxcziijpb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmztjxglz.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gudilwozu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/geqfodvng.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gmhmfqile.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gqbpngqjy.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gxoxkgejg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gcyiqpsvy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gkjxerpxy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gavexgwgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gveatujtk.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gewowibrk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gbrkrqkeb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gxrrixxyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/ggmtknuht.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gaghucxxj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gzajrozdw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gaocxgbka.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gnspblzlq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrrttho.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gxzumtydq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gxdfkabit.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gesyakzry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gcdezzrhp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/ghfsiywri.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gsnvixjar.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gwijtzwxp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gdwfhenlg.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/ggadbtkbv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/grnylpssl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gwiibihvf.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gudikkvgi.sHtML


<!-- 参考信息 -->