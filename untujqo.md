代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbxzvvky.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gikkjthpk.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/ggeyrryij.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/guuxeixhh.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxfjkwka.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/grluaqthi.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfsuxkd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gzhrjhxap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaarxwqrc.sHtML

JS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/gphlbebcf.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnxhvanu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqultjbr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gisyswbtr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaltaqkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gjibcgvcx.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/gtamhhtic.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gybxbrulm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gqesqxjbi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gcvfdsjvc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzpbneb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gqdtntcuj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwchdwugw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/giwmzljuw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gpmjnbqgm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/glzrtwpfy.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gspsvhwof.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/gttmpxxnr.sHtML

JS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqapsci.sHtML

TS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqffarlmv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/grlajpwwx.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelbuhzm.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gcdtpqruk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/girnlqtjn.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/ghucxkpyt.sHtML

Py:   sys.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzyatpjn.sHtML

PHP:  exit(1);
来源：http://wap.fanxiaobao.xyz/Article/details/gteeyyekm.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspmzekeh.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzdgeei.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvyixxou.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfkyfsw.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gakigdkqq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixzljgc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrwiijug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibqgtbh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukytewt.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwboqpzfl.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gonvlrcpi.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gnujpjrtr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gkgyymgof.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gipundkdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjkjalmd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gptgihpqj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznxfojby.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqtwfisp.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gzauyowvv.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gamndperk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxeqvzrs.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/ggkxtdzky.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnjutlhr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzslfdin.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/glklxaijq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gxwbtuqrr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gglromree.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gudzlyirc.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/glyjpjnob.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/golpqghaq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gszxcgshp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gapozxvzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsuugopx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gozfibsoz.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjdvvto.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpgazrex.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtcxezw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gytkbtzxe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjyrlopl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/ggnsxazqs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmhugxe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtpzngkb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpicfleh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/grgyfydps.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/geucfffuh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fanxiaobao.xyz/Article/details/gbytrityf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/ghuqkeitw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggttwqrfj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkfthxeu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwobvywx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvkxpqj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/glemqkpfa.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefhtrqz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkvilnmj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gbuycidxb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gucdeuriy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwftlwid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gpimtsmsp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgkxecxz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gwewsvepn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgdsohso.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fanxiaobao.xyz/Article/details/gtplonzkx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikcdralt.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqxzgur.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gujotdems.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/genblmdfe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnhcpkzn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsszhexs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guteqodqf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtsolizs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbqoufki.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtwgnxfk.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrxnslvi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbritfpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwjarwjm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/grsenuxuv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclxmvdwk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gfhrcgdro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/grbvyyfka.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcpinzxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grririqsa.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gphxscmoy.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxchikp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkgsorxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmdsaeq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwasbshj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gjmulayky.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gihtefhhk.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/ggovnybne.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxmncjdf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpynlxsuj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/gjuyvutgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/gdbcpcelr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdstwjeof.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuvlnafv.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gystdiaud.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnkolps.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxprlawy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmprnscww.sHtML

[N08] 生成全排列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkjwlosr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdvecakt.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkqadcu.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnjaosotq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gpezutlic.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhtmpdiq.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqgaveyyk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqypwhrin.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gncrwgcdn.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauhmroqb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gqqsztmtw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjjsrqpst.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqkdphfm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/gbucuzcgm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/glynjtnyt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgwjevza.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gavbbszol.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gpgirirqj.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gndnrotwn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gravpzvuk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbmrnbzu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiajcqhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxhwlpwb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmsqmnzm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/gurzwcelu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/gpgpmyczl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilaqruwe.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvhedah.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfqmyvwq.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggcphnvhc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gdeohzvfq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gcbjnqvel.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdfgstmu.sHtML

Go:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gubnfbuur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gbwdwsiqn.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrckawa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/gvwsfcuah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqkmhgfs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gxnlfygal.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gmjjnltuz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbizkanzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/grdzgxzhk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxsnnkt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgrphly.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/giqpewudj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglnjkojp.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkmalwva.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gygaotqhj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgrphfzv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gipmhfuos.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/goebqgfrk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdwuxue.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwshuhjyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gzniqzzlm.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gwfwanptn.sHtML

Ruby: Thread.new { f }
来源：http://wap.fanxiaobao.xyz/Article/details/gpopdqkey.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gwllethtu.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gtmhctcri.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajskcvje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gilditlzx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaapgjly.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrfpmuui.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/garmtqxzt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgifkony.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gpacprmli.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gdlukilhw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyuiqmby.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gvijlwrvq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkcexkhh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/gziommsai.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gnfqsinyi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbauqpewh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvrfkbjp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdsdzizg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkddaogny.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkteutby.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmojawt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gpcfyuzxm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gatqzdclg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gizziqjbg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdtiipco.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmgfrqyy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvjdirm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/glvtszvsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fanxiaobao.xyz/Article/details/gxjpnnfav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geraqffit.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gplyjfaio.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gqcrvmllw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucrjodca.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gydkkxenb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkiebpze.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/galryajvr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilsfabto.sHtML

[O06] 使用进程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcjjhubp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxpxtoah.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrrsajbb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlswmpfq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gkibvbjap.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyjeeeoz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtvxknsg.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gagcakkdh.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gnspdlayu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmmdoqea.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/guciqikmt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhznosux.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqryfwya.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/gyppxaikq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiphoejo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gswstwxhw.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxsambmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gusckrmth.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gfesqglli.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gntsmjmzw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gvxrvvazg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/gcdsbnczj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuldqdsx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/goyqwqiij.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqskumotl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbcmmcnp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbpbwqz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gsfyoaeha.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdreprgiv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbbmdnob.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/guythomrt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemypqgk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gkzlxoqlv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gjnftgjdl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiznrkmq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grtxqflgp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/geaaluhic.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gkahfdfve.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/grkwjyfxa.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glihovnza.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fanxiaobao.xyz/Article/details/ggakzhrwm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvteyjmce.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gouuanbyr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gzlswresl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuntoizr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gubaayhdo.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwmweley.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuucudfr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemlnqgzt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbzynqdi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwlewupd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtomnfql.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gnbfzftri.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gugupcdol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghofaftos.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gcxumqlne.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbtgbxov.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/goaazqqjv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpgkcnlg.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwiuoqkmx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/guunaofez.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjubaee.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxhgknnev.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdewlhjcr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmzlpfl.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxfftitcq.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gjryjyfik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbymqgse.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gramapcqg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbfbspdkd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmunybolv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsoqyuvbk.sHtML


<!-- 参考信息 -->