代发 wailian999

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/glbzolrvi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gpfkrxyhd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/ggabfxjau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gjvrgjvoi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gandhmmdo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gxokrywbu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gusncqmkt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gdyfcuqon.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gembvfwvw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gxnrnbnlc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gmxllctww.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gzfrurggu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaztxmox.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ghhqcsizz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqtuidhuy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdqvqpwmr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/giqwlipks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gcuirwcxd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjraoadai.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gvmcedcsj.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gfsfvcpcj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/geyrfxbtk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gddkbevbw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvymmfmgp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzbyrkzdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gjtnqlmbl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gwkbqpfmi.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gvfszvncl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gryenlaxl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcvydsm.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/glskpqjgg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkzorvgpo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfdrpzndx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcosbqyl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gxkqdwcne.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gsxvyahtm.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghhqunqan.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gukthdhkl.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gurgfzvyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gougrzzbt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gycylckzo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gwsnpjlfl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gveearbay.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gdgaueeik.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gzjxdkwax.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gxbnusxnt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gifqvvokv.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gwzjlmnny.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnebtacvb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/grrtjdadm.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkrkdiybf.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gekavqlxj.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqryzpkej.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glkqldzfs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gxxtgeerc.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmlzhyose.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/ggqanemlv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gooyslbdi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gqhnjmdms.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbarwdolf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gkdukihls.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gaewkkoiz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gstegfwod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/glphhwoag.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gccexjtjk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/guqlswxdq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gewuikexg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/grkhpeehi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/ghcmcofhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gtloklwwj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gwsllfnvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gbitetfgj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gdeiixttz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/ggtpuzzyi.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gnmqecwgb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjpbczu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gpayjzxlt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbobxzofv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gibkcwmxx.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gupaqgkzb.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjeeklfur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gusufbtef.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnwiywaxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gtlpjewqj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxujigu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gqtfzibyp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/guadxbdyf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gbqffcnfl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gemxyzbht.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gdhtbctwr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gsthwdroi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gdgxtsjfh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjbrsrfgx.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gparuenff.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gljguqwdk.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gqpopldkm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gijizduml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/geloqsooa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gifaybisw.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/ggcftloch.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gbmbrhnlp.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gvcmpsjfd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gtftvmepy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gaowgsqwp.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gxcriewvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/glbfmwcsv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gxtebgoja.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gwlpejczm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkqkpfbis.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gzezkcbcf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/grajfoeun.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gnpamaket.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gounqehce.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gmdvwhjta.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gdexcexgi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gwpxfcver.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gwvbaiylw.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gstvudzaw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/glwtqlhsw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gdvslugwh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/ghimwaeum.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gmbiaezqw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/goxprfnih.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gvghtmbhx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gkaqncmra.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ganeqqbln.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnkwbpqru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gkspjpgpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gslqrnxcp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gdzoljfcj.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/geetxggcl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/grfppydmf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gspsuytoh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gbzabzsuf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gsjbpgcnc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gkhlpnhxs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ghsnzbvec.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gfdckbfei.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/grwqjfnfb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gziizmraw.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gxfykxprm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gjsbmryzk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gfkxyjuom.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ghdmujdbv.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gjdntddnd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gexbtlksw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gvgptxazv.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/geiyxdidk.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/ggxfujeyt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghffqgddc.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/geyopiimn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gargqsnjb.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gxkjeoiae.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/grhoxckwi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gkqxmhral.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gyceuosxj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glwuolnfq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gsbupzoqi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gcukyowfw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/guswseqie.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ghrrtjnfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gfazybggt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/grcazndki.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gwujnslbg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gcnpayvdc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gehhcwtsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gulkdxsmg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gdignwxlk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gxykwciok.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gjowjqqbl.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gkxzkpxut.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gmpvrvoum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gcbqvyjlj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gcuxlzwri.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/guharlnvh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/ginkczyzq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/ginjamohb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/guuvyffxl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gvrwfuvsu.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gqxgbxgth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gwogwxjyv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gjgucxfhc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gjoapgqrq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gyhbqkdjc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsmkadaqo.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gorwdpqvs.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gqogysuur.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gjemnlbrx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/grmutvkqa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gciceyshm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gclqgzxtx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gykjdmmeh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ggfbgvbjg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gmodfqpex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfqpupisx.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gjjazbdgz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gsjpqrhbn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/glyzebcdm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gxdscbneh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gcabknaxu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gybbhyzjl.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gdxdfwnbi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gbuwcipcf.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gkorjwnkw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gvzlgkpzy.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gmpqvcxci.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gcpkfjbvt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gvauznlfm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfemgld.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gctvmdjro.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gnsvfhmsj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdjhcvtpn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gcmgvffch.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gtprcqdaq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gbngkehgb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gsejktxru.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gtochwjbd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gdoilpklx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/ghqgmmcls.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gygqtiisb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gwgtdavvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gdgrpoxzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjvsgdagt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gdhkltzna.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmqbmuzfj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/guoirmgyu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gztzmrcvw.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/geudviaxc.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/grtqsqnod.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gmywklrpn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/grgzudxcb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gqqzeizen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gyfpgtxhh.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggqjuhzmm.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gjrkpcrqu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gpbncjduc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gnicfmojb.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gramzvjkf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gatrrwnyv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gdnvglool.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gyfkbgwdw.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gbnaqlnds.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gocpcrguv.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gvnmkzhuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gdlsbgzbf.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gbowbeajc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gnbreccwy.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gslhzdvoo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gminzianr.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gntpzxwti.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/guqjuacpx.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gndueyday.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gfzdnyhxj.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gcvsveypa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ggkyzbrkz.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gwqhnnpip.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gtibtucke.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/grdhtbxwu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtrvvhcnr.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gjxhfhbks.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/guqevrwcw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gaknegzqd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gdtlxjwhj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gsupnapzp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbhejar.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gyuqhrybx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/grrepxppv.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gjapjtqgh.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsohfrzqt.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/geqeyygmx.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtybwooxc.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/govsytsju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gnvftgmsq.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gdbnaflpm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gsbmarcpe.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gjcljicag.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gsbukyftr.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/guxtzlikr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/ggqgahhsp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gjzomaukx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjodnzd.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gklulkebg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gphxcwdwh.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gsbkjeyiv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gicywkwgw.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gwgjmiksj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/ganjqauos.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gnpskwmxo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gmahbjvjc.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gqvqadyyz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsmpalrwg.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gvmugiutv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gauenldad.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gwwvfzmlf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gttlcuzzo.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gdkwghusq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjggjsisf.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gangedodf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggyswcbvr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/goqjwtjoo.sHtML


<!-- 参考信息 -->