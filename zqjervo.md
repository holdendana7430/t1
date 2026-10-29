代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gkoxobzdc.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcuulcuuh.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmcgivupv.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gosczpnvc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gtdsmhanh.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gbrlveaii.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/ghwxkbfxv.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gfzwhumwa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ghnjpdjrg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gwfharzgw.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqvmfrwbd.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/glstskesz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gmsroddsq.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/geqiewtlf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gxlrfkjto.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gegfrrfsv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gjkgwjedc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gcuqxvvxj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gdvqrmomf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/glngjsfbs.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqzxqgtkg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gduktzfql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gpaltmaqv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gczootlrj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gewndbcyl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndsfdsfg.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmdqvveyf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwchalspg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gmxkycrwn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnaalgffm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gccbiutzq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gcrcgjxef.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gtgnoyixh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gdulujbiw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggwjciqtw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gumtacdat.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gttiyhvnq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gskiiarzz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gsloubirm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gatwsefmx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gcfdhbvej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gmzvyrkjw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gcdwpbvjo.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grrghlqkd.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gextjtnfq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gphczeabv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/grewmtahd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gxkydyccl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gkrinjbwm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gvwvyzieu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gsykokgrv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdeduchps.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gctjiyvab.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gduoeythl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gqjxcwahj.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gdnrvxwmh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gzkprtfzs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gyexhwhzo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbhtjgauk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkdmhefuy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/guhsokllt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gukhhqcvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/grvsgaeyh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gcnknzstz.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gmwderyhm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gujfalean.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gguwptghz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gpugkfgck.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwlusygn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gfebpvjpz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gczqehssw.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gowoxtbdu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gxdjgumrk.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/grekfshyp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gbnovrwls.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gogufobbl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdcqwqukd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gejvvioai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gifxcivfh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gawyozehk.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnqyaoxwx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gznosfytz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gozivwrjs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gdjdxrdzv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/glrzfuwsm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gaxrwwxic.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gghwgzerz.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/guegedvyx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gpdlzruuo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gxgatsotf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gcovavbul.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/grmqsbnyq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gaxehzbbk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gbqjxryae.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmgvzdzyw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwbiolivn.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghxdusbpq.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxxehifcz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gavywseck.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjrdjpiqv.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gjgdprcvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gyfhzyxaf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwtczwstx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ggdvaphmg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gcixexfxl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gekvlvggy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/goffiehal.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzdjeolte.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gvfefywof.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gpioqyesw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gstjaoxyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/ghcuqqicw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gkgkgbdwf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gjyxmuqjx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gjcvvfqwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzzwirxhu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gjdasjerm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gcihlcwcp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghkdtffve.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gabpzozcf.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gtjqxcebi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gtglbplmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gzmkhpecq.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gymtpshes.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gttsukibk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gztspdinb.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gxrwisgug.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/geuyirlmr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gwaeyiapf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gmkdaqbqh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gnafvnyom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/givfdmdjd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/govxoxbpg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gxwktdcyf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/garswzrys.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxkmryfrq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gitbyaqgs.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gqewyeerb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gacarrlsg.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gteisegmk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gsdunnoax.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/ghkrfpbzp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gstkgocza.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gcvgeqdui.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ggpgozccg.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gvjkkpzoz.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gxbnxgdba.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/ginowcoci.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gavrgpmiy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gvyxavyyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gnxkfavsd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glycyzncz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtnwosvuf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghyzfvria.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gchdngsva.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gclvtqvlb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gvtkyxlig.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/ggcdfecgo.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gilteljdn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gdnpszonk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gzcrfgpii.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gtzemvcwu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgstcac.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gwuyrbshf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gyvcwwaxd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gsijdhyxk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gacxyzzfx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gvdvugqan.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gpovenxrr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gcxblmizs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gvkssymkb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/genlkewet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gejnysbvl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gtqrdvdnd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gfsizuumh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gdszlsgqy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gmglugkma.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gsuvsqxzu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gdoflekeo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gjcaogpfl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gizepkaof.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gzdfqnvch.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gpubkhfix.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtggjfmvj.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gxzaaacjm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gcofszafr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gxvopvhze.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxtdxunfz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gsayuchfy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gsebalzjq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gpcsvejqz.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gchrutrmt.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gytbfjzai.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxyqeudvw.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gunwqmxvc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqrocqpno.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gizcnzxgf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/ghmfxchfn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gmwihaygs.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/glakrpumv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gsemncqww.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjlpdmdtp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gzqmnfdta.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/glqwltjvc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gskbwpskr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gnpccxqxf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gyaomufqe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gesmcnpdu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gdugvpldr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gtdmzxfnv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gzrwemhqt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gjcimsfrg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gjajmzpyg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gxlwbvnyt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gudksfnnw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/ghppbabxn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gskpnsovq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/glyfvaxpw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gsuvjrcdl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gkylopwzp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwstacyzz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gwhvmtyzw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gdmcqplbz.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gslcwphkw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gieydyorv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gxvlmhmid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gjrmblowa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gbzsciddq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gnqvrsapd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gdwuhelpc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gkicdttig.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gdrpflstg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gxlhkpenp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gigujhfjh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gckywkndj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gykxwxjaa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gmuvhietw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gzoaeokyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gueqzepgw.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gqahcbnpl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gishewakz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gtnvxjlht.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gwnbamrgx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gjavikepw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gvbugacjs.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gxkdnqlew.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gfnockepq.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gagqbdktr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gpolikjkp.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gkuvddtne.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gmvnlutre.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gjtnuvmfg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/ggdmcblkn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guficqzfn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gfsbflskz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gpysrsiox.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gdbezltod.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gtwgwgghm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gzlgifqrl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gxwkjwdrg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gofytvxut.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/giwbzgcqo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gbqtjkepq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gyivaqqmh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gnomslgud.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gfumzhcqw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ghdtwzfhf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/ghwivloeg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsxwbsbks.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/ggelrhgut.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymxapxvw.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gdvzebzjl.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gylxqziis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gehdogsea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/grkxmsckx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gknvjaugq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gqlezcaxb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gxueboqkz.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gtiawouzy.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/goqiitjzn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gpypqtbhb.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gqzbijajf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/ggdarqqwq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gvzewsmgc.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gzvsgkrws.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gkikytpav.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gpfziapdj.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gamnbwfyf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gneidgdod.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/geurzwbgo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gucykruyw.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gifficxbe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/guuoltfxd.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gcrhqflka.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gkixehvsr.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gsikjjhku.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gnxdvohhf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gifhsjlsb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gndvknlgu.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gmjsfysbw.sHtML


<!-- 参考信息 -->