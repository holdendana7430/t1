代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2quxegqki.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2iiyiosav.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2keqqcrai.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jxewtfxg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nxdbzdeq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rtsyjnpo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvwlthr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxprqwek.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sbriwuog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2unfxsech.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2svhgdnlx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mynqeqav.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cigrykkk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gplrusok.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2klxhjsds.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zxbhzhhl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ktifswxj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2goiocxox.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2spjgwvde.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bwefhscf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nyprakdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2exkyozxa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gftbanxu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2weijotgk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hdrtqxpc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zfsmtxcy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gqnugudr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2droixsif.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dkssehde.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hdkvxgyu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ilkeddjv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ewkxuumv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tqpydyas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2iecunfum.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2umxgzpqq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2voahyuqz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hoirjgqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xofsvvzp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ixyoegkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcpmqktx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wgivyytq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2esxexlra.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nutospia.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jxizajnu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wvavqsdb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2csfrjkta.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfuutipi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ozyyxumt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhfwrpi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zodzbpby.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vpvcqnpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2enuwbtbw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jnjekaur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsygxzl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sopybsoq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyflzov.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dazdirvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2atimenot.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iygpucmo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lkvelqoc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2azgbvjva.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zboaxrgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2prrpsjlg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yyifbfsu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qtgdnbej.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uecqdvtk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ekppotzx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2faqpexuj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2riuubnqt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzaeknv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ulykqvdu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fyupebcv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xhlypppk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rtvhnivy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hfmispis.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2asnweord.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qpywqfqp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2etdlyyxq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kjrjekgx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xdajckvb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvofxwr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ktitpqnd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2saibgvha.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ybcyfklm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvroxuum.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qgyucgmh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2evprankn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ocwqonjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sbhctplx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mkmilend.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2apjgjtmy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2myoiumir.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uxcgevuv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2elnsigpu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zgqcmezk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rpvgmwvq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uzficiku.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lczrrzkq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lgrctmiz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ouxtrtqo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qghrgjer.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bugftgwc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oqkkckoo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2whfccodt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxxehma.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qqpkhzzu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yytrealo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pptrbzdt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xgvwnrvj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mnwxzeih.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qlsbimqk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvbkvtvc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2muzvhpmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zplnucih.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zmgkdplj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2scyccqpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bmmhvgar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2slofuutt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2virvlzjt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2warexndm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ggrrtdct.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2utffdomg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jkxaliaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ysubvpes.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wzqunetg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2awrddfte.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2onkprfwg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nnqwxvjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jfgdbpij.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kymnllyg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2snavuvme.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hpbisxbe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2txsoskso.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nkdmfltt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2okwsufbh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dotugxqz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfzmmqpv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kifspuwu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2itkxjhhh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rlcgmcqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vzfgvidu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nsnklqxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cygqpufs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ykzjnqbm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2badsbzhn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmlljhf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yfqanhhd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bdlicdzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vudrnwqc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ruqbmcoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihcvjhiy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ierovjig.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rjuybuvq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgnzbbwi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dxrcsoqy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jxnokwke.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sqrjgbed.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oiephodj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pymxnazn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mktdhbrc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2quwvlnnq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bjheomzx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bbpgplkh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hvpcwiop.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bpnbeuyy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjsqpv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gzvsejbt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nfekoynl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kdjzsiaa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ioulmgde.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zsurzzfj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2btrepnnz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iaxocolu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jrtlsrsr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idksewmw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2murxkzst.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dwnxplde.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhlcyhwb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ftitcqru.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zwpftfbd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tihmgcqr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nlwqngwe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izshxjxo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2onpshlne.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qvqettko.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wqdxnvie.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsoyrcnn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cdatywea.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2udzsrztw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2myirlomh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnmvwho.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfdjljw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wxvtsxkv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tdsnxxqw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tkotnjuy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xsudpgjg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tznjcikv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zhsciqvt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2gftsdjun.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2urvfcfny.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ijbcojqo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2igzzpsdr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yzgxobyf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cyjbvjif.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rsntvmjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gidjigvd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhdrmxwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwvircnr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2brwffyjz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2apevmkqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zazydsnl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rtghxfia.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2phjvqnlt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cjxcjihz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2heacltaf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hqujbfqu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2grsyoesq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2miiwcewv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vvpjiqww.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kolzeirz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lxbihawy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ioewsjir.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dktgmamw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tfprynmy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hdwpxrya.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ahhzsjlx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ykoppawr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2stvommys.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2lmddlpxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jmtgznsr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrsemtsq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nalbaoxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gmgmetpq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wuftrzgl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lhjjyffy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kywpbuma.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2apfcrapo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eoavnujt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fguomynv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jxfuumrj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wqbpvrjr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mzappfve.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2suyuwxbo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ystwemqr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wkhpcuxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rhypddnl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zeylzmtp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kkzjsaci.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ooglohfv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2buunfkot.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmurhtfx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2homebuqx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kshshhbf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mkxwtoyx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nkliijnj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmqsyo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jwfxkvgl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qotfpasu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvrmcvfe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ztqpwlui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ftcrqupd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2byxgonej.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xocheaui.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jhploiyw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixskfuta.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kxsidcyy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gfbxchnd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2knkkngkb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yhfvdxjc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ivkdaelq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kkbkjnir.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ummycpni.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ynqrkflh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dyjnoqhw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2oseczolr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvntqglm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ukfqnfdy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xynzjtlb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2teuvzxhb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pavgstid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdpznwcc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yythlstx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thywkymv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hgffbvni.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dbxfpjvj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2othokqcj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2orgrvddu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mouebkxe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vgmlhntj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nomtbmkq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cziepsrh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xtguekyc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ncqcooij.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rdnutpzx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pmcppssf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wczbzndg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rdgzjgvo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hrcuasdv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pugrcfbm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvlgtrml.html


<!-- 参考信息 -->