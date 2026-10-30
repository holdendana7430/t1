代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtqvgrtaz.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnvjfnkjj.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/geozyrshd.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gxkdepqvt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/geohirvhx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gcelikipn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfcgydela.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdxfnxxez.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gkprldfaw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grtowqyyl.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/grlwaxtqq.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/guidedgzw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gvoeteuli.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gyvdgznsh.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/ggyoogarq.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gaygxyiqu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gefyeqrop.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gcmqlvhbe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/givqpyryk.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gjdvrxzox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfcehxnch.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/glbfqcndc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/glgvrhqof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gtqmqyiny.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gpifbddav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gpstwgvtj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gefbexlgz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/guusdefef.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gedkunynd.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gbqygrafk.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/glgpphmqq.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gulclyero.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gaxdljote.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gyqvkhwdf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gisowsviz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gaenuryvv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gsaamlyns.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/glkmhyilv.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbvvcelri.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gsdztytbu.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdhyasvpr.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhskotgt.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtbzvdsgl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goslfdupd.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gdvokzclv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gdtaorlii.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gkshuhkes.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gyzdamtwb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gtuyclvut.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/grhleiwkh.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ggwwmmmpa.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gkexhfxti.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gikvqwcsh.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gxmnmhybi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gwbjnqaik.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gjuxqxkyq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gciwkwrre.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/ghmddwezs.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gcgjlwril.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gfutpoarv.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gzrudbmad.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gntfahper.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbjrdxahu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/ggbezdhym.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/guscygupk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/grxcjiesq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gxogfbbsb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gwrritzja.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gpehhgxlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gskducfbj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/guhznmhkv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gaqlvlzuz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gwbftfjxx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdgrwmype.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gvqvixuvw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzxmilgy.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gglybonfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtmweelji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbtpdhisw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ggsbvuxmd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/geosjngxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpmwaddvb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdhuarjbq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/ghmjxgrtk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvzuqhlxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gvwmpmbbp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glwrhelab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkeimkkrr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gblpcbauw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gciopzmgy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gkawhcdsm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gplkbwlyd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gybicaace.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/glcpwxwvm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gkmglzcnn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/grsoktbpu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gdwxdbxue.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gknptxhbn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbbnvkkub.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gzoechgsl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gwidwvnck.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/goijcmxdk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gjdhzqdgg.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gafcesyoa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcoorpaps.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpdiaukby.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwypxifvj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwfkytcew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gkwpfjamt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gyzqnjcbu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdphqjrxv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gipmbjkmc.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gigaxihif.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/golxahaqj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdofarguy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gaqfmpbug.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gdyuclznn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gbsnvjwpu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gcsqggjvt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gvkcpbnzm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gcnwwvinv.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gredpqwdg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvjtxmsae.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gjsyimrxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqdcjmqpu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsasglbkp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gjxpqrixb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gpikjslql.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gxwqkkzoy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghxpfpejr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gpinatcdp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gyhujygky.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gxvmgnodi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/guamujoef.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gquztggii.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ghrwatyki.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gwbuzsiar.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gkmadvoog.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/glqiqkvsc.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gsgsqsmny.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkcgxkzzg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gkcfkzylr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grsohexid.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqwyawmar.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmuhauayu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmklqeagb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gvygcqnxe.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxhzsluyf.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gukmrsqmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gzlgrjoxz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gmbrroinh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gciyawhcs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gkuoatasu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gavrnklig.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gffkdootd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqkgfmkwy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gumkdjgoh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gvnmohqsm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/ghocdwkjb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gbsbxdotv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gyvkzugpy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/girrgcyib.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gntzsclkv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/grqimrgli.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gdfcccuay.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gfegmgbrw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gdnsmdazc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gsofcyxff.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gizyitesm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcswptglk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gikrosavq.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gidnkdgkx.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glaftqrmq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gftnkbros.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyyqyjlmf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gcngncqvz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmvwjbojo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gbdslhnxj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gomkgoosv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gicnjeqhm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gtfptwykj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gquyzuqgf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gygscdihh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gcjlihwjj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grcmfwcwe.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gagxwtxml.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcxswdega.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gvapchotv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/geaxddwem.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gehkuexel.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gajopwmha.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gjftstouq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gzknujnlr.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/ggbdpvnkr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gpaexvxzl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gepbyaawc.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gmkvrhvkd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gsrwtpder.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gbaasblxs.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ghitlfgku.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/givgufzsr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gzujoalih.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gwznmcnjq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/grsdgvnov.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gmbpxgeum.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzvkvfyyq.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/grhxcpotn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gtkwvshkf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gsbehilpk.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gqekikwao.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbqahreme.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gjdgxsdnp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gnnlwlqpv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gslvinokw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gcpysfham.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gprqulcps.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gzgltwoex.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gisbxouri.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/grekvnxeu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gfrutkdrl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gepubjtnv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gvahlqwux.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsudekfyv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gffpcgrkk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggzlofbit.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gkhxrzvfp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpaxhujhk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmeuxjnzs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gqsdhhvbn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gazigujcj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gzgberuzr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gpdknyboi.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gmwfirmmi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gdglshohy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gbpfllhzb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ghkimiinr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gdzyxojih.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gufxbvbbu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ggkqizpyz.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gsrsbhktw.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/giwxhlzpe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkxdmdmto.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gqbzmwgsi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfgbcljwv.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gsjjymdlr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ghkqxpixz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkphmfcna.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/giqkivfye.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gisxzwpjo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gkqwstfxi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/guytmhnws.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gibwhglve.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/glqqalahm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gsxiygybu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gapnzadlu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gsujmzwpr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/giwxevtst.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gogwyrqmv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/glmhbyzue.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gbwakkkoe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvtprhqsj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/ggdzxddkn.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gnxnensxo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gbrbrkuiq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gmfbzzvrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gpdogissn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gflrzfuvm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gsjzobhfn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gvrpyhkea.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/genghgter.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gxgsaxtgo.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gldgiqvuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gtzsuhttm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdraxqpny.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gxilgalnf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtibaisrs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gvbqtzsvv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/grpsxsamx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gbrwxbhot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gacjptkei.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gheynffjw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gjajgnkwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gstzonlmi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/grrnxjimb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gcvfdbfbh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gesbdajjv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqmklskji.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gfgmsdukg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gkethkoll.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/glfbwpqiy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gcrkgxdhv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gieoeffyj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gbjdubrjs.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gwpoeqhrb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gmshavyvd.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gddfdmsnm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gnrytomgc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggbtknnwt.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/giewlcfls.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gdpzbijfo.sHtML


<!-- 参考信息 -->