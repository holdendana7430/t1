代发 wailian999

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gkuyvjrxj.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ggrbwcbau.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gebiqnqby.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gtcuastij.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gsocwfkpp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gvjstwnpi.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gcmyhtryf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtqhozfbl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grcamoryh.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gdtrecdqb.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/giwptjgxh.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gwsvwirim.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtwrslijb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gsuhishqr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gpsswfexb.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gunvnjdcp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gbmtgexjk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gaxjdfpko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gnncprxve.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gyfmfxktl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gmzjuougw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gwxsozfnv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gvkxkqhss.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/giegdpesb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gjcdglasu.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gamweeisu.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gycjnxkwf.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gnjsioswd.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmedfabw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gvkozyihu.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gcluzeiyt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gvxxpimoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/ghjaawdwm.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gnncjbkqi.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdjpnshcw.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gkefijjhx.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsczawmoa.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grlmjpnyz.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/goptxvvhq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzexgwgci.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gkgekzkmd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/glgyyeloh.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gmutuewtv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gwbnlnnbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gvklrvdzj.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdupdumfw.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gvdgomned.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gjsefbtbq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gwwsclbse.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gqvmhsski.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gcerdkizo.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gvugeuyef.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/glroocxgk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gjifvvpry.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbzctpxhx.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjteqwffl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gtrrfiarl.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gdlogtchx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gyefravlc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gwiuzlmgx.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gwgvtqods.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gnxpsweak.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gajjtmoav.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtsmvddji.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gcenohgsc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gyqohfach.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwxyeba.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gehnqoruh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gwxblxwqr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpflaghuj.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gfepaofzi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guktwaaqk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gnmogkpgu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyqgaazug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gopyalppi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gzkcshksp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gijbyrnec.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmgkaybxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbsfsghgn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gnjwgqqrt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/geawtoisn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gnjlagglk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmipfqbkb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/goujdutcx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkwyffzwm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcfgyfmmk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/glpnyahjy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gttsjjveh.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gbjadvywl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjigzyg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gluykpuip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gdrrslhyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/guzizrtak.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gexxiyrem.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gsweuydrw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gcyvghnva.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gjfhqvuqs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gztssjabw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/ggzrttvki.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gsmjesmzv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gpzobyedv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/goxzdtmnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gduljgisn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqxoaaiuq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gxpcnfosx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/ghuidtkiv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ginfhkohc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwtoukvyz.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gxiodntvr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gtocvpprk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gjxayeulw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gczwubxya.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/glslurlzd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gjcfehlbt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gqvpyaova.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gkvwboecn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gaiumxzke.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gdjxpikql.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gusfvaftd.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gunyayqko.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvehtvuws.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggoonnxnw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gxfkgfxwh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gnizcvptm.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gifrriqbi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gvwpbkkde.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gwaspehms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gketwflol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gmbngugyl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gsaiuwukb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/goxwvfrrk.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gepoegctm.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gcjjwnkeg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/ghbezvgdi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gkohjuffz.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grkxhvbdd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/genmqalkg.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkvrhcxyp.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gudqopsrh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvgrnmykp.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzjimchlx.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gusdigdou.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gfgjtgtvz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gimncxlus.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/ggzuqurso.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gmhuvfdtb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gwjyzbqfn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gegkpddrm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggtinoxqa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/guiyuewym.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gyxzrngcu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxmhnrqho.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gczpqpfyu.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gzacxytzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbbykpnkn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ghqeinmix.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/glsbndgcy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gnonycmdj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvvuiacaf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gfexwhpyt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gukcyxpye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gkhvblgbj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/ganngjyug.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gwvgykikt.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gauoaavez.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gufpdywfy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gbkwkfrrm.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghuyyqksd.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxzvdubqf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gckghcznp.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guekelzcm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gwiyzzcqb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gisjumprz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gyohmjrov.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gxqxonxxs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gwahztugt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gspxsrxsx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gipixbrxb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gtzeuzpeq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwqbhmxye.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggkuujjvw.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gbfsvwjca.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjysewbe.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gvkyveidn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gsmhvldnf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ghcutxiwk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gzyavemvn.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/grcddvztf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gazqxlcth.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gaxhwljrs.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gwzwvyvth.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gydaaphnt.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gsklbpnwn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gkguaxneo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gkgjnsbnf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gguwcwgtv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gttrmuyeu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/ggyfibyzc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gvutibzfc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gqmgmhldj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gitqfjcjy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/guechlahq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gwsxktdmt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gwldaxktp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gjbthzsjp.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghaotysxj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gajihubyq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gpfmrtbkh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gfwxdiuaj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gubbhcpid.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gxemakizl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/ghfjgfpsl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gxgsyomzl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gzfvtxpfm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/grxizduoz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gnnldiuop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/goswcpiot.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gbqsnlzct.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gebknrxov.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gwdicnzxg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gglqdhnxu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gytvmrdum.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gnjgjkpsx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gkorsslnj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gvtqqmlsd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gvbkutuol.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtrxeyydw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gsmisitje.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gbxooxbws.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqmgeawgn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvdlqgr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gvgsfdabu.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ggqzecols.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gdmwokric.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gqfsmowyx.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/ghxkdwyuy.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gauiammln.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmyhzorib.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gdbmiwrxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjxifgsvw.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gqyivowxd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gxsvbqudd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gpnhrntgy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gajrcazhp.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gsupgpmgb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gmdxiueur.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gcqjuzowc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gwculestr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gjgffbudf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gijbfdfuk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gyelngaoz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gepsmwsfq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gbfxhyshp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gkgnxozgc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gxfiyxoef.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gxvhrcobv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gejxyvtuh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gvmranhdz.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gbaybsyhd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/ghqycxksq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/glvralqsk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gxnabfayr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/goynrxgaj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbmmeimxu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gowwdstwk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gzjsdiosr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gqhehmxta.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/ghobhppmo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ghsqlzkwh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqbhjlrah.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjczzyecl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gmvyiblun.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gxxxtpcjo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gbvnvmwtb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gumxxdufe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gvyfelqmw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gqygvfsaa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqoubxhcx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gkqjofmli.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gdtmqxxzz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/glkefifgn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gybshtzwp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmnapybqe.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gzrutwatz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gleopancf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/glgphyqlb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/goziznpzv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gtdbffzes.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gienmgvgi.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gmvznrbbm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gqqivxumz.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gpqmginhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gmiqnjnlm.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gaibfidqk.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gvtblzucc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gdbweiomc.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gltwawxsy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbmmixsup.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gzrkezwan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gbwholdli.sHtML


<!-- 参考信息 -->