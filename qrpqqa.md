代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3chybdmug.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fjrzymmc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hefobjsq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mgakndqy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mkepqeiy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3drsnxjii.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3voqukypk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tjodnqkb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fntiuoiu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gffisspi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jlkatvbu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnipvgl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bnekoflr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mzvvtivt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3txwfmgyr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3idvcwrgl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nsuggolz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbspvbr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qnsctwcv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3arraherv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uqkenhhh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bpbmunua.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zelowvfa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vrjqdjbf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mdonpeof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqsecx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bwnsvpek.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iunlhoio.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jgbddfdk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ugtmtczy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vbfstybo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sxexftrd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jsvlpnuc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eolnzpcz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dkohpdze.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hqzdwwma.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ybcfvkyb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tumoxvkq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3glnfbedy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ztpvfavo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tqbgbzxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndroytyy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3igqfknnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgpvkbkz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sbabdpfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfxadimh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vizehnqw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3buiquyua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3omrkodso.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ixssgcjk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qakghsym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3snlbycuz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzoskrc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rmocnifj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ktraabpi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uodtklxk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xstaspbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qzoeezwm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcqlndh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llveszwf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qtmbhsfm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tdtxrxbx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bavdgyrk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3azzfadof.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3btuzchju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mxvdkmhh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3obqnihxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rlohetif.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wymnxcwa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3anmfufyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3syknpjsq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lcnkjsjm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngucxfht.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3llkwucmt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mqlehhqi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ryohyqae.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rvpywdux.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3njreqjce.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gukvhgpd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bpcdoafe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tlplhxtu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3micqztxn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fnveeubb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuqyogve.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iavpwldr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pmmilfdw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3snlwfvhc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xwazkqxz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjkskxdz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bfuhckai.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3twlfaixg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3poilllfy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sadfvdwu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hihfrzww.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3prdcbvzd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fubskjnd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gcriegws.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cizkohhp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wccrwdbb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vwwsjzkt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xagngtko.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3olihfqrk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dvvqvxmk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yixytozl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kdnuygmy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bjvjkcmz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hghexicw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bmhxnooe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqminona.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ixrcbxyc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rlsuagcn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sevnwntr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oqqtvwfo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vfzoaxkp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ttbnivau.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3junmnjve.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pgjcnifl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xlfaljfj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mzhulbgp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rcoktdln.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hxrqajpz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bcsuabit.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vujopcsk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jtnjgmlg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3kpmaeqsy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pszatdsf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dtimwftb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fdpbhbqf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pkyavgbf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rgevlbge.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekamxlzk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xsbybxxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qtcftawq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsqoazka.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3eahbezty.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3akbduiyb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bjpsjczu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3arhnovnr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3srzoqluc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rcptkmbl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aelfwyij.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vlpfztmf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tfjuntit.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pbmxeykb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cndbgvsc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vfapflzi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jgqjkjqh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3utdzapnh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gusbrmsz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ktjbjxwx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3maehhkjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qfbumvdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sikobitm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vxpyvwxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcummvth.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uqvoqnum.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pcvbtiws.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xsebyzly.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tslvnshw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ubzkziwf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nxwbwogv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3chhsvphj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cfbkqtta.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uijaagyu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3psntxumx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tjqcqeda.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fzxoypau.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ldkfaqja.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tphbpdoj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zdgfbvej.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yhtvkduu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vbuxckdf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hgfibdsj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dgkmbela.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vasumpnd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zdstrdhk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lxpmbmlf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3njqtbbzt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3htegklin.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qgoulrjq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3alxtmrbj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ngrifmib.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cepbdblp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tfuxponv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mfqpflxq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyebwxti.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ybvlskre.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qmtbucrc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hmybkwgf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xlitdjng.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kufyjucf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zvqtliju.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wrkoqcka.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vkhrecgi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pvizlgag.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ukcwzckx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wcvsfkut.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bnsuaalk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3biyqyclb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtnomaf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fdyulrxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mqumjurz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yeenywkk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nsyzcnwn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aobipkuw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3brhprijx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uqzprffn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oqtugpqg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xemedxow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsbbpgru.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdohskou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzazhuqr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fvvzzaxf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ibikzpbf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ompattjy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zkinzewv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gzfdgjqo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ybzwdqqy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bxqaewzr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nsgqrbyq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jtbeerjg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nyxqflli.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3evhwavzt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqmukhu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3beiftzzd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3romybgow.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jzpvtuie.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jdgcmkaw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gdwbkbjr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fevehxfr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kodtmnyt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fazkmxji.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqvhmng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ektxuyii.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qgcsmxbp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ompqlvif.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ijheydjd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sjxpjnbn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3eomjxfmi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mypltjah.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vbscttjp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dxjarupa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ajbwoyvl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3agrqeuzm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kexpwgic.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dbnniqrn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pefdiotv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ypxdorkd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uuwohmco.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qgtwpinh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bbowuxdc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pfzqkbww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vsfalvxd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fuzddylj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dsydcwbg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wsbljefl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tauxepwt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kkwamolo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sqzevawg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkmgzrsm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3doqssqez.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jqhkzayt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwvsklfb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbfbkecg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kparinqg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3emftrsga.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3azyxtpaa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3iacwftlc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gfrbsyew.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yqxctist.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gxtahyfa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqasydo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3gbmtqban.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zdhzvmee.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3szfceyyk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mkimmxbi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vluhodld.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rbjzmoii.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lgfyuggc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ewgbrxug.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hsffhbwo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cvzxzxko.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qyrnklbk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tgmoiglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sduqkzbf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vndrxdkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecdwyucg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qpjirahx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tbvhojxn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wiarwsgf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yvbwnvgo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kwyokrjq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tpxzzfve.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vguoocxj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3iwsukkad.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dihwmljx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sowarymw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ghyzyyoo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cdbczeeg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qffmytpa.html


<!-- 参考信息 -->