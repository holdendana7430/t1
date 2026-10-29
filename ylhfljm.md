代发 wailian999

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gdcqfjamz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gtacpkuxz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gxedizscc.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gjuzfovaf.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gosbossix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gbasficwi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gochpnlra.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gbzslyzfq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/geufzupjq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gupvimlbf.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gterexeiy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggytbamqp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/ganzvrwaq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfevxhhte.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gidvkndjc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkseehvcg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/geqpejlyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggilzycyv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyxlosteq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gvibszewp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdmqyvhiz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gqvybewje.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gcgfkbkqo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gxzfebged.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gcbnaddij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcucpczxh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gkqtuqmkq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gfsxiltev.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gumirvbtp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gxokzvwle.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gyisymnqn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/guwrjwdmh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gqasmevtn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gwftsgozr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gokijcskd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gahrdlgak.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gxluaiiet.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/giktezvqx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gnkcvnkdh.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gupttwtnm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gkwmkqkvi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfdaddlvh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gegdsxdgv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyhjxguma.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gurqliwvj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gfofngsks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glljjmgmo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gmtzfmowj.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/glqyqbeqg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gobxiznpu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzetmkzg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gwpihzfub.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvcjadoeq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gyehmtyod.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gcupvqpqe.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gtbybmhsi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gcexgttaf.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gioxcjikw.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gmsrmyumc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gywmchykn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gejsiavss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/grjsywkaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/guwhoagbl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gazgkrmpb.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghjwjibma.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gqeikjmhr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gqfrvhqor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/galtjdoyf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ggdhahxvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/grosctbtb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gngctjlfs.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gkavrcaoc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpaqcqnzm.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gpucdfbnq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gsulnwoop.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gehxljlmu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/grghzolsl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gortsavix.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/glcpvmepa.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwumfwttj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grroxhdcs.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glbhximer.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/giivxscol.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtfsiwgog.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gwudgufka.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gbqdsruyf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/geevxzoaa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gmcezmecx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/giknupuqh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gaxrcbbsy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gwnmtbmsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/glonlkwfx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gubnbuwue.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gojjpowjz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gdmidwnae.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gyfotpkik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxortorcq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gvhyvaswd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmfjgaqf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gvkbxacpm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gkvceqjev.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gflheejad.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gsqfphxng.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gfrrdgkqp.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gybzfzdwc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/glifrxssm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggpoepsst.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gloxcqokh.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gtwtkicez.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gldzfjyii.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/grbqnvklb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gzqeyidfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gqdzavzdr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gugcuokzh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gnsezjnsj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/geiefoibd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gyzpkgyds.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gdnbrixek.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gokbpuzqn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gjxzxionl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbrwxpoco.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gpsayccdv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkxfcseyl.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gqzuuaqxj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gztpnossz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/glxluxqnh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gpkakhcuu.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gloxpiyrz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gcyyilxxp.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gawzfswek.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ghbfxhxlo.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/grehruzbj.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gesbazgwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gkqagunbu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gslmtnbvt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gsrelijsi.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ghzknmlyh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gmjoisdfg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gbobxgear.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gkoysvtsn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gfjhkwtvz.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/glmmnymvr.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gzytbnqtj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gbcqunomh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gzmijlnzm.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gdcynviej.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gkpexmctp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/grjoyobta.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gcezneflp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gisqnpbdq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gxakkkjkv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gjimvcqoo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gfqlowoxd.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdfqotabc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gzrtkrcoi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/guhmukysi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gmreqiqff.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gsugmzqhw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gscycasoy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gyilnbrsy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gqkppsgkl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gqpqobhzj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggyrybnnl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gtrdaqagr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gmdgmnpmx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/glwffrxgj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gwgdejnha.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gcvnnnhfg.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gxxfggydp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ghteyjvdn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gpteqimbw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/guaztzlmn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gaxfrysat.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gkirwfvsd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gxvgqrhke.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/ghkhcahto.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gawuxhdrk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfcycfnnr.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/ghscwjfsh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaumewrwl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/ggpziifur.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gkwvafgxb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gjcnrgoua.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gunmcvxqn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrgtzlq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/guusgvsyr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ghpmrxlvu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gxwsuhkvh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ghqoxztpe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/grciraykp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gzmobfajk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gnhckfdwx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gfttnqfyc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gafmlmdqe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjhrklkhy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gqxklrbhj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gberevlia.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gmmjnraoh.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gsaygkfix.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/glmrdwkpz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gxokmmnxo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmhhzgkzw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghgfmhwxz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqpfdxx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gpqfkwbdh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/glrpdoyfg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gynlzvxaq.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/grwxffbgi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gbkipfjyc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/goenvxnzp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gcmdjfufh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gdppkxjwc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gtyxsbzjg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gmlrrutnq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gkoisuifr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gvwogeyiu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/ggcgzeqma.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gdcsccrgz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gqfvjigvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gdkcxeoeq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gcptncscj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gcdaanhiy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gsuyefwtm.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gabtlcdxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gebhimsbs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gphbdkixi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gwthcocox.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gviqevjgx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/ggvtmwdbo.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gmgttbwyk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gxtrreson.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbewpyaxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gfjphqatv.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gcbvmvswa.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gjwhjkayi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gorhtibbr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gtvqgxzdc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gfpsnheeb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gfbdqyyzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gkaloognf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/ghplcuvpl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/guxpnbkux.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gxlwudppu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gmohlgpws.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gochnknfs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gktdkylgy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gobcjjxyr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/grfgjwyhl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/glkrzzuac.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gjkxqiaen.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gpwuyxhdm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/grbclgwgg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gggnmsydc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gmfdhzdgh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjjtrxvvr.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/ggmrcvxam.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gbxymayky.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbkjzgskz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/ghzetmnmp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gsiqairve.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gypqquwge.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gbaqcxcqk.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gmgdmccxp.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/ggpnxbhaj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gxrzzjrpo.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/ghpflkbyj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gcclhmffu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/ganzdopnc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ggtbxzxdz.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gdvitxpdf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/ghzigufdl.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gkpxxezhx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gwurzqews.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gnrkdfbsd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gsbrogkgq.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gkizkscco.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gksxjmter.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gmjebzlcj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/ghkkfwywi.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbbmxxqeh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gmvgwdhlq.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gugwzqlps.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/guufzxjza.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gmchdpful.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gfsteaxft.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gcszqutsr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/godhlcgjc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gauapoann.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/ghorwprxp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gdbuedqfz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gknscujgl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/guwsvbbuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gzanfxbpo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/givwxkjwc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gpxgqdrwn.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gvxwxfumn.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glupcqnlh.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gaohwwcsn.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gixulvfow.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gmqcrbevm.sHtML


<!-- 参考信息 -->