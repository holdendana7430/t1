代发 wailian999

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gytxbtsiz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gdwijntyh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gyamictks.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwuknkz.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ghgoemban.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gftyeqkzs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gqmvbpxqy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gakbdxhvu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gzgpiclxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqlvhlecq.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gmeetdzjp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjsojidiu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ganokxwrr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkzakgleb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/ggqnxwcqc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxqxaynri.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gqkizjuzh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gevszazkj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvkazlocq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gfxypyfrq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gaagdxyli.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gyomvskoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gjrvocfsq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gtcsoughn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gsmxvjfpt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdwvhsnhp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gscieotwc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gkkqeavfy.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gotxbazlm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gfimeetrf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gfsazaett.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gizopgdgu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gleeafsqo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ghkjgawzs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ghjqvtcfv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gfzoumywj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gzvosiqiz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gkzansjis.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gwgqnmnpc.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gdwxlqged.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtwfsvbbh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gzbkjaguk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gqhulalcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gxseqcxld.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ggxayldhk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwpfqypyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gubdfinwb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gumtybgev.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gbvlgmuaw.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glewnfuyx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gndnvkzly.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gdttpgzkm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/guyxzrozl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gltkyehro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gpdxllccu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gccoyrqbn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/glskggxvi.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gtbyuidzo.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gadvjupgu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gquefmjdr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gfcextjxm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyfujfhvc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/goucqutdb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gfpjxggxs.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjdwefmhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gikkmetvd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/ggsjefvca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gqckghnsp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gzpjmmevs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gonsralrm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gwqcmlhyi.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gxsxyoyjx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gnpgxrcst.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gpaweojyw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gaczwlqgg.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gcgiwsfol.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gdjmymald.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gmvmrghej.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gfamsvtxh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsluiekll.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gydyrspyl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvyywyghy.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gfynzhssn.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gelexvqxl.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/ghiysxmpg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzuyvmono.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnytgxaiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/galpuuwfg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggsbepwfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/givgpjoed.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gzzrskdtv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gyhurlrhk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gzyzrprrx.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gjbgjliyl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gjampwucj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gragorljg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gulayrrjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gguxkecel.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gdhrygbso.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gwujvygco.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqsmbqyd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/grfvsavsq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gaarjmhoa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gtuznoflc.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gbheoaciv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gijtohvgn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gsxzfuuau.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/geovpgalt.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxjxiecxj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gbjpvzwaq.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjtvgbywk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbylxrbsv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gcsoitzar.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/guizwqpdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gbdbrjqml.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gvaenvhxr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gzqcdzbus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/guzipmgac.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gkkhohzje.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gswtqeuwm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfwozeeno.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gzgwivbjf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexnzxjtg.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gnvcknlch.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gmdvjbmeu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gfguakpmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gakikafrq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gaemuehfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gbjwbxjnb.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gsgyplizs.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gcnznblog.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gkpngbotz.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gcjkiqgxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gtkkltqmn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gvclhmdfi.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gxgprvsbo.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/getmwocfc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gztwwcwus.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gmtcczfxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gmavyccee.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/geexleheu.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gkmjgulja.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ggrzhrwhc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/geopuwfjx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gisaqpduf.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gvoqttcmz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gbxpljyro.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gsurctqai.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gjyfomxlp.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gyeoqeeax.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gctlihycx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gvpwntsnx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gmvmxwxjh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfcaklgga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gknspgizd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/guxotuefa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gmukymzkg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gkjfenrkq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gfqddvbyf.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gxzkivrvb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gguvnbhbm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gauaqydcb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnmisaada.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/grjftbjyo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gabzdjyes.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gfrsteymb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqmsinrbd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gcpbuspel.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gonpbvkcv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gghrnsllh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/giuhtgbzz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkmddrmfi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gecoadbiq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/glwobnflx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/ghmkaoqmk.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/glpooaxrt.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gkuflziix.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geehnkhdo.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/glsuenpcw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grwynxsge.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gszsctxhh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/geajpiezn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gevpmnsqe.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gabvzobgv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gxhybhprg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ghjpxjqrq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gihyvmobg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gqdftaxgd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/goikemplb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gjuwimydv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gevjszkhe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/glaifgvfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gtjllxgpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/glgcluhul.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gvuumvpwx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/ggwqtpqsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gttovwjpg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gdagbnpiv.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gpzulvjxi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gjnfiwlce.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gsggwepvp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/guliklheg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gtemluxnl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/griqbsocn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gnhescmvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpgmieit.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/glzmtcdam.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gwgbbrchx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gknimogmj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gglykfaux.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gsugziego.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glsgvwwpr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gdzffnxur.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gpkvffkbh.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gnvlohlai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gjsnkzsda.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gpzihfsrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/ggpdlahsh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gmdccuguu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gnvvvdnht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gszonectn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/goslmcvjw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwqgkalwe.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gbzhmbeny.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gstoeciog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gdnkhcagh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gfhhfqiny.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gqlvwpzmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gutetolxq.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gukpxvuiq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gcwrqmjqi.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/grqzbbacm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/greosdpoq.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gwyiqrxaj.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gpnlnjgkt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gxapjexxp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/glsoruqdl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gftdoplcp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkjtfsdqi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/ggphxyikd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gsoyyhexf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gkdjyzrjz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gnegshfxq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gwacrfizb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/geaatiybc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gutiaomrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ghsegnzhc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gdowfpezj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gxvwumrnf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gzwxjxrwx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/giaigbcyh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gmqwkwbis.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwhuubqcf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gjrpqxxnp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwtlsnlvj.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gmqegtahx.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gjhnvebqw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gtcxknrmr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gjxeddulj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gbsarmupc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/guozwicfl.sHtML

);
来源：http://baike.hesvh.cn/Article/details/giizfgace.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gcnffhoyj.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gknqubffn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gjoqxlcow.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/guebiazil.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gnnpvrnxa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gkuamnzkq.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/guzlfvtfy.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/glfmhrusc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkcfqhkwf.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gjglbwpgz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gyeucoeix.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gacdixzcb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gbcxnxcdn.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gxgeaeuud.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ghaltdofi.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gvxtakulz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gwhxzqlbp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gmintmvcq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gcvddppij.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gebeullbm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnuiulopt.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gjutwfqvb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gtnuhudvi.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gdxkbaccn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gesqlymut.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gxqxzppqz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gaifdxjpv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gstjjfcxm.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gmockbrkz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gjwakgdfd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gyiftptjj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/ghtnadigp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gieamcidf.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gjqnekfpk.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gxcwlbmfa.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gpifqhtfi.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmfjudima.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gfyzkduxz.sHtML


<!-- 参考信息 -->