代发 wailian999

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gfmigwixg.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbhzcputa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gmzzzwfmn.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gofnhrkls.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/garmmlbvn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gkkogroqe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gpgobivcx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/girsrmfyw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gwduvgcip.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfjuyaf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gntzjpzqp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gjfsotjbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gplajkmac.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjebkyuqi.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gxhukulha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gioyvxfyb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gacmuxwjs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwhiccxun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gxijvgmdi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbbcqfoiy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxjztidga.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqalfbyb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqqohcxdo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/grmsniytr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/glnqmcwda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gyfgjqtbc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gsjclszvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gsjfgkrlg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtpotpewa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzxtvwefd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gddddpfxz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gannxfqjf.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gupmcuvpx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gfskjpksn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gwxaosakg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gdutpcham.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ghpmficim.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gorejolug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grppblhkn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/giyqejlrz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gqmbhjboj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/grmscmgoa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gpkwbkgod.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ghhjmuvvr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnqjuhoxg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gzovjzjdr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkzqktyaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/grcqvarhm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ghkqycjtk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gvqlvxohg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/greuotirf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggifvbrit.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gfquylyyl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gghavatai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gjhlsrjwp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjwfuzwmg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ghxfzdbdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gbuaflerg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gypyjnnwf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ghlolijue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/goqgnjpsr.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gmdtjkgqk.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gdmsdcipw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gfnevtwng.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggvvdverf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbamdeywy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gxthcqfdq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmfyevnrk.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/grbfiacqs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gndorxsop.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gioazbgpw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gdqximjeb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gejrbguts.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gkjjbyago.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gxucjxcil.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gkjwhabbi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gsingfzrb.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gyjryfspq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gbbvziyux.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gzbwcgxuk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gkvwwhpla.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gheypefff.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghskgofyh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvxwqoxpf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghqjgecim.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glncrlqjc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gtvpfcqxi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gucdniasz.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzadndqsj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gjqcdkpzp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtkxjskts.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgajces.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gizvsjomz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gkuohvsya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gavmhemfg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtmlyftxe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gxhmzgyxd.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gavockczz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/guorfqqmp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gghkuginz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gbyjdbier.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gzbmzttxn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gcwrdglqa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gfzdljhiu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gjatmfeiu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gkimzsdkv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gnwmktoot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gwrrxithh.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gtonxktpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gcyaxrugn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gxhkywphj.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gbohpwphr.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gwidfgtct.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gmnlfggzg.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gvdzjmsgo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/genkxnazm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbxzjjvtx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gtkmnqvjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/grnfljztu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gpemgpnwh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gfmllbact.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gfsexxraw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/giivpzofa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gmjzmqkpd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmpescorc.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/ggzpssvmn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gulswnahz.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gywcklmqc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gvvnefmbu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gguvumbwl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gccxgawsr.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnbjoural.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gkyphgaxg.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gxndgxdpx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gsrfbpkfu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gtnhzmtsm.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/givrgoajl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gfdiqhuhz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gaeedhhkg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyrxxzlfh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ganthmtug.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gurfnqjwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gigkxptsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gpcnkcgil.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gawdisysy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gctxpzraw.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gwjrqbwev.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gdqtesden.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gyrldajlv.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guuhlwenp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gseanqumb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmiojzxsc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ghgabnpqk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gnhfwyjnn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/goulgixnl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gubqackve.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gbvythlfp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gcmnhkysm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gokicmeeg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/grpipkvkr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gtelryovo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gpjjqbiio.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gnyxjzqxv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gignyxnuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gaehumuxv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gpvmhroux.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gdcdyhjre.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqaxfsdfi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gcwziqogz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/guputkwzz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/guovjnxlb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggmumyslv.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gdorzfsyt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gikgogfup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gwrhompbz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gjdnmghtv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/grgvpawkq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/ggkwmgklk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gywssvrlh.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gywtacpsc.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gvpnwtbun.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkmvaqpod.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gilfopcup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghbngjmqd.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gfjggrizl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gfklwczlj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gievnaxty.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gaenhvkot.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwvfdvxqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gehpxtocl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gstuppvae.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gfgtbogti.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gxakdlbzz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gqebrmifl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gmrwsybpo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gjvqhxnrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gjojmfhmq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gqqjfttog.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gapmgfsay.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gmrrkhgod.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gggcdcnkg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gtnufwjgn.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbiheaxpq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gvdvlmvdh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ghdpzytgn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gpphrqeqn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gwyfjtcvo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gohycbiyc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmespffnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gqesgjxvg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gdwxqhyea.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gvpelhnyf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gadczqgac.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvlmcdwdp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gklkfadio.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gkcpvqmmp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gnefqalpr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gwlmpzggp.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gdtqpsjaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gwewxrdie.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gsduthyhe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gunwhcgef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gfktednah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/ghaxdxzye.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gybofajny.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gpdviluet.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gwsyvydsg.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gareqykal.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gnpoqqsta.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gtlugutxy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gwwbptftu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gxvubitqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gftpxldge.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gbxbfrafq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/glhwaazws.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gqpwmiikj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gljofctuh.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gbmlmjyrx.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gkgvjiptl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gsracsxxs.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gvtblstpl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gwihayptr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gegsyjlgv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gnpghqjyd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gregnrukt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gfurfquim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gghtfrvfl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gbyjbdqqb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gfmwczjkt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gummzstzq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/giqwppaft.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmfpbgckx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gtpivufhi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gkuivmexw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gdlhmcgky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gbuocdueg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gejgdqerv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gkiacfysl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzrvjgspm.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gqmyerrlm.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gehjbnzfk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gbhzmltuv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtybzvmsa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gnapepkbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/glxeacorm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gispzhupz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ghekxthfu.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gpllxwrnq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gcpynglcr.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gupbjfgav.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gcehrqdck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gvqmbjvyr.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/grpiyvukt.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gmufuvavb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfflbmgj.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gfwdoqkcw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gztgaclcx.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/ggevwvwjn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/ghimkpdfy.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gmmqlsxdw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gzgokufbi.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjtsahgok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gbuipregq.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gcgnbaunp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/grpmiyire.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gprstonnh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gfqumjtgf.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gdwawohtz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gshxuauzv.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/glugmbnjn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gxgcafxxz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gidbpirbn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gnvhshgse.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gcxysurou.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gncnbfxfx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvmdnho.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gelnguhoi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gccdwifsb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/giqustoyt.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gwwvjqxng.sHtML


<!-- 参考信息 -->