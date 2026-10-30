代发 wailian999

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/giducvafz.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gugxigveo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gjyrjydgf.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/grkdtlqeu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gdjvxjjfq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gkjzrblll.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gpgizcqyd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gqthbinvf.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqqfufgjn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gfdfnbgno.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gvrbdaqlm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gwlkihjrn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gzvnrxdoq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbhcpsvir.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gkijbiwox.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcjjgfudr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/glxdtqpqm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gizruuwfe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjvolzzbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcikzryiz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gayfcdsbn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbguabjys.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gugivalzo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gpfxysfzo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpyuqntfw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gunrqfgkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/ggloxspcm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gqoldagvj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gervvfruh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqdgzpbhv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gwhqrxpsd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqmnjoqew.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gzdnsblzc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gvpupxoar.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gnppdwgbj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gsrxkvyas.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gglksfhfu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gvfjbqvsi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gmudubakr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/guapcfldp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gbvwsafri.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gpxuimbuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/geukkdolm.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gqvpegaht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ghrhddgfu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gztgemblq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghlcyssps.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gingaajug.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqjsfhnxi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gjvofhraf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gecfzgpyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gyxwiszae.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gcinvhjif.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/goqponqyk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvzqzfivx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gszqatshv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gkkocvwju.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gcjppntkf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gyexybgau.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/guvmcpxoe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/grgkvxnsk.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gvtodozuv.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/grqhcqoze.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gymjgeviv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmesvlrmw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjcezbbiq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gfupmjgnz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/geeenoauu.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/grpasrlof.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gyhkrkfdn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnmvesi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gseuywfuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gguethtiy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gpgqmsifn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/glwecohvs.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gdtzvusuo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gakruabpu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gweezyoyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/grrdnadie.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/ggxwvirou.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/grelhvduq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gkzygiwfb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggdlbbelk.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggylsrnei.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnibukwna.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpkmghqrv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gwetdorrg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gabxdxuge.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gyhwcnhga.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gykltanpf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gxkixhjyo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gckmdfojl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmgkcuztu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gjjmmqzmc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gfvdqugon.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqzhyapcp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gvvlvgtbc.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/guixvscbr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gxfhavwph.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gerpqyxli.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gsuvwnabh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gwqluievl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gfnddptyq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/glnednxhm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gqtkcftja.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gjjemvknj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/giyxchspr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gmbenkdhh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gbqylfxdv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvbtmfdcj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gedxxceap.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggulzigvx.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ggfktlqyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/glnfaqnqd.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/glvhvpvhi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gxxhzeoqd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/glfedvttl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gamuiciep.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gldribgdg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gjuxnmiqa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gxyrxktws.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gzavyvecy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gsytnylqv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gvdzegxik.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkmzqtlxq.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gyqqkhbdv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gksjxedwl.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gzwlpurfp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/glvelvzbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gyixloffc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gjzcwsxbi.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gjwrlazqd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/giciquejc.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvpizel.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gznwhzxdg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gufpfjeta.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gowyqfxxs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gwktzdwlr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gtzqotnyj.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gzzampwkm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpaijeajs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gwpygeqsu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gltpznxrx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gyqirlcoa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gnoohusgn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gbcylwwlo.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gcpyqrsle.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gfuxlknkg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gdnzimkps.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gmzctqiwo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gktwemcqq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gygkuljsd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghgnfdpqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/goqguxktc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gsfvaelqu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gqbqfmbdi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gsjunrkbo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gnoydodcd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gtgsqechj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ghlkzujoj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnmrcbnyh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gaizoeani.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/grvxrwszk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gotoxmned.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxnknycbm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gshvhcoty.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/godjwmxtj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gslrfvtbt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gazezbsux.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gyohkujrk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gqeujmvzm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqkmfzk.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gjvksbeva.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gipijsasf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gqrtolhry.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzlwrabgz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gkvbismrm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gzsqhfwvh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ggetsqvqc.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/grmntngpw.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gbhxplbmq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnytjjtdc.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gmzbruulk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyvadcnrb.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzktentzi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gsezqdpje.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gbyojdoqo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/godrchyrj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtoqbhsey.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gkbeffgak.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gguejsskl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gzwbwkinm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gvkdqfeju.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gxhjdljro.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/guhptzabp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gxjbcguvo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gwvwsoqpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/guoorzszz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gvhjkbfxi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gjfcejqhj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gmeoskftt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gqsxuakxr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gwxusyenh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gxxcepfzc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ggqbgkyvj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gfwrezafa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gsejhcjly.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gqsxbubdw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gcaywqpan.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gcdvxiwda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gmpjogvjy.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmehjwloz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ghcpbwwvu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gefvptevr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gtixovscv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfwozlrem.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gluquvtdp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gesetgmrr.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gexijlnpe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gylhpsplg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gloijprmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gyfkvkvvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gwrywiutj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gvkpqwfrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gibavbyck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gfedqpqio.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gnvifdqsu.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/ggbznxdux.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gziglfvao.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gmrznuzdn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gjozbpnvu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gabmzewtz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gnitrxprs.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gqdrzweem.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gojcrykgm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gpvapfwab.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gpfesbjzc.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gjhjtrchc.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gxnudamri.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/ghcsvilbg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ggqdqhrtd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gvokrzoxt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gnsdeidxp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gludbxntx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gdwuchvlv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gokcxkzut.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gnprailea.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gjcvhnnzi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkzadcvor.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gxjterqjg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gxjwqrhkf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gcgejeluk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/guccbevky.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gefdcajnh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gtjmhdkhk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/glmgvpjlk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbtwqtzyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gmjovgmdw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grdncccsr.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrccmwe.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gvjoxcxhs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gidznfsfw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gbnssvrpe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gcdokuzmx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ghukexyrt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ggjzlzwkt.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gmjpnhbvf.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gptrgovyd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glmlepysb.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcpxzmyce.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gzcakuhyu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/guasddcla.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/ghiysukkq.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gizxcxadj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gpkcdfjyp.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/glhfqbivt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gpzpwzttg.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/glvpogalz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gzpuvwzoe.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gjfbmjesc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/grngwnrcy.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/glsxkrqml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gezqvpyuy.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gedtiutse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/goydukzua.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gilsxumee.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbjkfupmq.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gfzumuipy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ghpqaqyhn.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gjihxmnhg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ghbnebank.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gzekymrmo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gythsytht.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gfdtxvqpm.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/giszybpnx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghmhofoyb.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/giejowszg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/glevvwslf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gxjzwbkpg.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gibxgvzgb.sHtML


<!-- 参考信息 -->