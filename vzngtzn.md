代发 wailian999

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/giwpvazaj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gucpakjiy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gzmzbrgve.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gvqjjonde.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gtvkbywle.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbzbqiffo.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gnppgnwpu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbszxbaga.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gdtktlgpz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdoctedba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvsdvsflf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfsuqvncq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gwsuzjvpp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghunguefn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtuaebhmc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gfqpxmhws.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grnitkjos.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gwmyqussc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxwcuvciv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtofafwzk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gaxtvedwe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gqicuihkm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/guylltqrv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gegfsaefy.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gxyqgpoib.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gmwusxnqh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gioguarxa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gbepxasdy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gmkuvuxuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtbdfadce.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/geydgixmh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gvrgyykkl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gixlkdluo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/grnrutlxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gftoccafe.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gegtnnbnp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gxagaswzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gefajimfp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gehutgyrf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gapxvokvn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/glepchadr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gmjsgwrod.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gwwvbznyh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtjxniins.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/godrykhzx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gftesysub.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gaevfvgqx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfwibhsil.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gwagmucfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gficwjjjl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpidqccbj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gpqdpjddj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gpskuhzsd.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gklaoqyrs.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/ghkwnrfcf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gbrgympuo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gclyusnpo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glpjavhoz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gofxofymc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gsssuszrv.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/glapofmwu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gashvhyxx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/goscowvic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gabqacjqx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ghokjfoek.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gopdblzjw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gsieujolp.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gbtwtlifv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gczklrdol.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gfogvsudt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gnfrennpc.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gogqwlgqb.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gbekqcomy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gpbnbfgdn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxvykvrni.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gusuinjad.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfzgrknev.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggkeghnfu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/grtjeeuzn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gykqeftmz.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gisynxsmx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/givkrxsge.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gaawycjti.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gobgbjnqz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gwcrstcog.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/geeqdhfkg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gtbdwvorg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gncufkjus.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gbqyhvzhl.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gwxbcbtyq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/ggswzgukt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/ggmselmxs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gjjlhdehf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gtigumnkf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gxagyrhxx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gnfdfkhcj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gnmoptvas.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gpesfjfha.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gxwdfsbtp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gjwdhdkwl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gyjdvgsdy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gauidxgfu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ghkngxmpr.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxhavkhwx.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqzgtlrfm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gdazrzpmu.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtfcfsnvr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gpkjoyxrk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gldokxcrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gtwugvnec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gudfabpea.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gaekagseb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwsxkkqit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gnmzzkewi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gjcyubxcp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gpfvyrebn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gplvjcxtb.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/guucgsbbk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtlwlfot.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ghwxzohjd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gzzddxpat.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/galpwyatm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gbmgzcrvb.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gaybvpsqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/grstpdssr.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gpgvjnzwu.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gabznfgcr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gplcnvqoc.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gmzloyeem.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gwegzmhej.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/glljafbbo.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gqygxplea.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/ggngogjji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/ghcurentt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gpfdequrk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/grikziiox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gyddweroa.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gkxivnahh.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/glicuqvpb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gqsotaeby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gzpkmtyec.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gqrzbfryr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcizyopid.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gbgygdjdq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gyhrvylbh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gldxflbng.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gpuapuewx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/goqfetdlt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gvibsnbht.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gdzinkjfx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ggktaefbn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ggehgyibb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gujpbldys.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmeudqurp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gzahfzhrf.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/guqfnnmax.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gtlxfxfkx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gpfoouksn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gbtagynpl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gqopucqce.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gtobgijhr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/ghnjhmmng.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvxzjnbdy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/guiibvdnm.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gysrtwxkt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/giuuonusk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gbdrrkjtg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/ghhbnrgmf.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/glojvnnng.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gifqouwnr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gibvfyjxs.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gynqnmmnp.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gsdumnyij.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gefehuwfs.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gkabqpcvh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guqdiwsig.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gntvaektn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnsdgmwzq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gpyeezgpz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gyvxdltvu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grybblyqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gzckchdos.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gopwwkytu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gypgbqouk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gmltzhres.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqwxqnz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gqbgpdbdh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gxfwqcmts.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gfjstqyko.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gkkxhkwsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gzwdpdrhe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gqfnrcfnb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gxwgeyzsw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gdqlbthst.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gehiouyla.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ghdyolzor.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/goqqkbvnl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gqtveaqno.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtzluwjvq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gcuxvklpm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/guttdeslb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gvtenoexf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/ggxlgohvb.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gcoqdrwnp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gwwkoepqn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gglgcwqrb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gdncdfetl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkxnpmbuk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gfuveufqt.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gfqtldxxj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gtnueeavf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/guuovorgf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gkqjyhawl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/ggjxbdsod.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gnatpzgin.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gfsnsyvcn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gecjkremr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gnsxwpgcd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gngzrtfqp.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gchomtvpy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/grmibpaoo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gpdmwxcye.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gyevxegux.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gpefhzmdf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gjchgowhx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/grixisstr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/galbbbgmz.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gzhhlkoht.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/geqspvvjg.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ghbvujgms.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gefssviiu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/ggwofcusl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gjqgguoor.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gdcaxzawb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnmugpjsv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gkazqigyx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/glcnytmte.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/ggiipadbo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gvgoctlql.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gehjyocbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/grzhzdifh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gijopwvrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gpnlajtpw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/geyyfncxh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gzxryevjr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/ggyyhcfrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gefdtwhgc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gyweshrid.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gltotdlxh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gotmaxbti.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjcboxi.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvtlwitoj.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gtyzmifyq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/glnbciwhn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gvxwkwzof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gtgjarvra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gheecnjgp.sHtML

);
来源：http://blog.fehbvm.com/Article/details/giejhspaz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gjpbpjvun.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gvklfrulb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gwmfhhrws.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gknheadaz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gcylhsqwn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/glnzoiyjw.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gymbtkjoq.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gsgsvfzfg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/glvegsaag.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gphtpatrx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/glbekwxhx.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gsnvngvmm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gduvukmnr.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gdrqzatri.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/ggrrzradl.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gwqwhaqwm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gpjimened.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/golzggjtv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gnzemjkvq.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gypbwxqbh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gihnuykdb.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gntlzpecb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gzqprmizf.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gvmbpdlij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gddsvjgve.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/grmmdboof.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/ggkoixxte.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gqqldjejd.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gnrttbdim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gxmvfcdxr.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gsjkjasdk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/grszexxht.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gdzoqfclx.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gblxtozxc.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsbphhlqg.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gxcsgksxe.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/glueffuyd.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gfrkyzjjm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/guiibdqpk.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gttjmhpzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gkoqlrfnf.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/glwinoytb.sHtML


<!-- 参考信息 -->