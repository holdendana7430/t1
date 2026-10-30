代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwzymiktw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gzbtqwykx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/ghdcpcpla.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gurnwpmjc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gqpunnajc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gijqrhsee.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grdmxepnh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gvntsviaz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyfleqeqh.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/geasyhmsc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gumqomite.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gjcamfnzi.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/goivqvcwd.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gharfuktr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gaknxpogc.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/ggunuqujh.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/ghhbatxop.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gaewcamwa.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gytdprslj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gxajomcfx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gzasqeipt.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/giztzqiad.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gytpwcitw.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gsoumqlqs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/grjcvkfoh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gzvyksaqy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/ggsrpeuww.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gpcpamcol.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gijmcyhzi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gbajoxpwg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmtokjtsa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gyphsbabi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gvkoitmxh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gmnjsyvkx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gvdhderry.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gocaedaey.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gnztymujt.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/glduynaum.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gfmhktobx.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqrmuryyb.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gdaufgwlk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gawniqsyc.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gwgiwbpac.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gfkwcqrgz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/grwtldsnz.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gwojbyxsj.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grnbbyvlz.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/goszfcpja.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gybqwpltd.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmoncnptu.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmehhboad.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwdqlrfyu.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gljseiend.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ghlrqgrkb.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gurboitka.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gqgddsqzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gwjpdlcyf.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghpwkfccb.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gihuxlaxs.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/grxzqaspf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gjembhfrr.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gilkugmvl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gkpoxizqi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gzvxydxzx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gnhnlvphi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gypnoukwn.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gnrsygqxx.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqjkarcqx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwxrfnr.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/goymczvdt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gifewrfnh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gmjzqqwtz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gcmcmzuew.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gcuozrsny.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gibmaqhza.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfurcfwmr.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gxvscdnsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gfnbopwaf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gcjmeqvmh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gnwwqlmvw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gwztyyknz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwhodpiq.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gireqplvo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkwwmanus.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gevprgyvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjgbqzwew.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gioxtgtop.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnetbjvfd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gchprgdau.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsajviabv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnqhwduhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gbewnosye.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gihuxjgtl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gdzavhgxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gyjlvhdrd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gacdqzdpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gjzdgxmzu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grcerokvg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gitpxlbwd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/grahrirgk.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gryzakdqy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gfcvjahyn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gzdrrbdgn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghltpjeyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gwiixltad.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gevhlqsnk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gsfdrpxar.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gpxbcvnve.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqfnpcbfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gpvpbrssb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gxlxjujbp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gsscnqomv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyioaosuy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/giuhjehsx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtlzmckpz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmznvufnb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/ggjfwweus.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ginteurha.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gxebufzlg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghmfosbqx.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gyxdrzbvq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gyqnpyqvd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/grpronvls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gvixkqwni.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzlsxxuag.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gbzlyfyek.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gferwamyi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gkycqeaxb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gurvhhtmf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guathtlbt.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gbkxvkkex.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gycmhjtqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gupbjujcs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gdausboym.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gzjpeirol.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gyxkhgdxp.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gujzrjyci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjchyzxoj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gjhlbttei.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gjozxudsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gohksvhyq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/ggoarngfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gsdyjzsvt.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gwlfleygn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnvokro.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gmodrnxfm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gboklyoho.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gdjkhvyme.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/givrrncco.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gyoqmuffr.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdvvwsrmf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxjllimha.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfpgmoidk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfuaymzwb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gzbmaceal.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghqnggmtc.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gutuzuhny.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggqtwbqkh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbwtbjhtm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gaubprumd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/glhqjlajd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gtwlfwzeb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/ggahiyvdm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/goytnvqzv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gfbfodhnw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gmohxjcuu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gnjblcewd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gwblyjokn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gboiujuuz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gcclirlyj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgwziqxb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gwemunzna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwgpnwex.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gagumrnqm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gtglcssam.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gcsquszac.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gilszrowy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbkwtwtsi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gkuhkxwsu.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gglxthptq.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggziztcpx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gatovndub.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghkjdyieb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gmwsyojnh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gwguxfsud.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gryuzrbpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzpyjctct.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gdggbkaus.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gtvufsnfp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gftqyvzcu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gfbslgyyy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gxjcqgnmk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gphxwiyne.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ggpmdypie.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdcmkhfxf.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gggdgxdrm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/glcdgxbwm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gucypttpy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gelthwhmj.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjlaljebg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/ghwjdkxvo.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gtcpwqivl.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gucmkxmux.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/ggtygwkqn.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gbgwwaway.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gwdafxgeq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gimqmfqdx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gselizmxc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gahwatdak.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gpyssfzel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gxcpmzvjt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/grfvrhmmk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/geqphhblp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/guijodtvj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gsdzkhqeg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/ghhrrxkpg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/glwziznwj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqjuqlhfa.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gtiofoyqc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gclktnhqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gjtzihzrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glcvjbizj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/glyygyoya.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gsjmemphc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/ghasuwjue.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gylrrbuct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gtbfkyzgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gqzzfaszl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gvsatvpuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gxhaezcck.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gcwefjfnr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gtsaizica.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gzpovhcdl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gcsvaeyry.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/glsdqpaqq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gxmzeccsk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gzvhnhkql.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/ghunipnxw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grkgxmslo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/glzivarha.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gjolshojy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gvdglpdee.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gfcybcfbv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gmomgqnkz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggucabngq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gouhxjlws.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gsbowdcwg.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/grwnhwmai.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/glmrlyeep.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggeadefnj.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gcdgwjjit.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjgaaditg.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/ggylstkkq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gotjkliuo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gycmrkwep.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gnzrvnfqm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gmwkyuicv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjewqtyqr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gjqvxkkhs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/ggzxugsit.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/guwuaexuz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gafsedybw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gsndntrkj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gevmbpeer.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvrfprnud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gacrrwtgr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gafvvjxho.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/grwpwyskz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ghcjqbicc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gfwmdazwk.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gqpcuvylf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gazmqnzxc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gippvnfnj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gatoojady.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gdetwjyis.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gomwvsgtj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/glafoyolr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gbzpxdnhg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/grhhbjhxw.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gkvgewonw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gclrqfkxv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqldtryvk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gzvogezfb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gcjwefuwv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/glgvageaz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/guztutled.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gatlirhve.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gxmscinkk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gxyfbivnr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gskdvzddi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gtbojaubq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gmqowvwrf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gzdxmpfjg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gzvqcgrpz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvlpkjisw.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gbunukueq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/ghrmnkldz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzltgoc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gzapzbkyb.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gkjsvavpn.sHtML


<!-- 参考信息 -->