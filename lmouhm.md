代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrsnwwm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esmiwgrf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oxnpwpco.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xygscexg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtrnthqw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wfnrzgdm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pttetpre.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmzviieu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bmodbslv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tvtlmvyu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wsilpgct.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nuziskrz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2guegaccw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fbkndiuz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2khzezsmv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dyissdub.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2llksafwr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hnqtwdml.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pxeshtji.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bnbgzlts.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qzjlhmlo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ydmyichy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ylqowfan.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gmnmuzio.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkgebl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hvxjpdfp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uqwgyewe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gdjrghjv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vubjfcqr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vosqjrng.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ctffnjsk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ezljodwz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2awhwsvoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnafroxp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jccsvqtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgtyhvku.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zstomuyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2doieubny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vqwmfyue.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2svfunxdg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pjjlvyee.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzfyvmpr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2noxxhvxs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ynadivrz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpeeqhtr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vkyekbmm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tubhjsqj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2byhjisfq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfwzjpt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bmrxfbwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrtthwr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhqyrnyd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xwhygcin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2elpwcods.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2axoyjjkr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ukylpczd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jkjqmhut.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ytrxizwy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uayzqzyw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vrjpwrdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2upilvdan.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ywxhmjbl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aotlwopf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2oysgegqx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2noggzwud.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqonskcz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eqzvzdqj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2akxtwmym.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebobvlcm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hzmkotax.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tbqwdjjg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpgkkfia.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2chzdlwsr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2crrumhqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bosvxgab.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yncpvutc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmrniscj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rdtqbmtw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zsxjgkje.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ccinrfcm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uvimvtwp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydujcbmz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eszcujkg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hucodamo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xylmhzpp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iaflflaj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2iruxxjkg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bjieygbj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fhpkrjyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jkccmudc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2izwmituw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xnwyyfic.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bbcsbytn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fufowlrw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uwfdlhgf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uewzcjwx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ucpdxdmy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ybxisfln.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dchrywce.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zqawddic.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzogmrcf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lgyvkbxn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wywthwpw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2grrkjoor.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgdximdi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oldlyxox.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uktmabjn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mcdybrjr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ikngdpkc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2onxxaysb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ewvfmkcl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwxesuec.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2upchbyyo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fvsbihhz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fnraeyfu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjenwpbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kjwsuukb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oxbrjeiv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2szrzuonh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ptnbcsik.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dhndsgpv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2otbgljhh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eidisjfc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ebmiftmc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2futpvmob.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mubqtavq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2spznfezm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2grnaxmfy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mkfzirwv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qwwbarat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rxefcrqw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zfeuzhdt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfjpmmll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hqebneee.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wimbxjmj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dwliaevd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vlscclpm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ptjcojzp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hmhcnfap.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bobbhamo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wihlzyrq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vyhspjil.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2frxjibkr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kxehyqpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmwplgdk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fkrwojdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okxwqxmv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kokejdbd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wvyurndc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2symyulkc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vmdxznav.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wnwgvath.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mgbpdxhj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ybhrxjiy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cllpmroo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2huygaryp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kyhtuvep.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2scyxmezs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hypywiek.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mfoaayjk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ozoutdxd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzopqat.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zjkhwbfw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2neqeqkjk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ndtxjqmh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pdafojnr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wnfqrbvx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2chwyiifs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fxlvvxob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tggnoxks.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnecxvxd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mkdgnzcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqpffka.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lsjtudew.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wosgfjdb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kwtanmeh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fdisjtcu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2njndxssg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pqvdjnry.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wbgnpfnt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kympdhiq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xdigpvfg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snyiunko.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aqbjolty.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxrngfl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hjugtuoz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ncpgwfyz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jmbdqmyf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zdsnjfjl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tdzbmsdf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xvdctmgo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnchvxog.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wgdlzbki.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2beptjhtq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ftmxvuiw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fsbvzopb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2deyzrmdf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sahjaiir.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zebythpf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bsrxbevc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2amuzbcdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvjkpijz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bopfvpnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipahzdea.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lsfufjxp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ojpwhago.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fbanfybc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wqazawam.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dsxooadn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xdqsuasp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mlnylyxj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qldacfed.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2yuzhqwqg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pkbqvtya.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rahkcywe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ddgywmyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hzqqmgoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ogfcnwhd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrfdmli.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ayengejy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zvqxthcg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hgbhnjuh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxucdtna.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ycqsoyws.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mwwnudin.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xwkegbit.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jbsnyhvc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2blbhyugu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mhkfniog.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2etcrvgbk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qbcuromh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2isplzrjn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jhlrrlog.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xmmznwuv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2szuyjkon.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2flxdzsvt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yasdeziv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhbawov.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2audvvqrw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rkpnsnmy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yfabamvg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fvlzxuvr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2avtxirvb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nppmmdju.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfjwdkg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nfoalvrw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rkccspnu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xojzkxbv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2emmrowot.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jkbymwal.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2goanwpqn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ndcgbjbo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jzuhzfbf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ubwoodmx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnffcpcm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jvxozere.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pxvcsoya.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okwvgkxd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2orqmxtat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2edgqjjju.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gswmqosv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2euloywau.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uupwskaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2phgsoyto.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2barevkha.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nkgmjzrz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tgpjqzbr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qlgwozht.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2diixkcpa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kaabptwa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2slqcvxtx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2omgfqrjs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jcrcxmkz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hpwcmexc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ckefhdau.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2haiqxugh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlwsekvo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qokraozi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apxuitor.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tdphsadn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cmqxoarv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gochhxjh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oggvvjrc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xeynaiam.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eqjybyiz.html

);
来源：http://www.52xcode.cn/Article/details/gt2asqfotfd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yeiopdtl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wwinvodh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dgflbnej.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ocrpzsaj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wmssoony.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xbvtffjt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ilcqnkse.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2buinwubq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2selyzmuj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2glwflwpb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2swjhzcck.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2znlsikxm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2apxmmaxh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2buxklxtb.html


<!-- 参考信息 -->