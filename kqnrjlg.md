代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glzuxvyxe.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpqxyynkw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxwpuwkdt.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/giefmgbkh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gncljrbgw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/genvbwdtt.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gjqhlnuda.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gnscocswc.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gelenyznj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gduwhfrnh.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gvnjzmfek.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmndlypat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gldxoardv.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpjqrmpwt.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gplxhqaaz.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gnjoylkeu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gvplygqof.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gnypqkfdd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gageeutej.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/grirkdejp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gjecaegbu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gatwilbrb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gexfsuadu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtpzrnhay.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/guhlqbjyf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gincbasvr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/giofolrpv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/grfuutdsy.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gcoswttjo.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/ghdfiazhk.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/giyolaowi.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gynwwjeoq.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/guqrjydtg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gltrfgygx.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gpbfjbiul.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/glzmlyeow.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbttefr.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gmjtqzhpc.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gynkrjonn.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtxpisvl.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/geglnfxgz.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gwkhwycgz.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbrpmmvkr.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gesyizbzw.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/glrtigwhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gvwqcitax.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gwrrwaotu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/grbpocvou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gphzomqbc.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gddbsxuji.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtvmpfwvf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gyxxbcwqq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gsognsyva.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfckmpvj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gutfuicmm.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gsykpaieg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gpkxunhpw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gkbyiudxy.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmirtvvmt.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/grapnjwpu.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzivzqyn.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ghtotzkhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gefwemyac.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/ghfallpje.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gulalqtmx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gnquklccy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gfkwhsloc.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gekyywoth.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gbwykxcek.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/ggvouezkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gwcljumie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ggjvziioz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/ggemsplhy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gezhbpfge.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gqmdpirie.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/girlyemcq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/guzdqmoxc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvsdlusbz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gazjswjfn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gztjaflnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ghqksytom.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggjeqanyf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpbkexykn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gxfwybixn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gnvkmcnsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gdtrvdmop.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/giakjjzbs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gwskhtefq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gqmoqjjej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gylmubuxt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/guwbfptin.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gmozakjjk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gmrxunolg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gtlwsakjw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gcgyuotdl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gtzlhbfcg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/groavvkoh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gjqturpvr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gropspnsl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gmswfeufr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gvcdperqj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gtxnkoxrm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gnqgfifvb.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gccmwsimi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gdkkojhsp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gammdcwqr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzsesxwhi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gksffirwi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfxjsfzrx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gldgqywgl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/guzjanwuj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/guuyvoarg.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gdhzejplz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbtpfcahv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gciwhgfml.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzggmzohb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gujgkbayv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gbumynzll.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/guuwwazqx.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gkkngclak.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gbbpuyrni.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gsgqplpnk.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gsuymwurn.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/ghnarjcxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glpgtqfnq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkodeqcjw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gdmygrquo.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gctujgnli.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ggwhcxlbf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gmaporutt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gtpjlotla.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gshblwpwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gvundsihk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/guasgcfgy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gefsuimvs.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gmqwaxzfx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gdzbbykgf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gzmajergv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gqkrgcowj.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gtgyqgefa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gktfiuqom.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gdssrqpoq.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmggdbidg.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqxqzfhis.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqsytxxob.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghjlaeehi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/grljnswdx.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gywrrrhsb.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gtmqszfgj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gkxkgllfa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjbymhaeg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gteknqtpo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gqaxtbrsl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gmtpmcvkg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gtnrcverl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggszqixkq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gxpitkebg.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gwfvvxhdv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gyjkjaqqg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnhutpfoe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfroxchhz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gehbuzsze.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gpydwhycu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gtwdhrnpp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gzpftepwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gmiezwace.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gavfpavji.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/ggouqzstf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/glgtahxlv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gbmllhzpk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gdbqfnukg.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gewphnbeb.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gltrhhtvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ggdhzxgwg.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gnlpcctfm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gcusdagut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gvqiloneu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gajjuvqkz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gnkdtrhbd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gasixjgdv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghuacffgb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gfjpfdqtv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxspydxgv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gguovclhe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gadhjxzji.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gjjqiqrbe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnxsmwzga.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gwntfzqyt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gqogopuoc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gxitkmlpg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gtpbpsola.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gidzlkchi.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/guescnlng.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gkiwedrsh.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdwfaurqf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/ghjbhedch.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gbkczzmpb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gpmcuokvv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gnfpipgbh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gsnivitag.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gdzgerxyw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gmhvomloa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gzbizntog.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gksddrhwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzoqqpklt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwyoibsiv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/glavbqady.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/ghqopxvls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gqguxuzfn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gxntfcqyc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gqooousjc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gwnvsdjdu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gpwheznpd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gvyeihchw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gamupywiv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/ghzjnwmnu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gvbwhjodu.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gbmnotemz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gurbxbggg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gtmbpbppa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/glermhfqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gycystdnv.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/grmuosfzz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glarwkgcr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gkwzkaxvv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gxhobnsdy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/ggifvmtrj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gioqolger.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gzvaravjj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gyaawyhpc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkzrhqiya.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gijovubab.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gifyegidl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gkgestcke.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghjwugcgg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gztvqkppk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gydnoxhry.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gmlfgsawi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gjnougvgn.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gmzxbxwnz.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gtjrmcwsx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmaqrxaig.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gdfnwzzcu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grqxmtudm.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gommbtilb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/groxcnoqd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gbetkdqfz.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/grwepvohm.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gtzrodwao.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gzzipyqhk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gdugbyfnp.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gyipfxyvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/ggbemlnlf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gttpavnda.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gozzcsnht.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjpwmoq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gjwfforuv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/guveszlkw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggjwpumdc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gwzutonyp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gbcsffloo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gdyryukxo.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gswdmohll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gkzaybpzs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/girkycfkh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gaquxplem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gqoepqetg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gutlqxnkt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gutwhbznf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gaehhbodd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/guxhmytgd.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/goplaljor.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gzrtkdrba.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gqwehbtqe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gprfizcno.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwgqvwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gxmespmcr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gbhbgkxqh.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/glxdkyiqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ghulnoewv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gpivkehrq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gykcmbeeq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gpgnlwptq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gptcxkdof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gmcllmgpr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gzgotqbab.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gylxntnqp.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/glrraqrea.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gesmipuwx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gdaqeqfin.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gcyitwjjb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gsuhbwqhp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gjendjvfg.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gbftdqhum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gpvstkyom.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/getuisyrd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gpmuyjmol.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/guumtnkst.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gssahnzyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gbbuxhevh.sHtML


<!-- 参考信息 -->