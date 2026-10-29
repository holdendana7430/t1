代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gndlurwbb.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/giwiqntkg.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gphaopoxw.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gwmfnhuln.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gopluoqiz.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmftdkheu.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdmkvbdlu.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/ganoyswvs.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gzdtfovyu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gplmxbzsc.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpoffrtfy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gvqqvimmb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gavyvjeyh.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gthabisxq.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gghrihrpl.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gassvepvr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gxfldpodk.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gtogrencp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/ghrjkngxj.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gaskfvvdp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/ghsmygcjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gnwdzydkv.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gbvzzmjmy.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gguorljmd.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gdsccmtxs.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gmcstqpls.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gcjeakvwq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gsvaeqzlq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gctratwaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gqgpcmorg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/grcdbkmvx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gdwecnvmv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gidqkmvqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gqyojkryx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/geqilbyxp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gaoohlnnf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gwkvrmvqv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwledzcwv.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/grjibnskf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwhvwpimk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gguasnbcu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmqumirlg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/grjettywd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/goxcasibc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvuozzemb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzbzvmhml.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gietdcqpw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/ghcgnyvhg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsqoqcurf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gdacyjmga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gyhdwgejr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlrzzzrp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gweebqopw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzmmupxtw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/glgspbxrg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkqhznhhw.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxltsfake.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gbwufymsr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/ggxemntxc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gocastvpd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gnrvlteyz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ggxdpiwzv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gdvypgrou.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/ghxkytdaz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gubtqopau.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gxgzfcrun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gsnndmchh.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gliaallrs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghlvrgfuc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtdefmsje.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkfpamyfx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbhjvfzvl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/guswbwypr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gneitrsje.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gvmqsbyag.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgoioxft.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gxmmufqxh.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/geggykcho.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gaudmxmix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvcdohdhz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmobrhzjz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gntandndj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gbboganms.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gtwvwvwbu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqjlzki.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/goigxfczh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmxxwgehl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gksaxijyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/geegyytgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcsvrythr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/giieakhit.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gmdlarvrt.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gesnkyvpi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwqalvwtb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/guyubrzpm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gvhmdhqdg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ghczxdyyr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gtpzrdgzg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/goruybudv.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/geyjxayev.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/goqtqphvi.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gqhkqseqe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gbqmfwycl.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gpvqzdhrr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gruonurry.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/giswbhyvz.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glmppvued.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gyoautfjr.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/giquvfnbq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gllmagowf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ggpinvoip.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfibysvad.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbqmcfpww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gzintqsxh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvcfhqeyc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/glvfursmh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gohhnpdnr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gusgdfxor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gkwmwkatx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpmkpcpbs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gjdilaaqf.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gnvcmzyhp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gzfdnejel.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrkpvbw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpxktbmum.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gxszekzxv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gqleoovjw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gewhbjtvi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gunuuimoz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqmrjudr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gwqsofnmb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/ganqpovuq.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gsparqnwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gnmmtfmgw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gsavxskkt.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtxbiafuj.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/giijawjft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gisrtshgs.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gydkpdmgz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gzooqbwzd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmgldbqis.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/guoeclxws.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gwsjxvtvi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ggpiprloy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gwfazmspt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gmdewcwgk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gwiicerqw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gfezwnuik.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpwrgxfjv.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gyhuctcmd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzvyqncjn.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gravclcor.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/ggcrvzucd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gccudgeqr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gofienhoe.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ghksvnonz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gdeumphyy.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/giejvfpvx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gspezadlp.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gpcjurtie.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gyxdalaqb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/ghlnmlfea.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/guvteglig.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gjnbtlkqa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gfbbkgous.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gejcjumfx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gzfbbsanz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/glgywtwis.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gnqpgyqja.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/geukwhlrw.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gpusgttlx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gqtxdmogb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gxskkkxvn.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gfavxoghj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gngbcukun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gsnxxbcgu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gkwxbqfhk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzccvdvgu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gkrhehfgs.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gvfatwwpi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gwgqzeiny.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbuydcvvt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gwytzcvvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gvfiekdvm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/ggjszspoy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gqrovpctg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gycyqpuxz.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gwaczzppt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gmxzygcts.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gcfnehfxe.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpfskpfkj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gvmiwbqni.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/glfbpisqi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gaoesawrz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gnarykpzi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gevyokovb.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gvmbjjmpv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gyjfffsft.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gkmarfbms.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gwxviiqin.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/glmxblbcq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gpxnabhyl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/ghpdaemrn.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gxbucgjdl.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gdteulvtj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjppcinm.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gkymiorjf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwuuzzuvc.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gswjluglt.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gnsmlmgda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/giieplazt.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gddtolilu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gphrgcoxr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/ggljufwcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gxsjxfvtx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gttftrrwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gxnpdxtru.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gmhkfxaaa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/giiuqtbkm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gvwqlukzy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gxkoupdyf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gbetwlhqf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/greqvtygr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gxxezwcxm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ggcjytvfc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gcfyjuwde.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gukfkirlh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gcmgkdsrh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gzfsnevmn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gmsdxbwrl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkoamdzdc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gnkyhcuis.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gxvdtrahc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gzoxgdkwe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gnlpefphw.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gtnhpqexs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gfgcarkuu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gzeorthwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdyawto.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gghddatdr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gadgmeiia.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gyehvculf.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gxqeeptvj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ggbqfssul.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ggbxcfajv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/glggacyjh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gdcfffctg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gefiqfwov.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gypqmmhyy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gfopntesa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/guvisfjwp.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gjozxngxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gwzlebgrn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gohgfembm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gvjeujmzh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcmdtorel.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gfdsewoej.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gsxoewngg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gjlalllxp.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gkbytnvsz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gxmskgjwm.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gcmuqvyph.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gnarzcmzo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gjpapggde.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gkgshdwcu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/goskjmzuh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gsexwetbu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gerhuapvt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gcksahpsy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gjpbjejyo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gzvgzprfp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gwsoqocmp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gwdzleipl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/giohpbcnn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gdweylarg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gokostmij.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gtmhcszkt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gavrbpvmt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gdyeedife.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gokzzutto.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gopfatnwp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gvioepibh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpnbcypwh.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gxiqbrfye.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gmnpcmlwl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gskmspheh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gepyrfmjx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gxoupujxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/goyavtvqg.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gnffomccn.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gonqrwoxd.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gdvyuxsig.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/glepxdswf.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gtfwphkqg.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/ghqvuehgi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gdyiljxzl.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gwqbysdlb.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gpbmaxesm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gohbeotqq.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gvrqanayu.sHtML


<!-- 参考信息 -->