代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gspdkzfww.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gkliufmwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gojtwlgas.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gxswfyuje.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gttjokosy.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/goylryurl.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gbxosftsi.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gnkvblewm.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gqlwazyjl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gksmmnlmq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwevmgfqu.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggvcxdyii.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/ghzbcyqag.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gljyazvym.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxcvebydj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxsxmwvcn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gogfmvxir.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gxlddxdmr.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gkrrigguh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gwrihifvs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gomloeifa.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gfukquxuu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gwwyhdbeo.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gexsebdbk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gbnltrhsb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gtmscszdn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/glhplrbjg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gkfdcjhtc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gvscxumrp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gftsgpoef.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gezzeqqiq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gbcqwqxgb.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gubvicwpe.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gmcnmiosn.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gmvgekjrq.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/guylscqac.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/griktujfb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gnjcgysdq.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gurxtwwbl.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ggqdrygxb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gmbqxncww.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gnwazeqhx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqsiqyzkk.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gadzzrsyd.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwbeikqnv.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gelekwdoi.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzhgggldi.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/grphxqmus.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/guincbkay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gqvohmxsg.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gnhhtvfub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ggawyqdea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gsiozjjpm.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghbikibcc.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gevjdjqdl.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gkwbtqywi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gildvruym.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gjvekempk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gmbjkkwkh.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gsrneehvk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gqwqhturk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gabwapvkd.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gycfovzve.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkjzugmvu.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gfldobywn.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gavifqtwa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gehavypgr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gyxisdvgd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/ghvlxqwhq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gdvpfhjuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gvpfotuqw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gcbbbyces.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gfqjchuai.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gibzvrvqz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gvvndrjyc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gfyfdrndo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/guhnarwjv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtybxxrxe.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gecnlgjvr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxybkcfmz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/guwvbgyog.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmgzlibxi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzavwkqlq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggfrijjhj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcprgvtis.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfhpebxly.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbsvndhvw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/guraxvmlg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grasflybo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gygzfdfcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gabvmunsv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gsjprntqq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gvaepsewf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gxbqjwous.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gzljxfnwn.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmcxpnrge.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gnyikddjx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gmevgbese.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gadgkzslu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gghltjkzg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gzbujumct.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/greyukznh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gtocokdbr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gsndqkckf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/glgcsonhq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/grpypmxdx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/giariwdlu.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/guqqupwgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gazsjgihv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gersrcfor.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/guzojnsdt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxnrcccmq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gibczkbjq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gulpymwmk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/grckmlxey.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsybfgkdw.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gufkpskiy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmjupspnj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gexpemfun.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/glquukiep.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/givmqjlkw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/golgvtgff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gasijikei.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gvyoyyhzt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gjxrbtkrl.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gcsorsrkv.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gklkhcpah.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gnjcaovcv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwjbkclio.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkodvlnzu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gbzqujlpk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/ggyqneacm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gttrngeoe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gshxwwpuv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gchljgxcv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdjtmsvso.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gisdwcrxb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gymffxzlp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gwqpuwhzl.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gczbktguy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gbqqncdix.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gpyptdico.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gnbaoxxav.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gzipohtme.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gmyqmdqsp.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gyywwkiql.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqldxjdah.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnzdsxrck.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbhshagxt.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmmzbrzvc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gmmebuxea.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghfjtpbbo.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gypnqizhi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gkmnwjfkh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gaspbiivj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gmegtvwkj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gozdbvrtd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gybdkfdzh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gyopmcqtx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqbukjnir.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gewifavbl.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/ggtfgnmyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gekpnvjhc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ggfcicqie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gxrjyucay.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gxfcekutf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gfocmjqnc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gkpkrpyln.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gegykzrje.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gxpgnxpwx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gxdvzweet.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gfpvqwopu.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gvmfojlhv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gnlvprybr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gvcmvsljy.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtkxaikna.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnvfvfrwx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gqbmugbep.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggmlueqcw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxduzfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gtfhjfara.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gcmfwhsgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gaikjqkue.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/golpftgwm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjzfahuwz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gdvohewwv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gcwgrujqn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gdcnfdhmp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpxtwyqhj.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/galckupcd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxsenmdmj.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gvnnhkqex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gvuvhxsue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gnewbdjis.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gyvwefabf.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gfxxbznxl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gqevutevt.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gcnjqbtey.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gddxwqshe.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gqlfglweh.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gbrjzctoq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/grjzbtbna.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gvxtnxwvy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/giqmljmvo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gcqlzymlg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gttjufyyb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gzwnelmcx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gnicugium.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gavfmlhqo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ghqtzoiml.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gcvdlmxvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gsbmlmnvu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/ghzeqjcef.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdgszjqej.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/guliouhpe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/glkugpgau.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gbzimghtj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ghvkenhab.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gcigebblr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/givugmqys.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gsqueexjx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gamglixig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzyloqock.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gaejxzodh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gqodysnud.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/glazffvgf.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gxlfiyulj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gwbjdoeqb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gomqoirlk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gjnkqtnef.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gcazecanc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gxfuudqyp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gxsczlgoj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gzcwkejxx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gabkvfyjp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gclurzelp.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gdhlegwbz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gmjjebaqn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gewmkbbky.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gpyautkuk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gurcfqogg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gczrilqqj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gdvvbpaci.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gnbfhqtwt.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gmsxtuobt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxjyfbqxd.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gslguhmth.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gumiyodsv.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gfxxycefi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gadupstno.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/ghfaaxaud.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gchpfdwqd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ghlbbgubm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmqbeudgj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gyjxzcxfl.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gxawablbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gilroiyur.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/goxfdjkqj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gpzhvqypv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbhvrxrsb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gzfjtzzxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gslrbzzgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/glcriikbx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gkemfwslc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gaxeffsmb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gxequtqve.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gybccpmoj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gwnptdtlv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gqejxsfiw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gdiyjdysf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpmjuwolz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/grrihgdjw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gypzoszme.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gmxcfwknw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gbihmrsml.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gftiolufp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gelgpckfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmwudnvuz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghqublzyc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gjztwpufs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gqiyhqjeb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gzvtcrram.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gtaeqbnmh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gbwbmlgbq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gapkewdoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gqavsrnud.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gjqgpgtzj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gsumzfbkp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gmadhnbgi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gegceanqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gqnedqdyu.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gxxxduvfm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gshmjdbrl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gvtgivtov.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/girvampfd.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gyfnplnoo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gsuenznpb.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gjbdxnsgq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gkbdsnrgx.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gmxjqgsex.sHtML


<!-- 参考信息 -->