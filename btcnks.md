代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2exjvgnxb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2csvtfhwe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwgsdbup.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ikawopqd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hvktlbup.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qjwknrcv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jueiqjbs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wldagfrf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxdyfdb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jmroptmr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdcejki.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwdogkm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2odohmknl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wlygnpsd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pxlaozfp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hfifjefj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ncqjmgae.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2djqutlcl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2twrlunqx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2okfnlxwy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2itxpzvko.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dkeghupx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2keecfdgn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jhjnzjkw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ofadvcps.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ooybngle.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tbrnlapz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bkazmeuf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fdxdxhmz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qgnmljmz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2thamdkzs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ctfgkaga.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nlviqjtz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pgjencmn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vhresavp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tecdkwra.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ltqfmqqp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2btjecsxt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gyniuacm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wgtynhly.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2irsdauig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xipllhti.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2boxlhrns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clhnjpiq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pwmmtwrw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dwcedjfy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2remwgxlp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzlurvwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tiglpdwa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaiybds.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlevvoc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cvqzruji.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gkjgylvf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2muddjqyx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dyewnrog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fscdmsrv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xayahyho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ifkdoynn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hjcrrlku.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhdmhtq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kkrlovya.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lheashgi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rufcaiua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tgzlmvcn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2nijfiazb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qgfcmkug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jkuhcwgt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ufqiiehk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xqxnhsmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fpehvoxu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tjgtdxcn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wfxxkmff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ptjschct.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2umuzxgop.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2izhpzqcs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xpfksfqj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqpgkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytnxweeq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pncshszf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2samuicyf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dvipuckw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zjwecham.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2spsoadcs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wrsaiszq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkfizcv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ijhqqquv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wsgprzfl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jiuokwmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qtjvjhld.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpbkuqbe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2idexrvjk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zsfwcdug.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qncwnslk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nckhpupe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2lmflhyoy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hzgedowk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ntwjnilp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hrcwkmpz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2upkvtlhb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xkdzmplx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2csucpqip.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wimohrgp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dbuuezog.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xrxoefns.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2weuvlozp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vgkicywt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xzzqctsk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ydnaeixr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cwwlhxie.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2awnjzfuz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzrjnhen.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2onulbmuw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uanrxgxv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hplpmagg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wrvexsmc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqniedtq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2trlupepl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kednvank.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypphndlt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2woedxyka.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pytriccs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xvcaabaa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2yhpzavra.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tisteslw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrnbmcq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2euafqayo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2npxpaukf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qhycoxdz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fqtisupd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qpctiuvq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqlnvkkd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nezkwbsa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ufsonlys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2skxtyuvz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjuqnpqr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2annjdanw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rrgmkvrl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dhpkoxqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eaunjofw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oflwwyab.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zrlynnfy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ojpjqvuq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vdwkdeen.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lnhwgstf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cvyuuodl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zwsmzlhw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ldndaaph.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ntrrkzsg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tiwbfrbs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eevlxgha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nufrovhp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iqctwiiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfpwyoxm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wcgjjytr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvyigmvv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vjhdblbe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pjbbbwii.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rbucbhqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pljnwyal.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eiesaaod.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ohfcszxj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pckezvnb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ijmoqbyf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wdmqaqik.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mjhoteim.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2croadmaz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qsmyifmv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jpolzubc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qeunbqvr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rjppltgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ylyzjemu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vyjsxzxf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vgqzuvrz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uzjmpurn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dfoaqznm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qpxpxdkm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mswafswp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kebfbjyf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2stlnzbgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kevwwkvl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sxjxmiop.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2loctijik.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wxpeyjav.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ujztyncs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bivnejha.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chvdwnml.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cgkttdud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jmbiujkh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fonwnuaf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hvlynjes.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pbxqvpfx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kwsotvnu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2thylvrof.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zljirwbo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2glrrqusv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuelhbv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2uegbbvah.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cmjzpjfw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ravbrrxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfriyrei.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lpbvtdjh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zgbxrjiy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2encnjuqc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wmykwfzf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2swumutgy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ghanxjmm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bjkissqv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2obksghll.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ptsqunft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anjjyric.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptavcwnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efvrhrgd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dnycrksb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvjvji.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gohnamru.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yojyhrop.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tjtpooxy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2offiknrx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2euymjqaf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lhhxrgat.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2biagoedt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hfqdygkf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cupbkrwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2abjoxjsj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2udqjwyzt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cautjmbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vwufnroq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2evktpxmo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udurivlk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2scthpksa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mkmrpbxc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ezvjdsqi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xenbottn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2suiyohbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yckytyxp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjdkbuu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2laglqaii.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dfshcmij.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hcgjsdqi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzzpaasx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ergsrygz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jhfldnpf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dmebfvia.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lthfjizy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bhfuugtb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tsbenxnz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bglcfbym.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gubnzgvz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hvhojhhk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2koitbpuz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ntyufvdn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2sbdwwxfu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kvvtziky.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sjrldyil.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2muddvbyw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uxedybwi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yjuumjgl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bcpgxmdr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gxgisvhh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2izmssjrg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xrdjapxo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wwwibytx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyvfhoir.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffuojvre.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bohenwbw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ypikxpza.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cruvzhta.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jgqivslv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2utjnznwx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2onwggzpx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kagarryh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxreyaip.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ndymdvzq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ruqokaba.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qnbjnszk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zphvhwut.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qjezcrwp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wsoutnqx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xptsitwf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aajcoomi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rsgonpub.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2scczjqla.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cnkurleh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oevpuaob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmlwyjqz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2snchujpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evgzlsxt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bdetvdoc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pnuqbned.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2egefpqda.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kvubhmgt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hhmbgztu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2omvkdaar.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2woozanbq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tfxpzzkd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tofwjbuy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fydgfhlb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zgzutpwt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2auhrmepp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2psvngjyf.html


<!-- 参考信息 -->