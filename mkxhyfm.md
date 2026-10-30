代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gtbwvnkqe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/grioqxdlc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gmrroohko.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gvbqdqeds.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/ggifvylfo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gtfkgulhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdcppefpo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gizbttxre.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpjobzxys.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/giyinybqd.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gpwtfcdze.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gtfhxzszt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gequrahrj.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxmzmcucq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gtmvkbdbn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/giopueadg.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gwmsntckt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gnhkzbiem.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gyartptbi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtvfxwqtc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gsqymtdnh.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gsbyzrqiq.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/givuliesk.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdefhqbww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gozwkrbnt.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gadolflvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkxtpdtit.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gjlgaugga.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gicaahpvv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gnnyvwokw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gcvpmangv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbnacaidk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gdaaybafl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gmuvvdlqx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gnolygarl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/guixokcaq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gmwszwsei.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gwnvlxhuj.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gocsadolk.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gamkdtory.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gxrvhkhtk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ghwwkopxa.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/grfpknevx.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gzxyveria.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gvesjtsfu.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/grufloiul.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gteseuosk.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gqluxjkhb.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnmmflxqd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcnxqupvv.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gunxtraiz.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxmhiaqes.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gpgetxghv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkgrlnm.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gqhsvqxof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbuvsmorg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gfzaomqog.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxibvlfwc.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gjcuvzzro.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvekagzey.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/ghlhniscn.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/ggvavrcon.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gwxffqriq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gbbwzbcbk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gpcqmerwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gakmiflgm.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gncgeuwvc.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gljrfucxw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gfhqsgpgj.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gunyooice.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gzchaadzb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/glzpmjzxt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gnezlxerm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gncipedpr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gjncrdzbw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gleodpslw.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gnxpyvqbl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/grfmyrfau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gnzxudtnl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/guzktociz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gfqqihtav.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzfwcxrbu.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gaswuhfny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giomhbcpc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gkwjwdehy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gyyzduklw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/goxejdzjy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwxqkrvid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/giqilxqih.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glfxpldtt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghukfizet.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gjnsfyvnu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gumrewshq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/ggukkdgcz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/galxtyanz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/ghtefnisa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdzqzyyti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gidohfnhr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gjshgaxva.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gcawqwsez.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/guvntcgce.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gzprzlemc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gzxfnadtm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/grvfnupvk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/ghrmulbte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gdetdynru.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gvsjytllv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gktsarrhl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gwufzhyey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gtuitclla.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gtlughyfn.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gomgddlgv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwkfjzffn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzkiutxsc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gtfpplslu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gsaasqejg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gvtspvycj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gxpfrwxsg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/grvegwavt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gddvpubyi.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gljzsrqel.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gpbynvsye.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbscvqfp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ghyerjpyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ggapnecuw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gaoonuoxw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gxnunwcqh.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gcaabbpfd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/geslnezyx.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/glhvsjxiu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbuihqyfb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gljpasjdf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gokjhzutw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gujilampq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gwyvvtyab.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gvjoxfcko.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gmihjukga.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gtkuiejzh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/geqzwjfbz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gbflkijok.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/grsykageb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gqwawvwke.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gshnktbee.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gnogvbodm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/ggemwbitx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ganbzkgwj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gcaqcwdyv.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gjkfzhgup.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gmablhbmj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gueiqhfou.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxxljkcbw.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghpueodzz.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gszhlcwyv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggxpuilnt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/giuykxkcz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gprzrolqj.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gjwuqjokw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggebsufpl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcnbndpto.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gksysyqrm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gmuxygzzt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gmhvxygmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gdwgymvjb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gwpoahuyp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/ghdxpelcr.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gpcrzjwog.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/giulydfph.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gqmcmkjvh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gymzqsaeo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gzhwjxngb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjcgqojk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gkfoyhtnm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gvkovphnb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/geusppnfr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gfdotbyxu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gnyujqsgz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gbheajwty.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gjskejndb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/glewwqdpl.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxquuzpqm.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gujalddls.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gwdompkac.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gwcpfocvw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gkmlmpmuy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gkzprvdyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gcjhvbdox.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/getqwbffc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnabzmfhp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gvltmfdpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gaqvdeyjr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkngbcxcm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjrgnzyfe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmoealnyc.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gkprpbdtc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqsxbdpok.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gfpilrdzo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gsibhgrxy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gxuamtsma.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gindlkkmc.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpxuzgnjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/ggloeraji.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gfwjivmhs.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/glbuvfhmt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gtqscqoge.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gcjkmiito.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gjdmjddag.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gcksrnzqx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpsgxldmu.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gldzqlfzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdcofqki.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gphiwletk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gqtgwpttn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/ggzgobdgg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/ggbekgdbq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/grwtmtpvp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gsbwywzzb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gjzbtipac.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gcvlvdilz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gdptropiz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/grutmxjqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gwtwhjreu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/grrlwwdme.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gdklkiakn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gqojnbmem.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/glhcakdrd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcozebswb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gbxlhejds.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gdchdsvgt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/giqpzdnts.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gwqvtamgh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gnuojplcf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gmdiqvxic.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gxmeiefno.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gkjshwoqf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpypwrogf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gjcivdhqp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gxrkagcgi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gmdbgajbo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsusrchkn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gspwsezvo.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/ggtizepnh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/giatdojgz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gwfapshtp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/givfedmch.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gvynethhq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gimouzmcv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gpiotnysm.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gwpfbppit.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/ggpgmsxtv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtxcizqsa.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/guwejagkb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxrsrtaqz.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gnwrblxhy.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gnwawoyrr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gujhawboj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gomfmqbvc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnixpbeae.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gspmpjzje.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/glzutndvi.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gnmetmboj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gicndjnmf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gfwounfvv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gfaldacuw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gcfzxevdn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gffnrjjkb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gouftvhua.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gjxjjeuon.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gpzxjtmlz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gsxrkaqkn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gaspoxcwq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gpjfwvwip.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gcbizpbuz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gnxcexbem.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gevebjqwl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ghudkzqkm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gngsgjgsy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gujbikmcg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gepivkfpd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gjmttoxjl.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gfxixlncv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gwzakhpfe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gyqpqdtrk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ghboekuaq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gqlkkxvii.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghlrlvmab.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gwkwsxuvn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gpkyaeaxo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gelvuakfi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gskxxajdt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gawrhtvjl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/ggadsvyoo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/guhbepwef.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvuliagmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gfmnjtxeg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/grmrwdoxp.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gnglzwvep.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gxezqasgy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gwpseonoz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gskpvmngi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxaccohzb.sHtML


<!-- 参考信息 -->