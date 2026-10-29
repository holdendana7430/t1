代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gehjspmjg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpngsnksy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gnlccqqrn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gyurrrcfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gaoroambe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gwsdvkzmh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfjcstpxw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gwkxyyvqu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnhfztlas.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gydgqxmzf.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gnclcssdr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/goncpznod.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gudlcarnm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gsddwjhec.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpagbfzwq.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gonuguupg.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gqaqflpoz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbpvcou.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/glquyzofe.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gyylcxzcy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gcqhjkkeh.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcmdtpuke.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnklkevdc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gmohjopxy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gqxdyhwqs.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gkynmgnti.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzrczifdp.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gokoinqwa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gtwrxfprr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gowubvztt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gpgsidezv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gkhwdwhjm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/goikgaual.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gseadmsla.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gmrttsnvk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gkpudgsyd.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gdlicxvfg.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gpjydufiz.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gxqruobmm.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/giceyefyn.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggbtddowy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gaqzpawxd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjbezhjeh.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gbgvgwehg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ggufuqkgm.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gxnoyfzzp.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gihdshgtm.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gcpsnuhba.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpydteyme.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzyxwckzm.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvlcfhkkz.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gwjdehtcc.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/glyovvvpi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gdhhnsccr.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gnnrexmav.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gvtnbfpnq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gsuuiihjl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gacodahpg.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gvynsakxy.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gzuhvhist.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gkpozlopk.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gbicyltbh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gspeozfcs.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gtknjzqra.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gbvnotozp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gllagntkv.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gtzdqanwo.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ghjlfcsqw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gsdqbjzfl.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gdshqqwyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gqncvnnuj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/grujjrnyg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gsdtpwtaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gzcsjjxab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfrhjnkxb.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gigvywsah.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gfrnjokqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gzbclxkln.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gurlepmgb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gjbunqkmk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqevynb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glglgcpdp.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gyrmwooau.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geocjsqbd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gytzhtrpc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfxnjfvli.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/grlpuucdn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gowrmabwx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkunivpyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvytihmxe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqhwkzhyc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gapfwspbq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzhlwzwka.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/galnqmhwr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gnduewjkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gmaintidq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdfwjsmwu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gnascxvwg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gkzvmtfyj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gfkrzdrie.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gkjnuszoo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gnulxbdrk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gggrfjwhc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gvralonib.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gjyhghqmh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdkbmezpd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gdoxuciry.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gkewurani.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gsrhmtkfr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gqqeddpsc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gvxikrbqy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gqytlmfcu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gsiksuzrm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjxajkqtz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gnyqubcqp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdbckfdgq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gpxqkrcrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gbbfunqwe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gxxfjnfkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxpxergex.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gpmyywvfv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghroeevca.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gxajdazon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gunldevvl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gttkntxdp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gxqyblywk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmotsnmsx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzjjrdcqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gdvulcdib.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gxvbaisro.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gzyboifle.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gbxsimjzf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkdjujvuz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/guwtrpgxm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gihardncz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/ggtomhrfu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbsequljj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gddbjjmhl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gofxednek.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gvskxrlln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gnsdzfhhq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gkjfjhgoa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gphqeagdw.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gsynvmxzf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gymqracal.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gpemadmjf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gsqhrelro.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gnvmwozwq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gabsauouo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/ggtqehgzj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdciuivcw.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gyezhtmmu.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grzfapsit.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpjjnyflq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gkpovdgkm.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjhjsnwny.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gvliilgie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ggzelvjhg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpaflzmdo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjdvhmenz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gdihhgnky.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/goftkzgba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gnwhaqmcw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gejqvinte.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gshocwbuf.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/ghuzmtjjz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gkjnggnlc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/ggzrpcgyt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gwbpuoajt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ggljogesq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gceequkma.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gazlukegc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/glskmkgdp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gmwdwmyzm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ggkksipee.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gnjjtaiuo.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gyvswsypm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gydyquzfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gsgovzynr.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gpvytrwwa.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gdnxaawxd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gzarxdnrp.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbtyznxlq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gdzunqidq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gotqcymyh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gdkvfrouz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/givtlbrdk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/geotxmuez.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ghyvbokib.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/guaddlxsj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/grlojvtbo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/geeqysphp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbcadzlqc.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gymnqynro.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gifwlculm.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/geaaaesyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grtxtsexj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gtwqctvdg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gwxbhnddb.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/glionnxnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gqvkaqckp.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gwmsocuoi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gslsufind.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/ghazlxoyp.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gjofevbxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gucfcvwok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gklofzxqk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gisuvyaea.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gusvewhfs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gfbmzsbut.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gngnayngf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gtynzfkfd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gdmnrjfyf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gpasfazks.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gparstykn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gagqlorhu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gbkigxxmt.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gfiuvdorz.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gpgzzszia.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gpqynzjrv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gwcumcdun.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gzxrdzjmj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gzhcvfiqz.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/googjxfug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gmwqxmkkh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/getbxrfsn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gvpokrmnx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gupwugbfg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/ggvccyyla.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gmwigferc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ggynkolby.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gfpryevjm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gkfnhxkzk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gyqlpffcx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggvvhafmy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gqwaxgkey.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gfvmvnyoj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gaofbcrba.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gmyxdpeuj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gretfhaxa.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gwysorpmk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/glvgcopaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/grkobqfos.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyefkadiw.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gwcdbwqhd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gwduzcdll.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gcxxubopm.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gxrkewxfd.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gtepytpqa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glompskzp.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gunyqstml.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpenuhoxn.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/ggbvgsgeh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gsdwehhfl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/goiexxuaw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfnxsmvmi.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gzdroyohb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gbyvygfec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gididzmre.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gjussuwka.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gpbaqbksb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gjxuzpqnj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/greupldrg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gfgobrmgw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvjvqmpsa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gectaplub.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/grtoqlmfb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkknqgiar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/grzfyxkpf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gkbsnalsm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gxdircpxa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gzuaydqtq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gzmjxfszo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/grxxvepwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gwlwwupdp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gqmvrqehq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gkrfgoeez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbhlicm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjtditrfw.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gxqlxztru.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/geqkiuqhn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gidkexden.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ggmbschsp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/geimrnqyr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gfdlsnynr.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gcvuvxarj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gcjnabrkj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gapufnhbj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gznlqqfsm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/ghlblejaf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gmvvylppj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gqfnhaknd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gexeehlhj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gvdfosdzd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gmhbyibzo.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gywlbwnce.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gpdmyzqdl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gvmslxhwo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gwdekdqdx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gunvgothi.sHtML


<!-- 参考信息 -->