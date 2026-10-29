代发 wailian999

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gvkynaehu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gunyvnogd.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gszylzxxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gjwsynwpo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gyymhqqyo.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gabgnkjfy.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gublsamma.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpcbybdim.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gzwljuqaz.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gnacclgby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/ggzxvmnfp.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gizrvifcs.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gnhmhhfku.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gsssgyyxx.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gkyeboyvu.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gzlmavhfb.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gwluwtvkj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gdzhyrmuf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/grzplbxwv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gteebzvrc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ggogltizu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gtbljkwxs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gwersfqrt.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gdbquldkt.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gupjqoyam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gwobyccvh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvemzstqm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gqtunuqgx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gwxtabcoo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gilftnhbl.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gdlsmdvgv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gturnykdf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gecszfrvc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkdvsxinp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfemvnrxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gfahnceql.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gfsxdaffs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsmpobbpe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfaoltdpp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/ghxhljoqh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggwcgflzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gspulrcch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmvnfinxy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/giryfiyzk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gfgjzkbcn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmredchhq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gttsoxjwa.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/goxsrjqfh.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/giprhaynt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gpdcoxysc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gmzpvimti.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/geeswjaav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/grauqqoxt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gqskjforv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gblgyitrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gxpgijlvl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/giwprteom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gxtrxdxaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gdqcqfejk.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gitlivnmm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gzxodzdxp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gigmvhmjf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbxohwitx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gotfpyewc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/geuimicij.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/grdrnpylk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gupgdmhrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpctuhkfn.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gauigtpdk.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gktngazig.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/geivhbuwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gqznetayg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/grxxrztol.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gjsexynhz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ggdbmjums.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwueeas.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gciwdfnts.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ganqdhyzz.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gbcxdczdz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gfgopzatw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwvnkpynh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grkbkdbpu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gmegxbpho.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gepywhnbg.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/ggtiisgay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gszscdvkd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gyvjizzry.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/ggihpralm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/grzkhrrfq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gqyaitfov.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/garzgftuw.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gnzkdoibp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/glxlglipd.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gfwvahjfl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/ghvahfgsq.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gcoqmowso.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/goceidkbf.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gvkmhzhda.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkgjnysmi.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gshvvhyfs.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyvxuozgo.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdbiuqvrc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/grlfsgyzb.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghjfsibtl.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gpheeembo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/ggsgdsdvz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdkrwbyqn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzvdjzpvv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/goxcayqng.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gegnkvwsh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmbyilhrk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gitslsnqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gdwmziztn.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/guldqzvcu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gkuyoxoqi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/ghfiwmbjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gictwllgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gwhstvkdt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gzwtddzlt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqwoleyyh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gsluuegpx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gokpztpsj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gukezylxw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gkalqmkon.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gczgazqzt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gaksenmvm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/goemowqwg.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvbcvudqv.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwuyrnzme.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/grpdewxpf.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdzrfvuvg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/grahwadxb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gjzngjnkr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gmjyhuyju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/grntaqzij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gwsqrmfds.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gcltmzsun.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gragcqodg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gynynivki.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gtqxutefl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotreyjps.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhljvwb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gedqtkdgo.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gkhjpkxgz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gpdostxks.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/glvujkibt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/glbxodudf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdrafmgje.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/glfnfoemm.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gycvcehfo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gpvszycyc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gvwqvvxge.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gfvqctyez.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gydtcalnp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/galktirtm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdkxifbnl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpviyxsle.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtchwvbgy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/goeekpllb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gwdzogbmr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/ggftvgibl.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gatrjcodk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/guoyvrmio.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gqxypianm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gtcltymar.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsvymbjso.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gghipvimg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/givqlycpq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/ggjfphbdl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gtmokjizl.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gtvtosexy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gsgypqyvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gtxfdcsbd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnkjovwvl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqpnolezu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gixpusirf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gonoewwob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gorgaqkjk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gemozjlmb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gwbmykwep.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gyimgdteo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ggateifrd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmdsbknbj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvwxmciky.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gigyozvma.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gaqdididt.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gmmsuzlvh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gykecgbfr.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gxgupiwqi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gqotxpbrx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gmwolxmyu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gwcvjvgiy.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ghhjnipoi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gkkngkwuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ghhhhqqvs.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gumkvpbvz.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gdagjmexe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gziakkchf.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzglbqrkw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giclnfzma.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gwdzcvsyr.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/ghisjjorx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gybbmvrcz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guvchqgox.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gaqpkyhnr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gntabsshe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gymfopyhe.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwjzmqbbr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/ggtwuhdac.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gxtchatvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gpyvvkyto.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gtygbxckg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gpymotieo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gqcziyipt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnkpjroep.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gdmodqdrv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gnljxifom.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/ghemvwxxo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gqmpvagkg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gfgqdprkh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gyqoabzxj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcshvvzes.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/guosivrkr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gjqljpqdp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gtjqzljhd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/glxnxmpdo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gocccobex.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/grijxzcfw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gjtccgcct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gulvhkfgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gxhfewwqf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gizpnhnqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gfwdecngt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gkdkfrtlg.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gelmmnxep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggfbohopf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gvcgktbyo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gzxgyvemy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gooaqzfpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gatxcsqtr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbtxsaych.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/geodykaus.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqxjmlfes.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/golwwvhhy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gcjuctmma.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/ggyczjqqn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gqjckvaeh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gwpywyelx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gztzvedxx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghavpihli.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghgxcgtvb.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gbuuebzgo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/guifvrdws.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmczofysj.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/grihmqsyn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gxzuoqpbv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gyqzoxprw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfdgeypiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gxlrsdsyc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzdckede.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gszbyvufx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gwxxhvpuw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gnedoiszo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gweukdozu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/ghntoghfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/grrfptiel.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gxhauaehl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gnikkajad.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gbxqkwteb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gkygslsax.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/glvyurezz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ghvhgrvjp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gywdcorsj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gzxjlqcwz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gftcxrobb.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gktdodvlx.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/goycattnr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtahppepg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghthobgou.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gpcobqhze.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gsjzfgcog.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gtomnfnum.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gsfmfvesn.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfxeooimk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gvbefxqno.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmokyszdh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gtjtnlzrw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gxklpnupm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gzjfreyjt.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gjhaavkzu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gpedeihqo.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gyaaujeht.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/ggdeoyvbb.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gfpoekviv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gkxbxuvxj.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gqdekihjv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gptbskpxd.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvbpaamhh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gmutpnmtl.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ginjibwjf.sHtML


<!-- 参考信息 -->