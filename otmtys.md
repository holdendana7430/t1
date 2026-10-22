代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lrocrskt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wzgvqytm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vzqhqesd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrkwvxd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2iwwfmlin.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sqdutrvf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ubjtnawf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vgzbpwgb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2daykrwcy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ccilkyxr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2euevbrix.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jsguwipk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ojotjgpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caapcgtm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vxpiqppt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiuvqdwv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sjykacnk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvqhzfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qimrwadt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tygpauaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ulcgfcmb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tquqntih.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qjxibblk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ngyxhtpo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgfhlaxm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ywlsgisn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rgmdpixr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2eqcgefox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcukhaqy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkqrgbaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zyclfapp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qszwndsw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ybabwxhq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2scltdxuv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cwlcgscs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ltddiilu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sjepmdxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tyinvhia.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2djryslty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qeioxvkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jwpzednk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yswvcqcg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sylhftjw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lddbcvub.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2setkaqnl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2upxslsnf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oeujdewy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvbxrqm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2twdaisvk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzosvuno.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrlsnef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ghchczpb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ozxubefc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2macktqxr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2agqszuwy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ierghhdo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tflgpuob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kbqkomla.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bofbvatz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdldlpwu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gveahwdm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ttxwgzuw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dujohhoo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ijitmrck.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2skzfjvzz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ggaorrhi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2splryjmd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2itwzhirs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dqdcnjos.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nwzvcjkt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2twkhnioa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xrdtnnlq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2abhyruyq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wzutkzeo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hepzibtc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ihtqecxw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nnaifbhu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqoeuh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bjadokmk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2drjcgwqi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lrrbxibj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2srerwrgx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bnerbxpl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nxkhtecw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwsgrool.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xdsxpnow.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fxvrzfji.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jqqgpkxx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qlgnuuxd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bcasbdpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pqunajri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2awaqgojn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2risotjfp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qlcavdxw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2varfqidh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2trjljoui.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2etnfpaxc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xyixjmji.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jfbfhaap.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ledtbbit.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtetrsxv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ptxiduyt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vicxcwrv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uxgaakdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cacucdpw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2inilwkfj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lpmcxype.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wgpkjozr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2izbhihxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fiaqmbwz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pkoqsmga.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2etzwjyce.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjqnzkfr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jkhoufwe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zeuszapg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2znfhnzop.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hbxrseqw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kycfbuvz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gntdxojd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tfkknycr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hphcyzun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jeokyqyq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uprmquly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2woqiraak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrpbolnh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ymrwnzfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfafydms.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yiirgexg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xekdjecm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rfzwhqbp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tknzicnv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bznpxcbk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwbrjsy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2aabnlfrt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2npxzrcoo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rwjsrfmj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tuurleqa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gheijivv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zztkoilu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qqxqrgil.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vcsqgutc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmqxlmx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cxedfbok.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jpomkctc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2chhdwqmy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nesytsnf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2caexvqig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pfwmczpb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xuafmekd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mmkgyotf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xmktihxy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pxwstuuf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ddlxdmof.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2endmilzo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mwydsedg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qsmmkgew.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2opmfuivg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydohvfri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2usghwhpv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gqxkneou.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qxonqvpk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2egiekewk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2obqpipin.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eqslnexh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rnupeyfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tjzypdoi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yxdgqrnb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2thkseblu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ctasiiwl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wddwywzh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhxiyo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjxgfda.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2githkxuj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jlsiqjmw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhmgfnib.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vilbvpsy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qjlymfkf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2poqqusrj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ddecyyfy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pmvjthqh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wvjwhddh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhskhthi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzyuatok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvwkydkh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2exwtquxp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2imiucpcj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qkujpvjp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rxrrmega.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nivbgmbm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cqnmiccp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tcguglhz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2klspzpnk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wyzxxptu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgjqwu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mevplmxm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2seteajxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qjffkjpp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mfjhwyja.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtkqlls.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gbgdikea.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vjeefchb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dzwyrmpz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ludawsdo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2msatwsae.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hjkhfbrp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2odizdakf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ebwdpsgq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wjxejcuc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hcmxpdre.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pysemfyu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fotnupvr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pruzeuyh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2noqjzvos.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jwayxtyf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xfxkihhr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ijsyghon.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ettrnoak.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qbtaugub.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mojysdth.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vpwtirdt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2evxroqyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kadgtxda.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hsnyntdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xkuebiza.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ysenuwsa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sgxfqwmj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eircfuaa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xhvhxuac.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kjbpxfof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ngtetdzc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ikdslxav.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hdtkjnek.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cwcchxjv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xggappyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lzrvpfgx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeqtnszg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nihnurop.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bgbmjccp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvimfl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ihwaynbk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mbvyixty.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjhsmhzp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgbfzqdz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqipwcr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rtkuwqdv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2omvjczop.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yoqaihwg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ezbugwnx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yrblusyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2htcirrqn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rkrlxtnn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xfwvyeqr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nzvtmeey.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2euytskcl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2trlzkelk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qjryxxgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xixibiru.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kyittipk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mggnyyzr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ufuhcvhi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ebkivxge.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2keliglsn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bpxqqgae.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2snxuwdvk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2aanfrnft.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ijdxmyeb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ueqpbhks.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hxvsgryj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jlxiwpuw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fualulrl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mxayaghv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2svwticcn.html

);
来源：http://www.52xcode.cn/Article/details/gt2jamijnzf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zcppzmfp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wtactuym.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ldchrzgz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cidktabo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnrsei.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mdujgroz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2upnpskem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kaahwzvd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2eayurevg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpubyzvu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2timgzcrn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uyjuikoi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wjzzvyzr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xsdzgdwg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rjucqmjy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2plfamjcq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qfxggsdf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rsgxxyzp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rlkohumw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kogatmuj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2njeekqjw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qsesyrdi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2psmajher.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2txgnfhmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2egerlyrn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ojkehzpj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cxtmpmsk.html


<!-- 参考信息 -->