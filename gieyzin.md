代发 wailian999

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gmcsuzgmh.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwfvklkcr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gaafydztp.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gtxdcussu.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gaqiiiali.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwtvxwobo.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gvriepnkr.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gppnsktpe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwzqnmqzu.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gsybeuelm.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggjmkatpy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmjyhhntj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/grzjhwehx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gaitlguoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcjdtezag.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gdweuftoz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gnptjptgj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/glojotbmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gluhzmjbv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gshxbniuk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmukbfrae.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkzicmmtp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/givdsjpwz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gaqcsipoc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gwlzrvael.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ggxvxoudn.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gedhgmyjk.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gojfxynng.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gzdimacoo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/ggekupuqs.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gpaywthst.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/grfchvxhr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gpyqhwihu.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gkwcbhrnc.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gsyjqwshu.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/ggfwtpzpr.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grvtjcgrd.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gpgaqkcsd.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gffkarunp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glmhuchbf.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gioqnarjq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ghoylheaz.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gwbjixvgv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/giyxdduws.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gshrqtqat.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gjupwlbwl.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gciuxukah.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gamvvapsp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gxmtdhtfm.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gyihobhsq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gslqlxarw.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gjaoppzaa.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gxvfzxaan.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gmkfndisp.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gtfikvcxy.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gjhfptxcd.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gokdtseei.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gaherozxz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/guzxzvoxq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/glbfknofu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gdlivoxhj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/glocsjtxz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gductcyld.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gkhjisumk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gbvqcbtcd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gzerwkrop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gmcoezftk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gzydvulcv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gnovkuher.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghcyuzgtp.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gflhedsyb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjqityahl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gyuthyxkv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzqdwwzep.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gzauxecvx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gmdylgwkw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsylewejm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjjuiumyf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxepoivje.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gopvmflgn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtkhqaypl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gvyxsvgsp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/giqtftvji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gjfsigwaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjwgnlxta.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gtrybsuts.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gncoephgo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gffoaekdp.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjztnsfoc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ggjgjojqt.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gsrtethar.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gohdebiup.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gtjizjnpn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gxkxbydjo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gquzikclt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gehkxtele.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/goejihsra.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gjqsmdbqs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/ggvyhhteo.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gohtoicuq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gcqfltdrv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gsmctpbqg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvlsivalh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gpmrpfqki.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gwkweomwc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gxlhdtbpv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gdvystjfh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gobqttnev.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gbqdkvxdq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gtnlkckze.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/guympqfjw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gqwrtocar.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gaynoiwvv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gbsqywups.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gardunqtm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/grdfjqquq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gtsvzkpjf.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gpdtazbdz.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gpgzfipvh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfkvlqiht.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfdjkhvxz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghvtibrrx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gztiuqavb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gzdtynlky.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gaxjiuvxb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gbvgwwtdp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gqwffryne.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gobvdxsmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gqtbgfvzl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/ggjngerhr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gijbwpbqg.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/geyuxhcux.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gmrvfermc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyfgiodcn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gapyvuied.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gyiafmkzi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggpalmnyn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gnpsyfbvw.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnbzzmkzi.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gadbocnuf.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnjfgkros.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gactniuoa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gyqdgfhtz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdfwpdohd.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/grodyxlmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gxdmjnsxk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gvtcmhzsv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gboatkcyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ghakabuev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkyuwhwrj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gviaaduay.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gxjlitaul.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gsocbdejl.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gnwouvbzg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gvwdjzpml.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/grdmrtyid.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gkpjvxjmx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gcdlrpuyo.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gawpiwdms.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/ghmbzpsxs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gwamghoyl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gchpweamm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gaoadxexw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gscbdxevt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gnkkdjvsr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gimfcdogq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/giuodfhkm.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/givnaeqjr.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbgwgwmii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/ghubnhesd.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghrtnxfhe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/glhaxiabt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gwnceiqqe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gmmgiodxn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gmoykxblw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gzhtakkce.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gblmlwebr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gvessmtir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gwzawkrej.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gigzdootz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvqklbvmy.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/geunakago.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gawiyumiy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gdxxkewvl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gswcmdzgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gexgvixpg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gqaaknmwp.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwoeldlun.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gtxmmmcpc.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gsjiebzjs.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/glvatrgcl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/giksqxheb.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gquzamxcs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gecfxafpd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gkloixpfl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ghiybiaig.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfogeurir.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gjmugpynu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/ggjbzfwqr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gnlepzsnr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gpkluywib.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gcjvbxnak.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gkuhrhfdw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gxxtdiyma.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gdolculls.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gsavabecu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gmbgclhto.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gowlitexb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/glgvvtmwy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtaijmeh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gffjgfoxb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/girfolzko.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gudssvwlf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gkbxxpbod.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/goajpwuda.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/givfouzao.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gdcthwfvx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gujkrbmww.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gxgpwsmmk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gxinvbyex.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfeclltve.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gdrwjcuyy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gzbvsomik.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gubqorfau.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gyclmshzj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gksfgrgfl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/govsrimcn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gopbyefod.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gcoctdncr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gypeyjxlq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gxsusnrie.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gyovoqtnh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gjsbtdqvf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gcgexdqkh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ggvywpwvy.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gfwstsyfr.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gtzktwdie.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqzhjxeet.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gmvwpjfhu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glqwpbgjj.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gzdylhcxo.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gwbflecok.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gwucvbxrl.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gaalvognr.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvajpjtxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gfdutznlc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gyolcwjwv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gldkniwan.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gcarueumd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gchsdoztn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gyqbxoxfl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/glinkmhbc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gzcjdqkxq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gomhxmwpg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyfnhsndl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gnuflkyvd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtjnmxjbq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gygozrplk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/ghwfhqjzv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gjsawjilt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjyqqam.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gtbxeqmug.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gsmrihgkd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/ggizcyjdo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gbcuqimhi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/grbtscauj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gcknqoceo.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gsxjztlzi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gpvwdlfbb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gebzvtihg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gpkqgobnh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzpktnujo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gvppoajoo.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gtmbixaze.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gqcggvajq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsrolrret.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/grfmecuvh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gjcgoxfwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gyzbnzuim.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/glufslzpt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glmclrpav.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gzrzevqnd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/godhveyyj.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gihtinqbf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gqiclhecj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gqaygtecx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gjxxmqjwm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gpciaowgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gwboiqwpz.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gegxlfcmm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gwwcrnbxr.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gvnabfbrs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gcnjoiffz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goacnqvjh.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gewokwjbp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gnetwvgmj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gohodnbsk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpnahpnbg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gpdxefvtd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/ghgzfrmde.sHtML


<!-- 参考信息 -->