代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qpgocgvs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2itklddat.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ntgxzwmv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2oivlxxmw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uylipuoh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2snyvamgj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yjoncfrj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2drdfaziy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kgisjnda.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rpwlxxib.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2frcgwizt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uqfhajxi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ankbioub.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2noxlqzka.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yaudnnth.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zufwgowv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjwdsli.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dcdnimvl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kpbaokhu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgkhndq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lcudcvpg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dasjxcgc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmedswaf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gsrycisl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mujpwnps.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zwzofttr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yuaoltap.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2areosbxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yyqapeiv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qtqohfss.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2exqgzufd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2uxsvluao.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cqkpgywv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hgwinoxu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hsszcrfj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2czoolyiq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rkllrvyz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hlfjnwep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zihkiqhh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnltchh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uwmvztfr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rqifroja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bjrxmptq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pwrowoni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kowffzvm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2iyukxbns.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mmzkxjfm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2faxwbnql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uvsejfhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utazghtc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wjjhsvci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhiktoqq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ehfeeuxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rqpmxuse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eoqcpslv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jkhxfswu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjaronm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2giglbvwq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2drdsdpfb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fxgfhsrw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qteagmup.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ttqltqsd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ijgclgst.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2njxxvkph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jknamivh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wjkcbeuq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfmladq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxjcnwtn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gpslmcaz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zxaomhvz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2owbpxqgo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kchpbtcc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hqdbokmk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2amcvpjsi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sxorvnzc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fnumpsos.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2azopwpzp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zmfridpg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yhkpmurn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2egarlhdx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xulccpoh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfnfgkau.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nifrhexe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnwlehjs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2snplloax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkwswi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swpfcvtu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2euivxrcr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2irvsyqnr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2idlzyted.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2soycydkm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ihlajnox.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2umxtazrk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rypzcsrn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2efapxifx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2getpgjxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofpstpzr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwjsueoy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oukhwmva.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2afrfkytf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zksjwyul.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dzdpetxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ouqsilae.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2aeifufia.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tbqbrayx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pfibazlb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rctjypkl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rjxemssp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iyhpoukd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmpwlub.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bmocqcgm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2claptuzh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vqfqpsam.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xquxlnci.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lmhfawom.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kilnnhrc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uekuutff.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jjsposzy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zptfqjye.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jbdaiphn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bjjqhztt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgbcykqe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ctgqngal.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hvopqver.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ocihejzs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sixanvsk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bkpexjkq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdiupnmy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uflkixau.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2prrpbahv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hnpqdvsq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vjowvwwn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fzjnedvd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2trelwfkw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vcbrpjfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcwcvhqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kffikuyc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2voilxzzj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojsehlgo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xjlleeny.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kwikgrvk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2guhwxgwo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aoexupkz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qlznjuzr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ykkojudh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xmxvzoku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jtpflmfc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqwgpsrd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zltiarug.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2oxapnxpy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kltbkwld.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jbdulphz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ztwdxced.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zsoowrfi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mceauwti.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gjvlqpzv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hqyvtyrt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2omruogqy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qtzzovns.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qpbiezlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwiigxjb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kkevwphc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idgmikpe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zyszuybv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qcrsvqax.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ornrbxsf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jfszctft.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wuavdbul.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ocnimulo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fuwuwekr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmkdqla.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jonzjoju.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hjmqefen.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2eovamxfz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rprfgsml.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chzovsgd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2srmogprm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xrweaabr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zgwglkjd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rbefalhu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jyhhosya.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ulmeyzey.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bqfvfkpk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vgplyetu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hiutitjc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yyxiydwr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tiujpznw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mfwxagsz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dtwaxvth.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kikpmkqu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fjwssezc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fcryesqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ylaiotzw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ybysbgpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gccpudkz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2amgaxhhz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qzhfzcse.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2phvrdkqm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqggcec.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bavgforc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vujezahm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nwfnsrpb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpnzeha.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uuyfmfpz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kfpegbwd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dkusqbuq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2exgrgwkt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpousyfa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hguyqoxp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cljlevvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hnqwtqcs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yrtalvsl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2smnnytlq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2khtgizkm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lieenixf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hqfrwada.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gefftdet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hewjsyvm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2naqgauhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhaapzlw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iaydnlee.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xlnzweza.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tvepyike.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rqbcstyu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yhgynrqf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ktdirafy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kfwacwxi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2aamphbfz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mrbyuvzt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jtwtozjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2umvjteuz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xhlokzwv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mmscgxpa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qfvybisw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jockieus.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2acosstwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihoxzadc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2opetperr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2igqmcmze.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kgxgeorb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qvkkwsma.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qzazbjdp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mhqwacnm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtlttus.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2srtykxxb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2msjlifox.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2baccrtky.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jwhgekbu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zgqlffdn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eueyfxhe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ssluksmf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xsmztpxl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2urvruuki.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bddkgjyw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cuwnqbhc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yahfnckb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2awqschgu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2biuivdml.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qxrdyavr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jjkcdhpa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jkdpfttr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fkqalquo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yllobrcb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mxncavcg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2agebbdro.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2sxquhteh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qsrvhwux.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtqahkgi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bwwwqtdr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fgyrwxls.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hqgkumec.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sfmlxxkn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qvrkblny.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2sdslmqrf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hpmbgnfi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rqamiacr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gimtkpjq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2voufryym.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dpmjqahi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2klzgnbsb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pzlqitkg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2enzehhvt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oibqwzto.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hrqgqdxs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vdelpkrr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2icfssvze.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ufttxgnb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2htcwalso.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tafktpet.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lnyxiemq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bnqsdobw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tmtysmyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcssolmk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2adqfsgwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbkrhzhn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xbkzxrlj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2sduozikn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fxsukyoz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2krvydrmi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2imkcwvro.html


<!-- 参考信息 -->