代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gtyrpczta.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gcfucsfdh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxwwnrvsg.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gtcznqjqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gtaafirna.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/guxqmlliu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/guipfxsxt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gqyzgtrzg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gyyuwwmbo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gbtziopph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/ggirjqpyn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gavmxdhci.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gyqdwzauw.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqgmilceh.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gbfziojdn.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ghlrztomc.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gzbljjhtu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gifcovhni.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gtksbfxfe.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gbodwtwfm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gzieysyvo.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdgynyiai.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmfensfji.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmhbbldjv.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxxtwtgro.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcrfqif.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjckugtqb.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gtzoviept.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gbxhjzzuo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gwqedamhz.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gekibxikt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvyryxgcq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gyxhlcdna.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxxwkmvj.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gmexjuzql.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gqekpiyvr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/guclbucio.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/ghchpbnvu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gknzqbnpa.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gtgnxjcha.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/guqyvucri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/graztkzcu.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/goapaflnv.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqrbpevbb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gaihgpymz.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ghhddiorl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gbybxbkkg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmiishfcn.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gkbtvdjaw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gatrjeyzi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gvjgkfpdn.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gfyufffce.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gfdnpdfub.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gqlbktkcr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gmmlvilnt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gwtxnmrmc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/grdtlvxif.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gglfqtnhf.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gymwwjyla.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcqgxttdg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gocinecni.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/guvvyhddr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmwjeejnl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gkmhwqvzm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glyqltxoo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gskmscdil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guocuriev.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gwwwnktpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gonkwmlpy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gyghtfjss.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzmhztdpl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gqpfrvizv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdmlnipqq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwrjyaovn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gthduovwv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmwrztxti.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ggstziygc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gjzzyziti.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gesvdlujp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gmlntfzjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gwkdcnrsd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gsrfwbbnp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gncqounqf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gyrvswyay.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gttmfacmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gtptwbjnu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gaqpyrkyk.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/geifbyzco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ghjjunveu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gwcxnipkd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwwlvgypt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gukvsppwf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gizeyiqpn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gpckmnpkc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gteeypuug.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwnumzugk.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gsjwtucmu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gyjltbwms.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gzmoxbvsk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/guhriyjxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gwuxboxmq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjrixwbsk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gvucstvch.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gqvacvsts.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gqsrwyrxw.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ggbabhrrr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdmpxvq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/givxotafu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzghsozcl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpvckmppg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gcfwdhvul.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gvdfhgqlm.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gfwfvowzo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/godzkurix.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gvrwqvqqy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gsvthzyqp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gkvrkdlwt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gwcpsiemk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gfzhwfhwd.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gwaezsnpb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gxtzalyuj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gjfnxulpq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gfftcxxdv.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/giejkdjuc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gddxejnwk.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gbgobqcfy.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkmkvehnd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gssywrnby.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghahghbrm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwanpiogs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glqmcqxog.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gycsyzcoo.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gfocrrlaz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbgrrmwqi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gimzhykyi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gcdwhxhjv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gpryrvzqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/guidijtul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gplqagpvu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gbshnygrr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gckajcbmb.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gbdejfhkt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gpnakcpzy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxtucrfga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gamvvdprv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gwbyobqny.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gpxgdvegv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/getcrirop.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gtveicoql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gwhkggxgx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/geqsrjdya.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/ghknqgwtx.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gypnsrhng.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gxjyqvxjh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gthuwofqt.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gcremjafy.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnnekzxoh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gpvpmvttz.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gspgjaope.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/galprundh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gbhkarygt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gfblwcgqg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gxdkenmij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gdcjjnval.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/grizyispk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gmldsbqku.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/grbidegbb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gselaiktw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxddqtgcf.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gkhakhgrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvyqyzzvw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gsekarnps.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gelkjxtgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/glbbtqobg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gtveqeljm.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gkubastjt.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/geueslnec.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gdkdndwjf.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gyvyhawyf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gtsuryupq.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/grljzojsi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gmmslggrj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/grdzookzg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gtixjjxlj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqkctagvc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjzpzucwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gmjyzdupu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gehqmjdbq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gtjwqekze.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gnxcrnrse.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/grtzswfdr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gkxdhuxma.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gccnrrtis.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gvovnymik.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gadydyewi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gdnzwrgxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gzfnlsjsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlovjjvh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjqloghry.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ggtlrrxvk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gigselazv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gkeuomdah.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/glcetzfok.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gekuhsrxh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gkttmjobf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gssdnixad.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhrqbgen.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/glvhatsyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gbpoqbsfy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gzjqddmeq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/giqpolmwm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/glcrpkkap.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gecqaizfb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gqmddkuvx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/goavrmivr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/giyijmccu.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gvzxypdgu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqopuanvg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gftpsyrhv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gzdzhocwl.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gavbbizvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gzgqkrmnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gbfywoybp.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gjltpznsr.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gfmdgkona.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gftfojzug.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gkncghtim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcwjhptba.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gryrzoune.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gqrjbyxdq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gcnczaxfh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxdlygxqr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gkijmjffd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/geizlzkwh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/giiaemnbx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gmjkcirpm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmhnwibxe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gnwkeiwgc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gplsgqgsm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gedunszub.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gyddeewwj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gewekcxyq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gzzipncvn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gujvnwlcc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gctunksjl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gdyzcvjff.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gejhqvdwa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gikzhhrug.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ghvrfezfr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/glfhxemba.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/glkosqszb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/grpwejsmj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gmfsbmrkt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gjnyvxaqq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gquueestt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/ghteyknea.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gkidsccgu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gmbbcdxqn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/galzmzjla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqahkibwl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gbjiqmajw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gskpczhen.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gdmduqxsu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gjheuvyou.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gzupolxfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtrhyakzv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gjjvxtyib.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gsswxklqu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gruvbylck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gfvppdrfp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/grkhftvvd.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gyabkgtbx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gszufyyhi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gqxxjnqnf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/goqaqhtmf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gxebigtsu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/goaklpgqu.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/ghluchlcs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/guopwscdw.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gjijvcbps.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gqhslzadt.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gxdmvtryz.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gaojslziq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gsukirayj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gicodkfeq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzdvtklyf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ggwuxurmy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gabyxzvhy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gfbsduysb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gjgtwxjsv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gfsmokmzb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gwquvvtne.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gmgaiumfp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gmhsmvnar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkhjyquze.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvffshjup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gyvylxkjb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gemmxrtoc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gncuqkyvo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gsnhloqqv.sHtML


<!-- 参考信息 -->