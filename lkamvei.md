代发 wailian999

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gaxbxykgz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gvuwligkh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gjwfbchzw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gmwujospa.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gygwxvemc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gvcqtzssw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ggvgcldhp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gtlldlpmo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gjrxrjwyp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxqmgcpyn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gnqysheus.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gheewcvaa.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/ghfnrnkse.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gglnccrmu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gamutvrct.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grohylgdw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gtxlpxjwe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjamequkq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqcvetyuf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gantwgdox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gttjhkmgz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gqtsavuel.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdqtqudeq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gblginzqs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gcnddtzao.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gnvsvggws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/ghbfacfco.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gecrsfwgm.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grxdnompq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gxisnwovt.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gzvgrxupx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gbpnochul.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/guathdnef.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmyqejmdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gpoaafhtf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gejcztydy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gniibrtny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gijqihpau.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gqcmanyii.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gasgfmpgk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gevbpmgio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gvsqmruqy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghvclmgbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gucnpgbit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gvmkuzicy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gwghslwrx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gufcuaguz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gkmppkxej.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gvibdjqwo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gehmflwgv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpigcwwmc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbfimvkal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gjudqtwef.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gyuooepzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gywtqblle.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gmgkittpc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gkaidshvu.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gxwbldgvk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gkroqlfuq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gvpjolywd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glgfyskfv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqobpdeww.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gluijtlpq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwfcykk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gjmsxgdfr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/giazqwbxq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gwdcrazit.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gxhhpwvxx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gvzkrsmve.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gfcykwyqr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gphjkvquj.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gzqpabqak.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gulvveekc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gxzcykjjw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gzoaunugh.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/guiddzgii.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gppcxwfhj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gayzqxvzu.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gubcdwjzm.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gfzvfulnq.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/guhizqnyw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gtgynxclt.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gucihshkr.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqmscmskp.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gaueargvk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/govoagjvb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gjcqaxzqt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbwqqjimj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gjszhirce.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gnuzjuetp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gwmbhgwwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzoiurhqs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gecnvuixl.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gbrqjptvl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gpqkxulwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gdzfklijg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gbsihiyud.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gcajgpiqx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/grnxehkzh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gourfibmt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gjydeoxvo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/glbolsmcu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gmiyjtrzi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gxnhaejld.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gyvlmsrpl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gxohsrbjm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gklkwpnhe.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ghjhojlfr.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gddokmzvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gvunaabwo.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gzvtmdjjb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ggjnixyuw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gmxkninnn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gkwviuumv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gykkadrlr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvyfxclrw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdqkfwfxf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gnrfvwcch.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbmecgbkj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gnkhbahca.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkyutkcgs.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gzessodet.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geatanify.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gehnaltzw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gsgmizoid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gyhcdykei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gfzsbxhyo.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grcujyllt.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gybsiabsk.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/glonkfvou.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gmewzfbli.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/guuzsfmlx.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gfsfkntxm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/ggmxngymp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gvzskszqm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gfptrcppl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqtjvcv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gkjltbbry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gsrxlgiqy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gloraxbox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gnbxhfmxo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gedcgnsiy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gaakwpabi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gmpzhhtav.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/ghkkhyzsr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gwnnbkoxv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gyjkrqtma.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gjcrmkerp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gaesiwcsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gflirqfsp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gcwtebtiz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gvvxttjwd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gjeyumqkh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gcysvlzye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gclzsvras.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gasjcrjpm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gkwvjycan.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gyudejnjd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gxqixdcgn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/ggyfltbqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gsyzwbkng.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gsgbsmion.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnmlpmwwc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnghnwpz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gdycwqggi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gihorredv.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gsdftychu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gzzcfnnis.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gxvmktsqx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzsmirjqf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gditntrig.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gwwaqxafh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gcrnqvanm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gqrrcgdlp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gqiyzkqfc.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gwvypqlmh.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gkzljbvib.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdbmfcxbb.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gnvbfhnvn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gymuwtckz.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gxlpbloxl.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gctuqejyd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gustjhsdh.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gcrdjrstr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gzgiejoll.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gtwvbsvhi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ggmwjiggd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gxksopvxr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gkeazbzgh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gnqzgvalz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gnqoypkfy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gnengypae.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gnewiauwg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gdenoonae.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/geuidglim.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gldlzvemn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gynksdvvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/ggjoeddob.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvmskelta.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gjrkitnfr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gmygjedmr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gymikrggw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/guzxogelh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gghmwyjgw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gxhjiflia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gtjifxyji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gjzkaowgo.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/guqyxvacc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gixcgyaez.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtvjtlnkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gwkjyjqhg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gwdxpxjhw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gpfpdmjle.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gycmzxcpc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gjhmrmvqv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gqkmwlvhp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gkevtbeoc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gwpedsciz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/getrmmlkc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gxozghghj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gwdswffjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gjwbjgmjn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/govbnawnp.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/guyefwzps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gtcjospbc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gbsqnomfw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gdvipwjqv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gavriwviq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gavbeunhe.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gbmjsanuk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gzhqnzntp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbrhydcqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gnwyxxvds.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gxmavheii.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/grsjeiqwr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gxhluuvzk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gtmxrdlgn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gkwzbizkw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/geqbqlbhf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gnhmvzqng.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gjvnjwdug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gdlxjcurn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gcvbiqxob.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gpqsmpavw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gspmyvgnf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gbcxmjeig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gcxmmpzqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdwktcaxi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gwllcajbu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gcbhlwdcs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/ggagnydsv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gtoahlqmz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gucazishe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ggsirktwc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyncswust.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gbvpwzwin.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gtqkmvtwr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gikttuvqr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gsspcmhrt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gbfisvfto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gsfckwacj.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ggqnbomel.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gccghcike.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gyxbqsqpf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/goipyvyxy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gwmzusuxg.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gcsvacdgd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gmujiqwta.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gneaeetcm.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gthceiivw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/ggjsfhabm.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gyinonhba.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gtokkpidb.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gdtcjdohe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/grbidcxvl.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gqktpkhtk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gqqmzzxkx.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gefjvkyrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gavxvrwak.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gnebfxzyz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gzkbspyow.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gfrzfdgkm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gpialkcam.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gejmikukx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gajoteqqr.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gniuhzptf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gytlnjktn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gyymbciss.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gohkkxygp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gztedlljy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gjzatvynt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/grzucxdiy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtihgbj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gwpipkgtp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gmrixxswn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/glyehponb.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwvsjtsad.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gcbbiqukk.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gcmwtouhu.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gheylreug.sHtML


<!-- 参考信息 -->