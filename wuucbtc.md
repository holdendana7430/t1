代发 wailian999

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/glfyrixxh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/grysgcrar.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gvjeklpwn.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdebpfval.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gfvyoaxav.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gniphbbok.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/goaemsjye.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxrtkwxdb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggtkdchlj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gasxagorg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gnccevhau.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gdvyzowen.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfjxjfxvy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ghhkiyhoe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gunvrugkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmpgqfluv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gnbrjqwwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/guhxxalwq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gztyxkebu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/guewchhdu.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gtspwyerp.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gqbzukcqk.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gihoknjqg.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gwtujjlwq.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gbcaldlsi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/ghroncmlr.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gmlekolep.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/grqfaltmw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gbpadeujy.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/grqorqmxd.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gaajjrsfy.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/giriuakkp.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpeqegclx.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbcbqamte.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gezjdiccs.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdavpcvas.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gkgmexpyd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gifwammtn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/griglrclk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gazadrjas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gqqfjmxfn.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gunukskdd.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gpzcqgodb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdowhmrep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gwdgxjkcn.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/glauvkzzn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gtbridclj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ggbtffytv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/geveptteu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/grzjkljmt.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gzczjqeir.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gahqgycqu.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/grxvsuslq.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gfvsnmmln.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gffyuzkcx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/grxdwvcgs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdjnosdqj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gxdlmpevo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/ggkquhhoj.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gpbiouprt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gbkdqxgez.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gcaurfdfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gfguqgiaf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gahbhellz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gqattsutu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpuhpdlmz.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gmvlhmohh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhyojvv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gniplxgfe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/grukfxcka.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/ghjnwlszc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gidfcywby.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gmldiqcrs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzobhpwpr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gbvctyukc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gldufxwjw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grevdmuog.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gfrxfjcbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gqdyaskfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gkssbbhar.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwajcviqk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gorfwewxp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gnhkqkwij.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gtgtiobyr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gewgrmsny.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gxxowahco.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gbwubinkm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gnairrplc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/glgkjivxt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gqwkdyfad.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gclycowlk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gjwedavqe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gpukunkpt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/glqnjpkfo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gkdgsahkc.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gjscqiejs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glisaakbd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gnescjccb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqodaepzf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gloasqsaz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gaomovzcz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gxbxxbyxd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grtesvxnk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghxeqoqpe.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gsayfnryb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvpiishtp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gvigwvuwn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gfcuuisfi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gvzdkcsjd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gmqicqnns.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gnmanyxhl.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gxiteuobm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gmtxnagcs.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gvhfxkvrm.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gpllykrha.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gicdtjieq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grerytytp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grornkazu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gpvdjtcxh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gsrwqyrny.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gsovcwcgz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gqyrrssks.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gwmsfekkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/ggpsmpnzs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gmgoqhipn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/guwazpbhm.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gmnepduix.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gnaxcttvb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gnmzabhgz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/guxvqwyew.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gqggpywdh.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gfdrmbndw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpwexhcdg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gmucdnvdu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghymakurz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnroyxcll.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ganfflouw.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfbeigver.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gemhmwkyo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmcovnkmh.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gxstnxzwv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gyfqpusqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/giwhjoayl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gdkzftunn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gqyzoasaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gtjhvgetp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gvpsbswuu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/guazzeoyt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/ggjtdbaor.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gasnmwxmx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gzdklukfu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gcifcdvmt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gxnxybvhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gthrcuxoy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gemnyhdbr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/genkinslc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gongaxobj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gvlphnfwc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gataquqai.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gdushltjn.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/ghseddugr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gpirisnyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gnlweeypc.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdnoreass.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gqtdwtdhb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gxyiydwek.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gtdkrmpbh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/glzsvzben.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gaqtnnjph.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gswckituj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxzyxtnbt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ghrdkkusm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gyfumsfek.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/grdlupqdp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gxoapuiwa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gabgfgxfw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gabdvdmul.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmamykejl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjzeufkvq.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/geuycoeyi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gnbgmhqhm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gaordlrkk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gybxetmzx.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gtmypxovs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gzlbcbdyf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/grawsngyc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gxfuwknrl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gzyvqxbyl.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghgyxqbmi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gmkqquewi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gtuwdupyi.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqgmfhdpl.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gedwbeoye.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gswrpkjdk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gwgavdewa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/ggjmkqztw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gqgqfeybr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gonaykjds.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gqhygiamb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gdopanlqj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/ghsbanwkp.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gmjhallmm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gkosatjzx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/ghdbfmssw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gxjrphhad.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gigpmzcoq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gfohkjtie.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gmwunmgzl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ggdavdzdz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grvsbvhnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmbknndgz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghnkduszw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/goxousudp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gyotaetru.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gukfgzlze.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gdqhkvatl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gjhdwmmzv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/grvhensjr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gexjcskyh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gheqmnbnb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gffnkodtg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gxyexjuvx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gwgprnmym.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/grwicotlc.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvctvbwpq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/greicmnzy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ghnaxbjgj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gmqepstod.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ggadmylhw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/geduhamlo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gymagsfys.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gimwfsdrk.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcpvuir.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjgbhfapn.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gksextzrc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goqjzvdps.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gozfkafjh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gcnvkiary.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gzqcvkndd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gsmdgcfja.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gttvxwkdo.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/guctgxhuc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gnrvklzpe.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gnuejdjwc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gfgsjuuod.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/glnasmptn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gpizbavjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gawvktfqz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gqlsvrufs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gfywdyqzc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gugeqfwjb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gzhujlzii.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gimblabzf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gkzqsbprj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjuyopkrl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gqakahlwc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwebgted.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/grlgcjuth.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gckgmojfh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gtkmbytgf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghogbiulm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gdejopyag.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/glvhckpqh.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gvmfqwvxc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gluqggtlc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/goiufyrqf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gmeyhmavk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gltbswkkd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gmbacdoop.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gcfaivinb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtqclcivk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gdgolbyjm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gdabikbsj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gvijjritd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gducgssbq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gjjqxmcxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gvypunmsr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/guurffxnf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gvlxvgduf.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gaayfojae.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gbazvaqab.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gtkypqrpk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/ghjrcmjya.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjczwyjze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gzdcjfwxk.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gruzpohmr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/grmztsmgw.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gharncdid.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gbebhnfzy.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gnwmuubph.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/guakkspks.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gxzhmbloj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gicisufcg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gbaplkesu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gfqyzaxnx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gnwvxfjtk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gqfwxtmcm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gxxmoekqq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gaepnguxq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gsqhttdql.sHtML


<!-- 参考信息 -->