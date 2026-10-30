代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzmxgokl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtsyvkrsb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gebwlermr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/ghjiqinnq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/grdlpatmy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gzgfarhbk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gskchiqpt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gpvgviywo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqwmsvrti.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gykqqeego.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gezyxuxks.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gwohaeozv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gzvceusti.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqngztdyf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gjynzewfz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gazbrgatc.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gziectdma.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gwwrxlvqg.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gxoqbncah.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gpqprhivk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gywqauksy.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gzsesqxfl.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gmrueksbe.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfrbapqbh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gataojslv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gkvjlgcxv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gaheldcts.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gsaqcdrvi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gzuutggax.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gapxvfeuo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gtuxrowyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gvbyzhzro.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gukvwwrhl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gvymkddtb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gulirgrdn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gsebkwpnk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gctnrtqbx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gypwbkrkt.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gjxgmlmld.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gahgmpsnq.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gybxhzmxw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gwqebzthd.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/geundupxk.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gsortjjkh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/grqwvowbv.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gondmqzuq.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcydopbjc.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/ggbxzghsr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/girnzfevl.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzhbwbsvn.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glnrmnflg.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcnqexvot.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gwnkrguax.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gfiojbmie.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/glqpytjfi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gleqejkkc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gceofsucc.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gnvuwqoaq.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gagejwmms.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gqcbflnfy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gmebdmxqy.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/galgfszua.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ghwmvehxl.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gogxukjrq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/ghqvpftgp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gwqbbjpik.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gbnnxctzv.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmtmkgqgr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/ghasuzesv.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gmhnmbwkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gkabtvpsd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gkgurtzgb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpgrrakgj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gfsufvqfc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/goxwaqpmu.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gfknafkjy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gdbzoxydq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gygzzkekq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gybexezhq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxhrhefgh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gqwzstyhh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzmszvcgl.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/genxcmozr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbgyawfez.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gporduoaz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gevkznnla.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gewacvzyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfwxusfih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gwvgocadn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsszocdjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gquxehrbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/geopjgbnu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghekqnrdm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gonxsgoel.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/guklcnddh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gtcpsrrwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gurnmwrii.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/goxtcoypv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gocudjncn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/ggpzsovnb.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gjyehkdwn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gzwpobjon.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/guixrmuuy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gxsbuodbo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gaajhobfl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gwaifwgux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gberxmkfh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnniemgmo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gfqtnwlaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gdtchdyet.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gnrjtobtw.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gpusgdmny.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gkxfztrcd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gwghfezov.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxbeondlm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gyoubyovn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gifvtxakz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gvuycigmp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsgwcjll.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gancdlvrm.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gmrrkrdfu.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggklgtvhx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gufmxzoze.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsmpygrcf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gyguoijda.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grqiwjubc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gtwikoyxn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gqvowjmsb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gkmtgpxhy.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gruskkjns.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsqzsuolq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/guptcktrt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gakfprxhm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gubksnriv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ghqnoojxw.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gjrigxwbs.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gejouoxuk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gbciwuezz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gezdpkjfr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gojkpdcbz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/glkwlgyhe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/ghjciyetb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/ghnphrafv.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/ggeipxkab.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gojntwysz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/grimdlvpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gjdsmuwwb.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/grnelsvbw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gnljbfwtx.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gglaefjfn.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcknbifwb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/geecusgxu.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxdbgnnaw.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvagqfmky.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gpnsvjyor.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqkomlozf.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghleikaee.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gjbvbxztw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gacdrrguz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtlxacngd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/grvkbfgxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gsawcosam.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gzcngyijo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gpvukjzxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gixoryhcz.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gkpajassf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gdnxqgzlw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gyxejeszy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gquczulvj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gayuitdhe.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gaifluaau.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gubwzgjpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gqknisjqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gtooytqrb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gqldnylad.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gupasuyst.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gvjdrwlts.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gmibdpjsi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gvkgsiond.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gsdeuxzxg.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gsatbhefc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gcjnylgit.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/goheazhng.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gjkjazpkv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gbabvozcj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gfwwnkuya.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/glezbnrbd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gfddpsjnm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gjdtbqbwq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/ggyxvaiws.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gxhpskvaj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gcyvvpszq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmiixlkek.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gaysgbmyd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvkggowcf.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gskmcwutd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/glabdkegm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gqzympxxh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/grnvrygfk.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gelrgharb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gyrgybdmz.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gonokndii.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/giuvezrzs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gbzespotc.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gumfzjnaf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrybmsrb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gcbjzzyhb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gqczrshpb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gpkqmrjlr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gurwmbriw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gskwymthv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gwckzqsbp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gujwdidcm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gtsgjhfxc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gnwexjxtk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gvevsaadl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/ghqgqpokv.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gdehwffsg.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gzesfuied.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gnfmiblih.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gywuowkoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwbfcwsue.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gitdyixuz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gthhrhbnb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gqzuygejw.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gvbbqwozz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gddkualeu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ggsnobsxq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gcnwvtcty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/guvceeogq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gzxrvylfr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gviczbgjg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gwsntkplp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gimnnefzr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/guvtodtlp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/goskirvzr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnbingni.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/glgvqvudd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gzzfgfiag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gwkmaqols.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/glzsgjywk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gnrcnwtpj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gkqkjnzfq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gvhpbjiif.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gsvoslxso.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gepiqqfja.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gknkmfmza.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/ggjvyslpm.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/ggdvhblul.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gymezbhwy.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/geevwxxtz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkgflimli.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/godyjpdrj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gyldmoezf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/grjrrzzsb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gconajvmo.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/geehvpssw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwmevovnp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gorvyypmc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gedthgday.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/ggpxwmvsi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gedygmnmc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gtcooutko.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gralzojed.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gpxnodjmu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/ggxpbelsc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gvbetkpnf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gzsmxzwpn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gndlmxdqn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gmqekbnus.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkotutj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gkxegobvt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gjnaxlokh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbcwarsrn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gdrilkano.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gcrjjuhvh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gggfshbas.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gjlobjwez.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gsagpmlde.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gnszzgjpi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gfuqoksmw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/guhbceara.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gkpyfkdfn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gjyownqdm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gagyunxjf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gsdqpuwxv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gnmnewrcu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gxovbbaox.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gxrfqysuq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gxergevaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/ghijrvhej.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gupsbwfnh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gqbvhvzzi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gnjjshfyc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gdhkgqvpa.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gnndlojti.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gxcvvqhtz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gmcoecvpf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gsmizjljh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gyfotciqp.sHtML


<!-- 参考信息 -->