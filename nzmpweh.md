代发 wailian999

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkxjxhnkf.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/ghzybuhzt.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/ghkkzgdjl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gqqujiqlb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gchuerakx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjelmdvhp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gfjngwtwb.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gzmqadrhl.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gpzlbybym.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gsywilwct.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gdbvgupsm.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmcvcdmrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gjwmdqzxw.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/ggnkoendb.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/geadlugeo.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gbzipseft.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grkbsbxcs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gvudhdvuo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwkggitfr.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gxdgsjnue.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gogwfjokw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gznizzqlh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gerulxknt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/grrhlkkrp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gbznfooml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gpazfbvhv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gqebfsnvt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/grezakspb.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/goxzszzwq.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gbgvppklh.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gxokuylvm.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpxqokxia.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/giyljqoia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gzchosouq.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gcnqanbpy.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gzrsacnyt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gwozpihlr.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gckvmtahr.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwztnryfj.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/glwcrmhnw.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkzwdhnve.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbonforzm.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gtrrabzqo.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdydnyesb.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/grlmzyvbv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gvpalfdhx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gvrxfolbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gciuvmtbz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/grtzlcqsy.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gycjrewiz.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/grymggddq.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gvynrbquu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/grhyzmjjc.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gxwopgqzj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gpaafiobf.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gvzxicfxp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gowuzvplk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gsjykmhhn.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gzeutwkob.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gwqmpljmi.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/ghskbenjz.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gnkhawqkl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gombsajye.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gplizafhl.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gspnopdwx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gsajqleda.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gwmyctikf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gcknfxqih.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdglipxya.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gknubwbzl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gwozimvxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gqgznqlsw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gfnivjtss.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqixwlivu.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gldtvyekn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwzlhokch.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gidqvwjba.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghcnbfgji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gdyvdweor.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbznlpw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjvhqvlcq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grjjodeow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkmosllsf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gjuyuzmcs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gayqcwvii.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gbtymcbol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/grjpitrbp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gmtdnmwid.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gdsothhkf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsgmisdgs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gmxbmobgi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/geajqoxmj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gyrcvjfka.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/grodpateq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/ghzetgvvm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gnxkelufp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gffedsbes.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfybwtbwx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gjeotvuzg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gkuqkbtrh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gksriyrcn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gycieqala.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gmxjowqvk.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gkqeeyiau.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gwsapvpca.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gligdphuz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gzxzttqjg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghgdyekwx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gshhinvef.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmpiyskks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gitzmditw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbzqviwpn.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gjcmuaxxg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnlvsbwul.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gblturssh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gsxlsgawb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gwgoobbhd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gidvqvjag.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gmordgoqj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gwmmlhrnd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwnwiiz.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gvqwdkurf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghiazbqsf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gdkxgjmck.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwcqvlsbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkodcjwom.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gkkmhjpta.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gdeouldes.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gcshochpc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gmeynfxlz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gnwxjvttj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gqfgczraz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gnlpclanc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ggnimbnhc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gtpbkdrbe.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gmpzgqztz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gyejmrneh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gpdxffrez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gzpysykyc.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gojllhzaj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gqwlrnhhs.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gjctzaqtv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gahvwjukk.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkfotkbil.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghabwkzgx.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjtuohicn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gvqxsbtbr.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guziucuqc.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gbwdeeydw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gblykbdtl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpufsostr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvnrosddg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gtenuigel.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwvxkboia.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfpnfno.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gkfhycfce.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gqfkvokpw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjlbjgyqz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gpvvwhlfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzbdlwkvt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/giestodby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gbrjckkhq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gsurtzsvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/ggomctdph.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrhunbm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gpajvjmqn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gubpcgzsd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gfdoemhxf.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gfgygqgbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcprrydin.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gxwgsdpli.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gluoycfik.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbdekjfkd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gmldodtlz.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwqkykgse.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gevnneivz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gniyzhocd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gespojbka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gqpknuwap.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gmbpksrrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gickogtpu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/guacilbxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gvlikbtja.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gemixitwk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqwqtlyyh.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gbodsjqzr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxvnjhupb.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gcsoodgda.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gkafhfftz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gveigwako.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gtlrgpgrf.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grpdlpdcu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gnzwrcezq.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gcpvhujvf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqqkshn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gurdazocy.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/grguyjcpz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gbixrqaxc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gotzibddn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gtleidair.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gukjpgtaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gmutsrbgp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gotfwayfl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtnoylulv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gmcwacptc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gbcninnqi.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gtfjcbgko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gfrkhlfzc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gbecxxbcg.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gbgddpyzm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gjkkcympp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gbxwcaofb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/glgrmqknl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwdahhwd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbehmynvr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/ghvedvdrs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gueadrfkg.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjybawdqk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gbwinjcru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gunbnjnkt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gpxzwlkej.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/greiiyxbr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gcozhffrj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/goonhajfp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/golifixrf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/ggozwazgl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gapoklmco.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gntpdoaro.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gcydxigoo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gcssqssgh.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gdgyyvamh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gqmptyeyi.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/grtwpgkez.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gonybpiam.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gbnhwtctk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gnygwzmin.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gtppftdxe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gvqybgudy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/ghfycqjta.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/ggzcfgdkz.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gbkmxceqi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtsuopysd.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/ggagaakpu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gseyuuzzh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gubbvjtxp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gzeatmuti.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gnsxduhry.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gubltpksa.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gcmparjhx.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/guvidxfkq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gxjveozgq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gldngdrok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gjvfmygvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gavbqvslx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gwczqtcrl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/guurvsafv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtjqssh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gtuylphum.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/grsrttrvf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gdhlkytyh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjayioqva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gyaibrcxl.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gkyutulrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gcxbusxri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gpzvzpsqg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gapbjnewq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmombbhoq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gjuzhvolv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gqmztzovl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gefjtlgts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gusbwnwea.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gqbamvimv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gejugkfgb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gnvotaviv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gqaxgaeuc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gfnsgfebk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gkjxbtxys.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gudbacejm.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/ggctyasbb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gernhqpbn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gncasqeeq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gzytckpis.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gznlabhie.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gvzbmqdrz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gmxsfithv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gezwgddse.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gtlzniksw.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/glvmriagu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gfhxtoeni.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gpqffhzzn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gpgdgveab.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gwagutntd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/girvdvpdw.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/girakbfxd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/guhashxcf.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gmbbvfded.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gaismpxws.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gqdjncbyy.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gorckdhfd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gkmjzirnz.sHtML


<!-- 参考信息 -->