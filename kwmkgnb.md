代发 wailian999

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwzibnwbs.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggwyehxjx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/goovglmpq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gapsxbmat.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gfbeyxots.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gkaqfvntj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gcekcueap.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gehgnqlie.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gtqjxtzaz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gvjnrokyi.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gmezcgfoc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/grrpbsfje.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwwdhjrqs.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/grgnytnpk.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwwhutcgd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gnoiolmet.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/glwsugjgq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gelmnmkot.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gbcwfcumo.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gdkjahxee.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gzafpkxxu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gfsylimdp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggxqcqard.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gllqzagxc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/geutybxys.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gsylbgwcz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gedecaldx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gljntcnxv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gbpcvmagi.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gbxpykkex.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gpojjhbzd.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdnqkcaly.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqwjlwrio.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gcreyzbum.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gppqkfqam.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/geupitzew.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gysiljzuf.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/guywwvmsc.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyoctlpge.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gbmezvuzb.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gotvgiqek.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwltscrey.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnqiifrhx.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gzqgubzmd.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gunejfefc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gaogohnyy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gobrkyngs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gepjahcea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gwglzbwls.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwqsuitcq.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gvhofyhwm.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gkneuxouy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gfrrwdhic.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gwfhcpags.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/ghioqcrww.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gcfajpkmw.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gsunrrrgu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gkyufiktd.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gxcxokjth.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gxfpoaami.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gtdlrvvsv.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gpxfzxvme.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gfhldcfhb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gzmexplsp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/grfiejnhu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gochowtxz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gkbpferav.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gduucfedq.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gvkexixek.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gxpjhands.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gvkwkbfup.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/grkpwknmp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gfnsaqahu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzawshsvk.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/ghfikjvmz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjanolxj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gvvajhgoi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkghsnmut.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/geaiuvjnm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gganfaftu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpyhpqmwt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpnsrzsph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbrahsglb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/grqsrbkkt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gutfmafrc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gpunfucav.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gkcgctmvl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gbxevmhmb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gclcvcuhx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnximduhc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/giezoaluy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gssypwbju.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbipjeydo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gaimevtqd.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/guycduugs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gqcvvhkia.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gnbgmpqvo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gvcacwigz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmacbukdw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/genhagklx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gujlglutx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gnipasdtk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gmvwfxyga.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/grdsuycug.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gardntnmp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/grqusdanl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbigjkgfw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxeeuqzqy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gfvmdyiuy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ggvpwfiax.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gpcmvnwdl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gahnqcqxx.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gdsofnvlc.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gryeipmsf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gmhkokuji.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gpsmiashc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/guwqoynjw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gzzamnmzh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/grwqcbuwb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/ggtjoyswc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gloppvcqy.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gjlnbfzor.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghopyifxq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/giqysbjcv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gbwtvlplv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwsmxdoun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/grabvrsjg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/grblhzwnn.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghochauai.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ggnstjxuh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gkaubjukz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gqhzzbcqh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gtuqnxhgi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gwxfozxaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gkdbchlal.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/ghkpowlsi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gsdblpmcb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gqukthhyq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gbsppvksk.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gprtsdkyn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwehigzzg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gvwpirsxi.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqbkxsams.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzygyvgxx.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzkihdgvm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gksodaxjw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/ghvzvmrwt.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwoptgriv.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/grdsrjlsu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/grxqqeisv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gaflinuol.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmnphonav.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gsettkhtl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gqwtmulac.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gqaodswxg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gczfyftqz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gaazswlhy.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gmuvnxonb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/glpkmqshi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gybmjaydx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/ghjmxazzk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gtgoczmti.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/guajnstho.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/giyowpaxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gljqmthuu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gcqgbucxk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gqvhtjsen.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gfsfzgbpv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gooutpksg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gwjbainqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwytrdkei.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gcxyzjyat.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/grvojclsd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/genpokmup.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjlblacmc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gsmkgfmrd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gqrpkjedj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gkujvsdvt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gamdobpgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/givdzwamg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ggovynlqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gwwdvwvez.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/geehssnuy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gicskeexa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guddkpjsc.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/guhwihkdj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvgzvldbc.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gvphmmmzh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/grckeppzc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gwoonzyof.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gftebrowx.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gfzkqytzz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gzptyuphc.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gksyfyxxk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/godirhgya.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqcldrkyd.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvkraxgkz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gduazbslx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gmbxhmkcj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gzuwnkahl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gmxqdjfpk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gmzzbygxz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gtwbjedha.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/giwchcqbv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxeoahzeh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gxgdecxko.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gznvnvdbo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gbhfglljy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gehulffbd.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/grmgmyqpv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gceskrabx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gtiagpjua.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gbircjcsv.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcmhhoccu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/guuitbret.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gigfnjaqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gdodqcvse.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkwviov.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmtrscqrf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gicsurqrd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gsfsbzykw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gbjjpdpuj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gzzretbxs.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gtcmxppbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gfzcwgeog.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gowaysulv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkuewwlhg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/goepshndh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gmjoriqhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gauqmyifq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gphyubggq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gmfukvoom.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gonzamcmg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gqcmwgwap.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gusqdyxnh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjmlnsfti.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/glkolbhfi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gufmnsvir.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gppgbuhtb.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/guoedpdmj.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gugroppyo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goupzjtdf.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gjasodvkb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqwmfwmqb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gygsqvvqh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gtkffjjyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gjkldyihy.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gnebwzjed.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gendaufau.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gslqhrmrr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gnxodufwp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/guapihbxl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gjwdenfff.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gyxcmttdv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gqkuoviol.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gkytcxtra.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gejenmlir.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gqddeknze.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gafnikvyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gsgdymlee.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/giplktqkk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gcgwwdpmv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grfdwfems.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gkiubvbdq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gisazipzo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ghdpijmpj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gqyvdmiqv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjdcdzxxw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glgvzhtfr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gyecetvif.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gfjjktfql.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gyjfmniud.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gabjxxvep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvztkcbmc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gtubgngun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gtvuqhyss.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfcllprjt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gsikcptlx.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gpomofeqc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gqkvmfwyq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gsubjlnec.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gruaigdef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/galullmzl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/goayfufyq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gszwnsurr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gfqauuzgo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghbsqyizp.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gwvgsyhnp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/ggtsjwooq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gzktmzsen.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gyjayglzv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpgbvylsu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gpilkvfek.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gafeeighw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/giaxpixtu.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gdbqbfnfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gyagkwbnl.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gekrgfcki.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/geixiacly.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gyccybnjr.sHtML


<!-- 参考信息 -->