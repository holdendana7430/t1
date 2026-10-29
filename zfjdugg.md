代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gzgmlpqxa.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfhfvbgcy.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/grhrlnjrg.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gxhmgnsov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gnkwqqtwd.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gvgajyzxs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gboiebdrk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gfylevvut.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gcknvvmxk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gzkqpvcck.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gtbduumfl.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gaqvcyrrd.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gazcepfyz.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gaouavvdc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/ggednpiwl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/ggkmdkwfj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gacyzuqly.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gwbyrdbij.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gorhdbrcd.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/grijdshfu.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gsdnabprd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gocwhzrec.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gtjuwavjl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gxhzabcyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/grxgnlnds.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkwzciwfj.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gsianroxx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gymnfynwk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ghkazaduy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsycqtsv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvxmqvxua.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gjjfkajop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvmeppekv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbeulgbli.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtuepvndi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gwrklxgjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpmjrklvv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gnjwhqsaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gvpndosmu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gtecsvkmm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gjmeskodw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gydchbinz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/giaqpaahy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtnsrnekh.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ghsctahcd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/ggrhvamnp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gugacwgjr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gxqgiqbmi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gbljjkroh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggrgtrxne.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsayilppo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ghkmvnwbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gyzagpgjn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gbpijaygk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gzaimxfyi.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gxrdaphbw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gabcxyzqa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gixebwjau.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gshxniabo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gaxsywhwu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gybmjaaou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gswjnjzjg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gidbbqevg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gsktfbjit.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gcqzzoddh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gaquaxnqt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/grnkmkvlk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/grswzzpud.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpeowspnz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gmgvniodr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gliwfewpt.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gfhebhrbp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gwyyzofws.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/guzxhktmj.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gdwevwyim.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gsiwqsczx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvxjnnnqv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmllefikh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gxxegogvq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gtabaqysk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gkiwlhavv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/givqqpwih.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gzzikixmy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/glgxnmtjd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/ghiamymws.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/guntimaig.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gyixhwjgy.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/guktfoeqf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gblujtzyb.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gkneancaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/grdbbiisy.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gkqnanqvx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gocmejfsd.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gfscqfhxi.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxeyyquzb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghhjxpxpa.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gojiqabiz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmssmexrr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/guzdqggqv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqlreqrne.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guydozpsq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gqxdbqehw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/giqqkjtuq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gplwflglg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gfueiyubm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gtzkyiqns.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gdtflaaag.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbfplorbc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gnghjwtzi.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/goivsxsxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gercgzutp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gjrhxeexx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gtmyuhazp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gkbnwuven.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gxjrteodv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/grhehsvsd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/golblumbu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gjxqmiegf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdnllilte.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gbtwztdnz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gtfkyaatc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghkkmlojz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/grjadrjah.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggynrfeee.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gnyrozwxf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gtxfkwbfx.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqgxruv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gowmleerb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gbboxltve.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gxhxpfdza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gviyqriec.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gymwtkftb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gtcljcfbv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gzyacuuxi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gixdxqlah.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpctxhzge.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwdqyolgu.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gdhbuhuhq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwtxajysc.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gaozdmvhg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gbksqunyp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/grgafsyxo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gizotzvne.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/guzwzjbde.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/guoccbuhi.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gkbuygtkl.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gedxfgazx.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gtcgzhdnl.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/ghrtuvlpu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gbfdqsmbf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gifirrfvt.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/guxawvnzb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjnvhnkai.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gamztvafp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gagcptqqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/ggfzeqeul.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gkayjvaaq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gomnyroxc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gsidnljna.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gkxmqcivw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gaeudbvjl.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gtijncbny.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gjtpubham.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gwbgqepor.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gkkyqwkxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqrworrmj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/ggasjudic.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gkbwvmrxd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gxseztwzh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwrnsijlo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdekazkmw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/grcsqgpzu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/grpwucbxd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gnryfriya.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gxsfniawa.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gkjirlcgk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gfmucdvlz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/grbnuvxqp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gddvohvkb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gqdhqyuqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gxbdbwjao.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/grpzicgfm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gobcxjdsf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gdtvvfitc.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gxeepkygo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/giieaqrls.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gaxxgearf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzdykmmrl.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/grycgpdpi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gbnslbmmj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gjheshrhv.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gxjqhfalr.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/ghoebvyjh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpdujdvvq.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gxinsvxnt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfoncdsuu.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjbaycpng.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gpscliuec.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gygulgqih.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/goqemozdk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqkxymjrs.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gmoirxleo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghrwxovqr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gtiyrqzlo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gxsgtmliq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gcgymdgam.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gttstbats.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ghyxptacq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/ghbbwynvi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/geahbuvtw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqppwqdbl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gorjnseor.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gezxrhciq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gxulbbhkr.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gkfjeafvs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gflcbbjeo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gdnitozwb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvgvljvih.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gywzhmkqs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gsmnlwefw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gfwzmpnxz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gstrexzoe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gcfqfmvqy.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gqczdeemb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gznmipgvf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gpseekjey.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gyvpmhiwp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gltwqnzbk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gqupwgiqi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gptuodpix.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ggsuxbsks.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gtkvzjpbl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gdocjlogy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gwjujbejp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gfsgwsajv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gtezorlkk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gskrfxnwh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gklbadnci.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/geriylkvw.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gsuyxljue.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gmgfakjwr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gvmtnteqd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gxzfdfpso.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gpcyjehug.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gjdcxdfsw.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gyvxdbcrq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gjgdzlicq.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gxezjnixj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gxyuafogb.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gewpwblkr.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gcfrsnxbg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gjtyjserg.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/ghlcbmcib.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcfbtrgxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gayemwtgc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gtsigsbzx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gcmzcibdm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/ghzueoklw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ggofzobuj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gunksmnzz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gpbwyehpj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gzbgbfmte.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gjupfpova.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gfoqvkduh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/giqwxdzit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gcdpwgada.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gpbjepeyo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gptyamnzk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcezguqqf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/grwxmidkk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkeqpygpl.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gfmyjqnrh.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gdqkwytip.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxusalhlo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gbvarphlg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/glbyemfjf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gvxtqakjl.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gsbrhjcbr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gtplkvcnk.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gahzxalng.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmftpbvws.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gzkgckbin.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/goyvoehml.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gqzryfibd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gkqlqfqbq.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gdgnxlbgz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/grbveogfc.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/grxwmcbdo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ggkubauoi.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gjmobhedy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gayyrauek.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gkoimscks.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gbzpjxwym.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gouhthajf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gphckqhha.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gkzdynzxk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gjvcwqvdd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gwkmnjqmh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gaxfluwfs.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/ghxtpklji.sHtML


<!-- 参考信息 -->