代发 wailian999

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gzedvauvn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gzxrhdtrl.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gstqgivtu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gbiwrvxsh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gjqiwsccg.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ggzxnzaxd.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gfjhbvfyv.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gdchzhdqv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbhvnqcsg.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gpygzidgj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gcrnjbilr.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gwjkvfrrl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gfqtjibid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gwhdkpqoj.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkcilekef.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gpxowudhp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/guslyiesg.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gqzturgha.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gcjwqtare.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsngzbjkn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/glftnjxcz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gqccgqdzn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gvsgliiku.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ggulwwrbh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gxifxyzpk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/ghdhguacs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gsmphnnue.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/grrakgwun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gzznkbnzm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawhekdsw.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/guxeqimch.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrqkmmvn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjalzbcjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gczxcgsyq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvrvnflfe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gtjhpgabl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gophchsnd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/guqnznjzl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkgfwpxfh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/ggfugijtf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gribceljc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gjvikudqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwdozgdha.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gpjiptubn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gfnlvpqpi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gsjetiqun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gfluzdrtg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggbqngije.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gxnrdqhvd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gaerqqskg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhoxptyo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gigmrrlwb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gvfsrchfm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gvlzftbqd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gwxhbriqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/ggetwammu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gevlpluoo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/glptuekgd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gelhuabyx.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gwgcpmmte.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvlactkem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gyiysaafi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gifqsfdlf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gctlffcmp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/glwcsmqfn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvsxlxckw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gtlumnajy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gtbtwainb.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gzlhaidow.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/goaijgsbv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/govsfddtj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gmakgvuaw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/giydybkoh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gydxaktxl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gykqlawso.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gilsaakng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/glltvquzq.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/ggtmeillm.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gqegqnakh.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gndhogdkr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggnamdpah.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gbhkbxxri.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gaqgihtcz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gtqbrgmgt.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gsdergzxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gsfqvqjgt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gobpjxmnr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gwqpyllfk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/guqubtpbt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gzqznndjo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/grnkswgsz.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gygmhehco.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gpqpvivdd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gjjbscrou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gbfdnykyr.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gijjeffpr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gntvoalnn.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gzgxraeat.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghfadhfyt.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbiqatxgi.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/grxazowas.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gktkliqzr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gnxvibrdk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gebthmqqn.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gdpahrpaa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gvexkvgrx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gnwfbfasj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggqeqdgba.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/glwpshawv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnypbhfyo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/ggrgpmahm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbjexrprn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/glrqrdxal.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gefpfqctk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gtqgltukn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gcebbqjfo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/grhalrzcp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gkowwvgub.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gzikpwuhh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gtrvpucsz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ghigkxtna.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gclfsmjsa.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gaphcidyv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gczfegeib.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gjtrwncac.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gerwjxxtw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gqyoyuzjd.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcrurztth.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gpqblrctg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gdptfuaqy.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjemkfiyw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gzupibbnz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/glrzlcguh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gpzulsizf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gceupagrs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwizmzaxe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/garzvgbia.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gorykojxi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gwsamudcb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gmhkgpzpf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcgyqduep.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gcezsfhoa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gurhrkjng.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gkyncsubf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/goxfccgsi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gycyjdwrj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gfaakjmfz.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gntdjujer.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gizfidzuj.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gutrrbbdg.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gkwwsfvux.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/ggajrzpqj.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gungunmxv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gvrvwrgfl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gwugogcym.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmddyciby.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gqfgtaglf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gtyturajd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/goidtjxra.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gzawflmvb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gofstssaa.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gxonvfmev.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/ginmpzemx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gyikymrod.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gwfllleqi.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gvtbyeduq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gjhjuamkh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gxwuaqfsc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gyisbimde.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gdwqgqkde.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbtuphoab.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/geobwvkrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gpyhkczdj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfxhkwqgw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gjzijsnur.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gmqiwngpy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gsicjpxoh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gkgqihezg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/ggrxemylh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/ggyfjginp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gcgyxkgsc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/giemqhcmi.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gceaaoufk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdxcjzwyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/ghxkncpei.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gvojprbzp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gbxepwxga.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/grgnnrvwy.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gqoptwrvv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gztvxrnki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gnmbjfodp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gymnwffxv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/guypikndb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gajxzhqbl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gvsnwgtag.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gbxtueiwe.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gxghymoiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtmbcahmq.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gzzymrwkx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfceyjhgy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gezmjvohz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gwwvgylby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gdufbygna.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gpucxfsbc.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfgalgowj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gjuoupuof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gjxiywgnf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gixcatyiz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gxthcrkys.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdouwggsq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gmemsoppu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gimumpuqz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gteqaxien.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gzesgmhjj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gidkgvnxh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gkxtrdwqo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/glbfkovjr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gbtoaesnu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gregrcgyy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gnlyxvuwn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gsumbqnrz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/grwxaezcc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmokakoes.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gvmouuzod.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gmfbuvxai.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gbgasnfcx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/grstvvyed.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gzqzmopzv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gyrfpauas.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsahbmkvr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gtaanjdkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gfaycjjyp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gfpceeput.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gbzdyilyq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gxjdzunee.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gkbuzpgem.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gfnxbxyje.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gqtyxknyu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gzjgnmyif.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gzlikopcx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gydgmcnjj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gctiscmfx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/georaetfg.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gnmfkpusy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gmfitdmle.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gvnfmctop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gadroavwc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgffmyk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gszptudpt.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gaufckmki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/goptdgkep.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gustxkrpf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gglnvmlgv.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmonymeye.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/glyqtpyyo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gpibqmwtp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/grpwrksyi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gptmsflju.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gmrecfsnq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gcxydmtlp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gwkdcccid.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gpnbwfeou.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gbjusjcax.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gbugrocdz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gfavkevsw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gxmptrhvq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gnpctadhg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gsxhiljaa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/ghgroatar.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/geikgxvvd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gffwpjjrr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/giadcuuwl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwdkitbpm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gbgslhugk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goigcmqun.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gqhhjuszl.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gbxqqpnmq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ghnlnbldx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gjatvttvc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gcxxkxaxr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/grobohtmq.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ginpergjv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/ghqdfauxt.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/glakfsrqr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gfefpbarc.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gotqzpcnh.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gmoyymkkd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gfijpdfis.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gfvagxtna.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/ggrafcckb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gtfviytrz.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gnddybjbp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gkxdiqbqh.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gixvgyptd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/ganvtbysa.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gtornmzbf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/ghnzzzczd.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gycwepdfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gtgkzjhob.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gsyjybboc.sHtML


<!-- 参考信息 -->