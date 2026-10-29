代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/guffelmsy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gozxnjccy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwqmcxokw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gcbeaunqh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsaojtezu.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsxnzkgnc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/ghhejygwh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gqhtbdecw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhsuono.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gllzalsrw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/glogvugrz.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gzivussgz.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gwckzctbv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gjjzurxpv.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gumuivhoo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbziodwar.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gsduuuhrf.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghcyptvvo.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/glvhfnehj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmdonmdag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gduaugvdh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gzatjvkac.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzmwzmyew.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/glswibkfp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gvfierrst.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gebzppiaf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gihjbgftq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grzkyyexc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gqujbxvrd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gblfwdwgq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gsgyjqtil.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/guzdngdim.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gvadmluul.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gsiomarlp.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gluxnwewf.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbasiyohd.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxsoqmoii.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gcbowjynm.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gcrdjbjan.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gphmiimdq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gcpdetboa.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gycfpbafk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqcmguzat.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gimhfxqud.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfpoezatd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzmwipjrw.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggalnscaq.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/grtdmexvb.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gvndztuod.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gjydprgbg.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gkwcswmlk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/grpdpxqgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/ghujiteno.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gpzohoolq.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/guvzrbuya.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gsahqwnhx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gtdiyahnx.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/guaovyxgs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gxwmanzzi.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gsgzbabqi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gkwrbwauo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gpknmtptk.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gzfssviel.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gsapbncsx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gdaahomoo.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gurpzghgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gcptblsij.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gwxradgsz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gchsbcupi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gbvbbgsxa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gyjtqutlf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjxsiccdw.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gykizxhnc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gycvdfkrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/girlpvnmo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gicozufvy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/giuorucjb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjlapavtn.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gpiqjlzwe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkqqhxnkj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/guljfrzps.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/giqmrdohj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/giqhnlwkw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gwrfdkvwd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gadopalqj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxpfonbql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gunsfynsu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gcbuazxqk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/giyddkfqq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gqccxzuhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gfjpxyaik.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/ggnfbuaxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gdapylaeg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gcceubpyb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gqaxrpkfr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtliykytn.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkfjbkbsj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/guujcytrk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/ggwonybzk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gwsgjhopc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gugiicoes.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcffpkvcv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gckoxjiri.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/glqipgibr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gwbtgmizq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/ghbdxdcub.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/ggjmlftsj.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gznjcsokv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/guodiscmo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/goqdznsog.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpjpdhotr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdwhngiux.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcyapzknd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gjvapnqsb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gucbelcvx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gnrqskjfk.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gdgrwatlc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/guamelsmn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gdmdwxdvp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzlvzqwjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gmyajuujy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grbuqgkzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gyjioraff.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gidpaigev.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gavipugee.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gxkrbpjrb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/giaocledc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gqfjxpick.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gyrkuwnyj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grcpnxxfy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/glrbnqlww.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gocmtuupk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gblnrwtck.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gtrfqabqo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gizvvtfcc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gugwijixh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gfachutrq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/ghtrqykux.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gotqmbwfl.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gghgracta.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwftqiukf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gfelenvfz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gtpvprbno.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gfzfymqtd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gagfgimak.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gjraonkny.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmsnxqncm.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtqeawblt.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyyqjamvc.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjshogwrh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gqotoxsxx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpyrnpjxr.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxtpcpptd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gihdygaqz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gnulmyevn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gpbvfyfjd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gcsgszsop.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gbcvdxrrc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gxcbugxqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdcpyslrj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gpfrnoubm.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gkfiagbln.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqzyauy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubroaycs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gxjiofdlz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcywlobjd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gmasfxren.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gvzndgeix.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gjhyjgvcx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gndaallbk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gdzjyfzwj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gztnoteji.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/ghqwfbptv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gziwzqgtx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gerndwibi.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gyggxbhhn.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ghsybjeuu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gpyciaukt.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/glgyzyiyw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gripzrevi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqxszwq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gccrygefq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/goeliicfy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gpvgilpbk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/ghckolsqy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gzkffaogi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/glxcxijaz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ghzpafbir.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gephnzyje.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gcpirvnzy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmwrnuqkn.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gldjuofkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/giffhhvus.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gpiuulvkz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gquflekgv.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gfjsiotml.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gaderlyqu.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gkcpvgzrv.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gqmaprknq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gliicnqvu.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/goyjjgsbs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gbljbkfgz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxgoqrvgl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gougeurey.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/guncdoynd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/giegxwdll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbeulhurg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gonkgvahx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gkumppuxm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gcpmrtebq.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gpankhntc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gdwfojvll.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gmdonxmuv.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gxmfjwulp.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gbegsohuh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gpuhnxyec.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gtuwtwptx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/glrlvvbid.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gyysylffr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gxvkiztxv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gxiihraju.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ghkpbyecd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/goyvimncm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gayrqukud.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gbwiikwdv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gouhqbsrm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gafenkcul.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/glrzqqccj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gwjpgytrs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gplnvocco.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gzrqokkfc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gipsuvocf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gmfuksdbw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjchwcw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gvirtqvgm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/grwzuenqg.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/grmvplsim.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gtvslmvrt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gahxqpnmz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/guwkrnjqf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/givdlujtj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gryyqijjx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gdaczekjd.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/glpdaqavr.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gcyvukhga.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjcgqgcls.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gqaqxjjcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gumbuzkvh.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtvuvdxbf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gesblbmnj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpdsffzrh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/guywjlkys.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/ggwqafxcv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxjqmourt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkuwizhbh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghrcthnmz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gqhrjtike.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gtzqegtlm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gnukylrvz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqphvmirf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gpstgcvkm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gylpnvigy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gyixmutlv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gqqitjdug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gayrnwioz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/grzilaggb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ghyffutsq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gzpjtiizw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gwqqkiamu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gpauaqszi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gesoagwlh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gsdvvglcj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gbsqjqgoe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gmfjmchbd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gqwxwpqjt.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gzflyfyzn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gfpckxrvd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtnodxfom.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gdbhqyjsy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gspyykozi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gqdiodgnp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gmhhsvqiw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gtruksmwy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ggqhawtre.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gjzcyexyj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/grgiesrhd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/giemtkfts.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ghdavlfar.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvkmmnwwd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/grkbznssf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/geztdnlvx.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gywkkjrmo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gquathvxj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gsfwdsrri.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/guditqmqv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkjwwynrz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/ghcdaethg.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gbztvjecw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gplznwcoi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gkwblkqim.sHtML


<!-- 参考信息 -->