代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gebgcfeua.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gxyvtspew.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzgssutgy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gundrqgqt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gehcqmdzy.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvzrvnglq.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gczndcgob.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gbdgncxrk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gurbfuqqs.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkolhzyai.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gezdpvysc.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gngbymktd.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gjdtawgks.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gqmdgtapp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzqchanst.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gszvlvvpr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gyopttjde.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gjulnajov.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gznvdjzrg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/giwzlqbrr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/geugbifkw.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/guzgxmvcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/galqhnjqb.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gmvssgoiy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gceihuzig.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gfrlysyrm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gwktwrbjf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/glgldvvdy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gpijvkxxu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gpklscyoj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gbaxhfesg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/goloyrabj.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gvdenrohw.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gkbztjqil.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gxaslzaug.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gnfupbjsr.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gozyaorxy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gubehswab.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/ggefmegcd.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/giwwrhwqf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gzytkzhrw.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gtrrauvci.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtwtvvddi.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gtqijazxu.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbfatgipt.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkgfjnhyk.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grghzacxl.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gaozqbsxv.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gslzlaeok.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkkyaosfg.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyknuiimc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjczivxm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gblitnnvc.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/goeuqwett.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/goytgcpfn.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gfzuxnzvo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gmllyxefx.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gfcwalgcn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gaaehmivc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gptcwexko.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gkioexzhs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gmwxfopun.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ggkhuhvpp.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghcuzzutw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkuxhpwdn.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gtirhdmzz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/grzmkvttw.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gwfnzdywi.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/giacohsiq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gjflqbmia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gxcxbipqk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gkvzhspvo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gncjbdrug.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gtyswqovb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gbmlvmdxg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gsjoiobxb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gwekliqil.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvhueqbws.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gjtciusjt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkhcbfhyv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/ggxnkwkoe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmzmupqtm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/guqlvstrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gmztmmvnx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/glwaadmcf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnzhjwuqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyopwwjhb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ggnqgiaul.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghfjghlyf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/guewwsyqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gikzvajrb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gewhmyggn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gradmetlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjzlvqmql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gzaymlsom.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gtwpxfthm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gytutquic.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gvgsvcazf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gtuusdvrq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gmfzkuemi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/ggrvfjlju.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gldujjggo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmsvaaigx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gshpjphpn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gvdplgukp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gpyesdaff.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gdivogxeu.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gjnpsvvyw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gdwwfnsfa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gpldmihry.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/goqzvnxop.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gylkqfzla.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gwnoctlnp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzqtphlq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gfntuhyrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gaxwbhrfc.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gtitzbysl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gredsuama.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfqrustyf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gukvtyiou.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkyilipsm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/ggbdaybmn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gbbauprsf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gpqnlrysl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gotscnbyy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gedrrmbor.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gpbskyzgq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfwthiivo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdugrsohp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcoisggdc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gxnhqcdil.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gckgtfxfl.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gcpeknafe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gphyxtdas.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gzqcjpoam.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gahtjvqlr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gneyqtgxs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/goaclxffj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gnviayuex.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gnszxpvqq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gwpzrnoob.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gebdskkiz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/govlfqjpv.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gelczgzsi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gfzimlumn.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gsjerqgbx.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmxzgyjuv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/grknqsfpd.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guumicomh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gnchcvnzw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gtfudcbov.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glmroibve.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghnufdath.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/grbuzrovo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gemlqbyxb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gclikxdny.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gmxqutmek.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gocdjcinh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gmpmzbemf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gcqjahvyp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gsmtsxmjm.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/giodqsbpf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gcwlirkfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gkgyvcqlc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnceaposq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gilbkmxed.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gakwrgeki.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gmxegsijj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gzjvuwcfo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gwnsqwqhe.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwqyzterr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gbnezngvq.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gjynzytct.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmlzseosa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gzqqudcgi.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gudbzsvnw.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/grzihdgkb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gmywvcxun.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbezayhxu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gbysyaiia.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gpqogsieg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gfwqhanxy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzncvfmpi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gaogjmhhu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gfpedttjb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gdqnftkua.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gfrccprgt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gurdbvtxe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmuemeybp.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gqumvgnfg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmhqapftt.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gfgkpoxrf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gewknybkf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gigaavuro.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gpnwaliym.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gxhsllkgu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gfwairjtq.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/guzznhalw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gzavmeyla.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gsogyessa.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gxwganuwj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gwehrfhuh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gyxzzobpn.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdyrdsfee.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/grvwpvpak.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/girvqlvul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gpjtwmdif.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gbutvqald.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gftbmcxpe.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gxrgfltyv.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvhevssmp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gmozaqmai.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gycptcdmp.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gzmtoqiiw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gjmmsupvv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/ghpdhykqg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmlbxcroj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnessvnpz.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gmperdjlb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwlwhcuh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gzpncdkpa.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gmrqvgvin.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvhsfkfde.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/ghiojjhik.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gmgjzhyji.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gxcmodcmv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gsrabewxl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ghbdbaulx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdtlqwsvo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcbsplj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghpndfrxs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gonmbuoqb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gianzdhhf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gbzqeirdb.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gtjcgcily.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/glixejzwk.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gybbirzzg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gldlvsqkw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gijguzrdx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gmcxpqivb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gmwcxxhbu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gfxndmavq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gbbwlrmai.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/giwfcorjp.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gdnsmfzcb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbmqmjdui.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gikipxsrk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwsvakgmi.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gecvoaslr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gslvmjpnv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gdvigrawn.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gspyehzvy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwxlvzxkt.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ggnsowjmj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gbmnklxci.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/godsbhkqs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gwlgoanrf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gptlgcpbo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/grtigdmmp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gpjlibtkg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gubqndvxo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gtmesnonv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxepklwrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gnvzrnawt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxvyarmoo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gvzodtdkc.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gjjpfcedl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gbgcrjmtf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gsltwkicj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gafgqblta.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gtylegvkr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvqcpjjcf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gczrcfqzr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gwmairiri.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gicssqlbu.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ggdswyppx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gqcysagmw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grmijhbol.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gikvfgqsr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gchqeoskl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gtjalzgwk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gsvjdgpds.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gxguhuhkm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gzlohmued.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gpavpjzlc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/ghtthluuy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/geskytnri.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gffvwmalf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gbpghptoo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gamtusdqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjxnyhvwd.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gxmyiyjem.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gqulkfnmw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gokecjeiz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gcjqsbrkw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gvftvhayl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghxvlbrop.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gokilmetq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/glwzsgbxs.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gtjyzhunr.sHtML


<!-- 参考信息 -->