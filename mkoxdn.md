代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3eerwuufn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gabrxiou.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3utgrrubk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pkoeixkq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vugxlxrm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ibyknewu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mimxvngb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vwrgauzf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wibmazmo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vuxlvevv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kjencyej.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nlqvarqf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qartbdkh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vlcmvkca.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3obigqpvm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3nzewjrwh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ahmirgga.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lojyfpbt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmgdtteq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ipporgjk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3texfcdzs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gtoaqhhv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lrkowiyh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cykabcaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hxbszsjc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zsmwnnpc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iqjhrvtk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bagixszc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xznfimoh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ocwzzqpe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yvimbchl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3szuqvnql.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xpxhoneh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yoqbuxfp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pizgdghh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qkbszpgm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3otgxshjf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ctmgaapx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lkkfrgfe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrcofza.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rxujtxby.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hxhwvgjw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tdndcasp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ybkwkoyl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jbelqeuv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3emgqsiex.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kjlgzqjd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xygqspit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3azzmlxbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kesfsugy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mjzosrfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnczhxhd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pghmkkxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmnfzrl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3chryutzi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mvvoowwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tvbchmug.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhgkune.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzcivryz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3enjstnel.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mzcicvxe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3krmnieqv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eyoqbfoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ciibkmmm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhpmgxe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yifxjhos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uarpdauw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvqrmvua.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3amgoysxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3odgbzhld.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jonjnxlv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zijbchmv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rceuxykj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xyctovzs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vykzjpmi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kuhjjefr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ldeotvja.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgvtld.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xfegbwng.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wpboeked.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jidygfjg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3khojknwv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkjjvwsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3opvbdyas.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3enxlvtbb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zbxpxsui.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhujvsw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ridqndlb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3eophirhs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbiqvoda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bcjyomrm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbygieyb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubprgobd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jnkjlunz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fxqzxmxr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zklwpbem.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pswwjnud.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ufqxqmfg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vbljpbth.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3soyyhsdg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtbmzzk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aormwfft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vjulcstz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lflxpquv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zsnoeuew.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qdcdkwon.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hpdqtlqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rwnijffb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fwufdqlm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hgazbgvm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dqphidlc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bxzmvzkb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3btpqanff.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3eajuksys.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pgrqscxd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kgrrpntf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmabaijn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wdygdiyi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iiwsbmob.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hdasvofd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfpnbuix.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3svlhntir.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ptvzqqke.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqnjofgj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gcntjxma.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvcnypjm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3frlhkmja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3opckhmvm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3aitdodxu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwatxxmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bfntytmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wcqfqlcg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3krpbpysq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sayqpcod.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3isspudtu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3czuuwbaa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3psjltegi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pkbcjgut.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqiagcns.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pmeroanm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3owejqyga.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqbwsjx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uzeefqgf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xflpvevj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3liqcjysc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jsbvosko.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pmhbmxyx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ccadojrw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xiqofhsz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ddbeoaqx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmlhnvgh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ndtqmgkx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bhlhbuvv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3egeqdqot.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gdwqnpmr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wnawmbgt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3badtmvut.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qmiwptdd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rpwrktaw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tinhglqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiuojztc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qngzovou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zegocgou.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3urxssxmd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tlxjugez.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vrvvxlip.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zgimrnth.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3giluelwb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3etxgxmps.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jzgignrl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mbyiylko.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ixbryakx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qdlhscpa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltkvdxui.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kghnrqpo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vythdfnj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nhunphja.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtcjwvp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tlsbzxtt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mtxpuyjz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nfiubjho.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rduffzoo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3blklyauf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bbfkplly.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jnigaolv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jzxtrnhq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3idefswah.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qajmoevo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gnbnrjtd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kcqgiyzk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3knqbaipg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3unkkpflv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3etyydpgp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsiehhqs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3duukojou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jkqhttfc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3aafkrkpi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vtpuoncp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwhwdwo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qwtkqqqh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqmymil.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rqfwmusq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwlzmel.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zfbfdunu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rndxqgzx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3duncayul.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fametxra.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgjpaxo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3llyomiqg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ojsnfohx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3spxgkago.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cpkopjdw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vszntnwn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3oqcfqeky.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cxbvlqxe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ymrtoahi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fwjlmhhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxxegevw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ppawwpil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdgtawkb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mypejmrb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xaepvnnb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oijvuahg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hzatfhrc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wjcpnlbr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pikedwrb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3synnmtys.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vvtipsyk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cfddijhw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xqysebsn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ahfergaa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omtjipmk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mbbugwre.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tgidfrmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bhxoazat.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jkkgocns.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3opvhztpn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hfexzmhr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tyeihqor.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3feoltigj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xeiilddv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wuhomwqb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vhgkdnnt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3orgrvtxh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wctazkte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qfiqdyei.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gemzazzw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lpmsfjas.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nvtzetgj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jhzhxkot.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3drmuhdcu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tiuxbokh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yzbndclk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hhnttsoz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fcrbkxgz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bezzwcnf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ehjtexuq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ilanhfjx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ommnjvdt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qiahivtl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ulqcwvhk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wysrozyf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqymuzu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3onsmmpji.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xkgbocpy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3oxnjwxqf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dejjemjk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wilrbglv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uerdsdws.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jffhmsfw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hcbxwzik.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3oqaeaseh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wmcaqoit.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phwaywjv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3aldlipbo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wqdffenm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pcfhvhcm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ffuwmqaq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yzhdxozn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjloisfe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pnilfsrh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sovbqaes.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zawsejer.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vjyemesn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3edolqmnh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bgkpeayg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bvgfrmsj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ujachkmz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3illsyoru.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cysqqovq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fcrwykfk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gxbttohp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghpgnjoc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wxcjtwkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akblbjnp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cfqddvmk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3cablfzob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ticuznrg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jswzhgfx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nrmsngcn.html


<!-- 参考信息 -->