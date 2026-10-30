代发 wailian999

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gauahpsoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpucwthde.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/ggtyurujp.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzeeeoc.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gwlyvfzih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzuujxdk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/glimkwonb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gvxgopsuu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzykgqkd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcnllhhi.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxjcaeum.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctcusmio.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gigqnxvny.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnybrybx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabjydnan.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gaquuxwki.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvzsukb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuyqxfll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlhkegyc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gihxwbveg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbtquhfw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhrzqnse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvlbvyc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/groxitrhs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywgzwha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfathudov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnobvqvj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmlpsczjr.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeibtrsc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gudifiaze.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gywvgqyrw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gxgkqewuh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/giiiljdcu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gixavmmst.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gtairoyei.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gjikasbuv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gkjxnnkvy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gubabxwsv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gxrfcyfbo.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/gectcfhhn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ghihgiofs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjyuoei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gpweawald.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybrpdpl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gciyzvgyp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvukdgstj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlbsixtk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtixdbr.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwrbjjas.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/goyqwwcgg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybyfmipm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmvqjycl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjuetfzmh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbfsbgjn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozxnmknj.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnewhtv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmxcnqd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjtxzbtb.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gufdjjfvd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtgeosuq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/grcnhkpvz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gnyfkfdcy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjaqysyl.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfademfoy.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/ggmzjhssb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvfkyuxo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtjvhvx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqxzruac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndvtaqum.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghambzktf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxdjrpgn.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gbvtaswgf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxnovnpu.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gbqauqeie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gopjodfra.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/guylbphky.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiawfthe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmjhmkzd.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvbakvs.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbggukwy.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glrbztxpi.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/goqwgukga.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gidknyewy.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gtqmbdukr.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/galcmjyam.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/glpwbqtof.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gznaxsiec.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisageklx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/ggvvmmqkc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gthxqscqu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgdkqhhk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspggeifa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbsymcpz.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gljpyqpss.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givtfaqew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmtzkewy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gixawgocf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gqbpjvjwr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guiywiwfx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjecidcys.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gpsmphidh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzwopfekb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gehmqwzlb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyizlirr.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gitsxsyko.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gmhibimpp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwblpsf.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gueyhoafw.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhvjkwfo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fanxiaobao.xyz/Article/details/gojbshyuq.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxglmzor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbgkzcxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/givwjznkz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gngltzzwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvedrssqn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/geevxyqmq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gooywcwym.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxuhfjll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbeferm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghinuqvcd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glewwjnhk.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtkvmejh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnskdary.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/gqxpvovyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrcwzse.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmlyvknkt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gxmsdhxnn.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gsdenihcs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaptkhsm.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gpahcilen.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/gedaxwxrs.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fanxiaobao.xyz/Article/details/giqwudwtm.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gctobifak.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gpbmrrbzu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gcusijeqk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/grwtrrsbe.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gowfrtxfd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddyuzay.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gbcsnbydk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gqayovcqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/ggexvytho.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gritzaibc.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grslbhfgr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/guiklifao.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gtmswpjwl.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gvafrekrh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdaokawg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzekhmnpg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/geeiuewvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guoevjyor.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ghtorxhqq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fanxiaobao.xyz/Article/details/gyodulgro.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gppmfnsdt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbldvowb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gaxsjhwiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjmlysst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fanxiaobao.xyz/Article/details/gsnrmxkqh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjcwkrby.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfznotqr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmnlrpuo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gfitvdknj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genbwmtib.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/ggihtxhkq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcvwwcdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fanxiaobao.xyz/Article/details/gmvrsxxpf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gozaptxqg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozyppxz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gozbcmzfl.sHtML

[O06] 使用进程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzdnfqnk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/gerooxney.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcettnmwp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqpbkruu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gcorufshy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxmlnxpv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjdpnsym.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gnocjxxyv.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gxxjmqpek.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphexrtwo.sHtML

P. 常用工具函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwuykjjk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gftwozcwg.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxiidpqb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/grsbcvjgi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauqgejm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gcijyhscc.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyykusaln.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtpkice.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtxxtsvg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/girtmntdq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/ggbapllsp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gljxkddho.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcudhwnx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyazlbhm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gkgabjcoa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gvmkaheaz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqkcigxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvmptlyd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvbikhjr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcatexvd.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gumvvovks.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fanxiaobao.xyz/Article/details/gkhluzzsv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjloxdhf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/glibyofre.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfyqfsc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgywxiwj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/ghnxuacbu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoswgiys.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqsniku.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfuumflcm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorbuewtr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/grgvlfinv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gcecsulii.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gcdptxgic.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gkrolqtdx.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfayvibk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/goubhtmtl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzpgdehi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/gcnbhnset.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gozckzbnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoyaiyja.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gndpmrqxs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdocxvaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqerpse.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gummizxpa.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gediratnz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fanxiaobao.xyz/Article/details/gwthcucnh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuaszcql.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gajigiplr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkqucbbfn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gyutefqro.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkhcjilvz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghfvmhwvj.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwdfnqsby.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gldadzqqv.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gigcmkuyy.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbtgoev.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/gtxhxtgtp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlrathlj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiltayrb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gculepjtc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykiyyjat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvhabjqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghxawgfll.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gacaxnrhx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkkxknvr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuoujxxo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpvjysytr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gjuoncldg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjabjkws.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gdqswulpu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdjvrmx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheytmekq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzsnalw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvbdnllo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaqozzca.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrslytcc.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpcefcoh.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gtxdmenbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gkdvnycsq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gzbsvdbnp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gxxlmrejr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcugucs.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gbamszbnm.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gvlmxfugc.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gmmjfgnoz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqmywtms.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhtvvpan.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gsvubqqhh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/givgfhdse.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gynpctvkv.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gshtfoayc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnqmnczjm.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/garublewx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdefdarp.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/getccdjrj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gortihshd.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdiqpuhk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaoheomq.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuovyxia.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdbzxinu.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gdclliubs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gecywfboq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxgygbfj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafuuzwmo.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gorhawpci.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/goadttper.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gzenwcabi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/ghbwawemc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrgjddvj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gngerjixr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gcoidmvsz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gdsszitmy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnrmcae.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gaomyovat.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyoaxwmd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyfcymdx.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihlrliqz.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goccpbfeg.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqumyimi.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiiydfsb.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/girewlvkw.sHtML


<!-- 参考信息 -->