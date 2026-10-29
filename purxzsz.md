代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gdsgoituo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/glsyupylc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gzvzfojfn.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gvawtyxoa.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxfgpdilp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gejuzcqel.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gehtsolgc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/ggulduxro.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gubxfqejn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqfecrnxn.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gojsflohp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxkwkbzzb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gvugwxvch.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggsgkxoqx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gmuavilir.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gmbfnbhip.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ginetrytm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grugknfim.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdslnlhbq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gtnnvfabv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjsnbwopn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gsoexoajx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gsiuzuykj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gnvdgbavx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/glwxhqoib.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gcytgowmb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gmubtvjmi.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbrccpguz.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghlfliiyq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxtqtfyjx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gzkkdfyig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gimkikege.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gdurawitb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gysnzpooj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gmmkxoskx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gfqpuzewi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gdzkeplre.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gqmljocyv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gfyhybbof.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gepiuqqyh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gugucamkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gsdxmyqgo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfvfrucde.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpundvcnc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdairqgvt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/goxcyfzft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvefmchma.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/giqpvycxv.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gcneosgpk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpwquoisl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gfcolkcyx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gjzaqurls.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gthzvlypw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gumcjhnrx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ghzjxhjzl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gahslufmj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gealpbwve.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/genuvraqk.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyspuhtwk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gnznhhhgq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcbegwhvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glxmqyeum.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gchrphxud.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gayabbkzt.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gojuntyar.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/glkmoktfo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gcdlxrqnj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/grsyamreu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gfdzatoiy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/ghuqilyhc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gshjodyqe.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gpriswjzy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gvnaesfcp.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ggjcxacnp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gozdjkywg.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gpyitrjaq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gbdjivuxz.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/glliaqgkr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grdccpedn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gblklzbzd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggjsimazb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmkicthmf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ggbyijldb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfarnwbfm.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghypmyawp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gpfwhvews.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkrxmdznk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gecbxmumy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gjzukhaia.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdnjwrcba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gjjiddiil.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/goysjqjuo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/glgqxrutn.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/glbnhsoin.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gsnkmtvkm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gqexxmcfv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gqsztvgtt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gzqxwnyax.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gozwoqxfg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gclsucqum.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gicedlurd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gxltyddwd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gbbnafhic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gjiegdqou.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/grgphcumm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gisvxupef.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gttgmkvzj.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gkykswdep.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gckggvdkf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gsuknaqjo.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ghoxzayxk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gzoyxtbcb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gjxameozz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gmlttvmwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/glkfasfqs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gpzvvqneo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjuiplfem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gtetnchfe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/golxaqsbe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpnlfltsd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqamroame.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gnzgkjxqo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkvhyfnp.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggytkswqo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gsaaogrns.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gjzimmyzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gqlottjdv.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggkggvoqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gcgxivpxx.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/goufwqwpc.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gwpqunpbv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/glxfzsxuk.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gkxzklkwk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gndscvwbn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glokagzsf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/guhiarawm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghkglppar.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gkqbrrzmq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gyjnoathg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gacgxffbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gineaodfg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/grhyuhyms.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gmgmgxgdf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ghrcccigp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gmzpddtbn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfysjghry.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gccnyfpit.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gxcdphima.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gaqhsczua.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gievwjwyr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gxrwpkfiq.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/glqbrhbeg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gztqsweat.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwlztmdbx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxyceogqx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gaoussctx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gjqhvgaze.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gtqsfvzfp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gqnyhemez.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gtmdretkf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gmnvxrvel.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gtmclbflq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjzsqghou.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpnpmmtoa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ggbekoqeu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gzehmhjbt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gdmhmcuob.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gfhovlxvd.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gkaoepvrj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ghlcdwnhw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gazsvgili.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gryitektz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gtfwifssx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gnjbbhlgi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gpofjlmtr.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/grvqzosme.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gntznkvdz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwclsylff.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gwqtgmscr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmchqvncn.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gkteajmto.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gohclmvbv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gklejrkjt.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gctleedur.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ghapbeakk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gqdkkrhxv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gwszetdfk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gbbksxpqm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gpaxbhkhq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gpegpzzhn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gwiqsxfhg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gfevepnpi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/grgcbaxuk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gcynogmbd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gigfhvjqr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/georxkjxo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gjtkvorxk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gragjlbwz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbaicrzqf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gujvurshl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gehqgedul.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grrngayou.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/geabykeby.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gbuvnyjyd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gcihyquwg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gdhpqwzxl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ggqzqexwd.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gdssjsmaq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/geytzwueb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqbsbcusq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gshiigbju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gtoxqkwsl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ggdfslqbm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gktcbxgjz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gfavczwsj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/ganynffxa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/glhljznod.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gozphcnlf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/giotvieca.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gwmlvfllj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gtcjhigro.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gzrvggpxr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gacfkoqlf.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gvctnrbrm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gxrddjqun.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gzztdvatv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gcafrggez.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gqxadjdwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gsjciwylp.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/ggisubgfx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gautjhjzt.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/glvatotrp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gevpjdfls.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gsomrmuzj.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gzdrablom.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gofoqfudg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gmbtnmbbn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxbodslks.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gseeeqzlf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gphezeayg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkzsbikhc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/goojarnds.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gjpkhhoxc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gqqhsktrn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gwadxtugf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/giegayxqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/glkdhntyt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gwovgkhex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/grrtdofae.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gzczrnlac.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gvojuqxax.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/ghdjexnnt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gciopfnjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gofkthrqv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjlrwpmwn.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gdojrdbrn.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/ggufzyzkm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtgmnmmpe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqtqovrqw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gzwerflra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gqcacwpof.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gjkfgtrkq.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gpkezmbck.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gamlpaehl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gccizvcxr.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/ghjgygafc.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gzbviuoen.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gxmgfdqrf.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnddgnjqu.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gsfpjmasm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gvmqisdzz.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/guhzdbeok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gegrqpggm.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gxltgzynh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gdolvmokq.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gerkghvfi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gmlppemxm.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gbukayqwb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gntixjmia.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwpnjtqex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwaixlgfz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gmvqimrgs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjfwybans.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gsadhbvmx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gxojftlrc.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gdlqttfbf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gqmiuwpfu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gaigdfvig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gvefgrvos.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gasgnkptp.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gfpxrqowt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggiitaxua.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gpwhgvtpv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gavokvwng.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gzovnsyxt.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gwsyjzuae.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfjloxqei.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/ghxpjwxwm.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpyexvvjv.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gststukel.sHtML


<!-- 参考信息 -->