代发 wailian999

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/grgkufvwm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gidvqyeht.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtziqjzop.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gefeklkjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gsxsbjrfc.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggkxkwlgb.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gturontus.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gcexvxfbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gbfiasiug.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gywqzvyaf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gfeshtoyh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gormmbooz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gxvfqoptu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gbzymbvax.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gyvcjicsc.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnccjernd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/glvgbolwr.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/goftwtxjl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/grdyopylr.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gqtbdhzdi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gtjrvbzqf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gwmwnspec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gnqsfseem.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gtnhnhwno.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gfkghxsox.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gsalvepry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gbssrpecz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gghoitbly.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtpyermla.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxorlinkw.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gagaqvrqe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkcvdkcwe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gfvdyblzd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfjteelef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gcawvdudp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ghodppnbt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/geliqimtr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/goqycmqyg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guthsxhgj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqwnhzt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqqxjrjzc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gkyfuiioc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzqwmcnwr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gdceuzejh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ghutcpimd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpchgnuoy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gucvnxvxn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/ghhkizysn.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/ggalhzsdh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gnvtohihc.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gmonrshbl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/ghmqfgann.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gcdyedaqi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gokldjyia.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gmzkfxyiq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gbxmficyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/goegimruf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gzxgxepom.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gvpumuisr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gskqahfcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gmiamkqkq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdktxjyqk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxdorqfmk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gddoeduzv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gybhotdal.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gnroxjlfl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnnoiqyjp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gmzgeqxbb.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gzyshmajr.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/ghnmxorff.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/grwsvqrul.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gbctfhbpd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gbeuvtkmr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/ghfdblmoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/ggjdnodwi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gtwmumyrr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gjwtkkotp.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/goiomitfi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcfnfcwqq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ghxfhgkzv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdpcarztx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxexdilim.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/goohmumul.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gwzmercky.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gsbionwhk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gopypfeln.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gleyjydhg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gsmgndbnv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gkgzolpgw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gcbalgtef.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gvutxzlzs.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gjtqwnton.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gjoietucq.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gwjusydiq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gaguebnse.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gdoocjyla.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gcpbhdvjl.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gjmhpqdgx.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkpwgxhuq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdminbpwp.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gytsperid.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gkvzuxemx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gthrszhbh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggawbixqw.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gxgtwieqi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gtgfopssv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gjmgydclt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gadrhilzl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gwsszlbdu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gattusdql.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gzklfqsob.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxcofbwuv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gzdlqbjpb.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/grmqjmnch.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gssxpolnl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/grujkyrow.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/goecivhrh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gfqjjctxx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gbljdfcbk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gcpjlhafl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gfnodeift.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gbxauipoq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gzbcigzgb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gnyjtzpoc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gvcayxegq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gajnuenwa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gefdxturd.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gnarkkdlz.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzpqrvzqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gypxmxlnl.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/goynocjis.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gvytpqvwj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxmchhack.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gqyewcpvp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ggscjafwn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjqcbbtqz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gseatexxu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gsikqpjcs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gpqcilgtk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/grlprhvvk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsyqomdck.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gsupnxllr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmqiguzal.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gipnuzmqw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gkbtgtilj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gvpwheqzs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gqnfbcsir.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/glrigbnje.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gbismdeow.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gknwotfne.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gwutfngty.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gmubymmcf.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gwzzwkhkz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gudqwrpuq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gpzgxampi.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/goigptpkk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdbrxxnlc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gikyxdmcz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gwqupffqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gjxrigjly.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gxfbghuuc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gtwfvxjjf.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gictstrqm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gvnfwbbyx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gipxfxfze.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghgctsasl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gyqpuclyc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gdohtrsrq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gopzubkhy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gradkldqu.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gmhzvtlmj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gtroubbdl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gopwmigpz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gipuxxqez.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwxlmqwdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gfspujzuy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gcuzueqzd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gzxajsmrl.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gxkzmbjin.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gjdfnstqd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gzsrojnsw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gxiswbrms.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gfgoyabqo.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gsrdehspo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gdcuvazrd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gnmuibejs.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gunpnmneq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gjgahxqic.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ggwdxqdmm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gggjiukcj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/giutwtcyw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gebhucghk.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gyabjdycf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gjcaeeawy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gpxwgokxa.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gurhtgrbt.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gwdjrigwb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqvgjsqfk.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/glfztihah.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvbmdhnmw.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gbmxambtc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gphvnvtbl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gbhvwmrmx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gnhqfjpxm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gbkuztzfn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfxctyhju.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gbywzucde.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/garhijpvo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/geaxfpxvx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gxppmzqwq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gxtljgwub.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gutxezlkb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gtklprgbn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/goqlsxmtv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gdhqxvehd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gjowelymu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/guparsorn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gxjaqutcx.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/glsqofxfq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gqwckuihu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjirpnbf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gccipadjp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmuluairn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gqlxubxrq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gknfgvifg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gehhtdwfd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gaaclavzu.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gwyajmlba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gbljzcvpx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gexqorwiy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/grtovxplb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gigwaboyn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/ggpahvxai.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gnuyqrjyh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gdsaklbpd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gudtqcsvd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gtblaunel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gbnzgqhut.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gxvqnafhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gcfebisrt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/glnrnxkjm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gzizhzqzh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gfbdtrklz.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gnvvsbokv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gfagsgqbx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gfunfgzce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gednwuhsn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gpasgbtdh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ghoiqwtql.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gnbbwsdkq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gennawesl.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gscvwaqsb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gbcgwssmi.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ghbmjshnu.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gxdpcmmfn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ginkypdcm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkjkithnf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbuegoxqv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gxtbnfttx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gpeazgrxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gjuyryaec.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/guyasjajd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gnmqnndzl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gogqtgxgx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gqesqnmic.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/glelzbkgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gvpkcopry.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gdfjwzlpd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/ghoidqpul.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gvsfsbbwb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gfsbpetmb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gmavlrfnr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvvplcazg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gbszqcrxv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjtlrzslv.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gnkrrektv.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gdjvqafrm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gmnzkzxsw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gygvxjfbl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gjzkofgdx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gfxbdsdxy.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gpzbwtnbm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gyfvrakki.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gliqazofw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gnrarsdft.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gktpsvxfx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gmmpwacex.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gnsoehnop.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gzefvrbmq.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gjtqwhgyx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gtgkzrgip.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gvaxvhkld.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/ggmpefdrb.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gyewgrsel.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/giuyhkajs.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gxczzwmez.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gwatolwbb.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gmcmarsrn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdqdvefvh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gxysyqsux.sHtML


<!-- 参考信息 -->