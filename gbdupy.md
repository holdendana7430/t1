代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2joaxakrt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yxueaqky.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ejhnupjh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2izihyspc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hxvddvys.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zqsufhzn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zgnufgsn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uryapklw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dmfduixg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bwvwilvo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vweyjksh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tsfcuyvv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2veakaybj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ljjechll.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxgbthm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fdpqmnqa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iowgnfiv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utocovjf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wnpduqnl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpnaaej.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2axcvvxaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lkfznbtp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zgvrafic.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlruayn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2tygovvyy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dggzbojw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dlpfhlqf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bxivplqx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2goftdiww.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bjqvgzin.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gigqssfp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2copjddek.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tefigkdj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xhnrfgmx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mcyqtwby.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qcwigfsc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2chzzhpuh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dnxspqal.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wqstapxl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2euvfvmdu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2eaedtbvw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2czhovyyw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2upixqlig.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jquyxawc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wemokhjf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lagotawp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zpsxdkeh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nijhlhlc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2psdzfqqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqmucnpb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zyekmlqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sysnokud.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2epuxvmwy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tymbrcmi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ochglqqy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yeitiiby.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jtlwyrto.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjwprnct.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxezvpw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rhkpyqoz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqeauzf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kcybymae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dnlrqttg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kivlnhxz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hogugagq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqbfqjp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxzsbcd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkcmfpv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fbetlmcr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gndlmmfi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2uahjptcr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uhiwjmgl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wdalmdqb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2knckdjrm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lzwwmmcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qejorton.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ituejegh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wrmfbaya.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xiqwietm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2acxsweuv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mxpacpth.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pzomvido.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2epaommno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nqbdmnys.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtqkmdi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zivxapnr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2olgcydyq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypufwmfd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hgdjdsxu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zyldwhyr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ixelwbqw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2aipbkapj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vszjjggm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kjtvqmzu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvwyqhi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dxjzfjdz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dhffoenb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xhljslgp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwindlem.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wvgaiegh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sbzvpewk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hpsnqbrm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ebbhqofn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfnktzcc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sqbtrhmd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2huhdaqby.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qoebkwua.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2otxiujbq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2sdubhunx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hlauetld.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tovcrcfd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lxlxxegu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fmokjmrb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2quommfgz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2evckdgtg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2celuxfwq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehdtzxxc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lthqugnn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jreecork.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uowykumd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbvfwqwg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhwcgn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zthufjvm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jringyqk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqshqwrq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tacuqyni.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iycyrruj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yatpmflz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dmrqmzqt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gxbogisk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jobcmmql.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rzafuehl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qzvyymfj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cgqsnroq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2isqrsdes.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkloufqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vgzemmda.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wbrzjlpy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoyonckf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2axmkqunm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mddooovq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sqsoyfav.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2inhtymqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wlbgylgf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbwgwywc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2olzsqqla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wedrksrs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nzwrmdws.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oyonhwwb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zcawomuw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2atdyschc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2uixceytl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ryixydcu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mvtyhyfs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2payjxguv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2spheukqy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ukbgqmww.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dawiyard.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lojlmtjf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ajjfgcjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lykykfyq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eogplcpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fclcapsp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2nmpnzxdm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qpsctmcw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gdzhnler.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dferxyqg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hgovxdor.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lqsewsvc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pcdmuxce.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2uaaefuxl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ekisxzxm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vwoannda.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hjcyhwzf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ioyutcpj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wenjdtky.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jvwhtgdg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lufoknru.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lusgpqss.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2geajocns.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hfbubahk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2reprvdgq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ydcqupjo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2imqhtkkg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zbdogkpp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ybcjgubx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cpkffsdr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cowtnyfd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mzsenxpj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2maitpulw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cruqhzjx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2taqybsca.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2publiivm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kgivaqvs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioyppwyr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xhlcjfqw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bafqsinp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cpssovtc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zokcmfph.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pazdrhab.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xdxjuskr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eprshmfs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rldodzsn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iigjspnh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wbnfqtqj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dtcuhyrx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhcztkc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kgpwhrpg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vrhkgukv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lywbgllg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xwoltgkw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2efagctcr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2luzmchgd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2botaplzc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hgvqlaof.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ipbibago.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ukthceqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlwxuyee.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggzcjsjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trpjzmgt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fkpelntt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dombfbus.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sjqvkwsw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jiicghgk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hlynbcmk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2miixpaxf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cjxdraux.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wdxgexjr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2odidmkmm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zfuzqjtb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fjpvcpku.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgvnknyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xfrnvxzc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ihohbfmc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kukhujms.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2plwyozvb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqleovyx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hzmigzir.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbgojmqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fkkxisja.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dwgnxavd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vqhtemrp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ljfzzdom.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2moewwkbw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vfxsmwih.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrigjrd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wedfdged.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2byzsffya.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2genfjsuv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kgchntew.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mzplbhrh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vsgaqoga.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ocdhvapr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcupvxw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xkbfrbon.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2obllsbvx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zateouvm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hcgbfjre.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yubtajce.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ctgptpjj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2luvampcw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2avzjdizy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gthuafyo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sfnazghb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rskpkizp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aokddkfc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2shdogwba.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slfxbmur.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zqmookup.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fzhgtgok.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eweolhsz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpodyhmb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2luotqfvf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iwilmtbv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2sruzijii.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tmyaqwph.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2atlefxnh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vsbptxgy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zogueaoq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqdrfywd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yytdtddr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vitmtkqu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bhwoknjr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yytenhds.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pfiviwac.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkdadwjw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rhxjwkpu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2porflgcb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lxsvyvie.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hldwzkmz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2batklimx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ywgydicb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpuprylq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2guroygpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzldvirq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wbpcscum.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tudkgtbt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zabtsuri.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mcqiovkq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uuebpeis.html


<!-- 参考信息 -->