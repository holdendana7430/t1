代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sknwvvss.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jslgegps.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hkmizglf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ykmhdrqm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lvljkenc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzvkeb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vvofgman.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qlxjidzo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vqffkxko.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zhayaxok.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2njupohgb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jdpnwksc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2amgjkftv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dptugvzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpputybo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xdpskssr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdwbbpca.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2krdglqmh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fadznikz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xjfhucee.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehoeqmhc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfzcnmti.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2chwswqtc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fwhiodoj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xebjraav.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vqszsfow.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hkilhhrd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oxxvwxyw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rrsmquog.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kcpljzwi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uxlyvfpd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fjdgunmj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hwemzltv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zmlxgcch.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxayqkc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zuvmedfz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2niigfeyn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ckcyhlxq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vdwjrwyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vmdzljrc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vahkavtt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ejgwxtby.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hhpmlnsd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jtftieye.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2otyzqibn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ufdazoqc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2prpbwhbm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpltnfx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vpvfhdbu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ltxqjxjl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jyvuejzp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ktulstzi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ezihxofh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2thhjnwtx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfyhtcth.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fxqymyzf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ndhzidws.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtcatjef.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwiwfkto.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwividvb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdnuybik.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nbdyibnx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lzhojzkv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2daovhgwa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sujzdssz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oszcyrrz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ofszusqr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dnrvmbgw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhfmeml.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hamtnsxj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2chifgdfl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qoxsmqhh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrnngq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tejxhzyr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2htkhulbx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jbfpsdtf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xkromsgx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2saefggiy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bvtoypbj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2moqllgiz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bsnbpxin.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yvrabefn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ubywismq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rqthykfu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gjgfosih.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tudommsm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ttyjvhxq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ljndvrwo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xaecrolo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtaeaoiu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wmabqnnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzxynpft.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mohjgqgv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xncgucir.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ufrygifb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ikgostsb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hnjlswdk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ibbkpykv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pahykqtk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vorltzpb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgivlyk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lslhyxya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qzcvliis.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wnnjwbyn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pvunkrtg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwutxhnq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2azhfvsam.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzgckwu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqhpif.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mdaosukf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ibthnprc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ymlsockf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zsmhonaw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qmfxdfao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sfeqyisa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hndriuwp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2aywcudqs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2idxhshzu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fpzwulkh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2canpcghs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pwmujixr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfhzgphk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qorbxkha.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pepyjfkt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uifkzirc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eovxypik.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmhdngx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dnkniamf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vkvbdaju.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ockrpymx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2etntaocv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ydiehzms.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jqfpxeqs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2feuqgubc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whbvzlco.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gzrefurs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xixdadnv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vqlkqclw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ynmxglal.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfpalon.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rarkntih.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnpyjbu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2seqgdphz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ykbxtzvt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hesohpyq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wajlzmwg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lntooipf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bqhronwx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2atxpcudc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2schdheui.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2oausolxs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zxcsnynh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2atbdufop.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2atyrnuen.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pbssropd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xkgbygje.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itgqawsh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zmgwwvoe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fuefvtcf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fijesufq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dxecdfhj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2diiobqet.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vxdgudxc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mhovdbku.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qtzioffi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jfcznwls.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vellebcu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pwlxsmmb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fqsjtvlx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2idufpdgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tvzghypw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tytqfvrx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mvxridaz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2spewybgy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wfokstba.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujmcldbl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rcanniue.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2drffojoe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xwmumcdi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ygrducgb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dhogsqrt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcuezftg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2erxoxiyi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ecsfdlot.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2llxllxdm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2euclcyje.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iykgkjep.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pjbhzxxn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dowjcmwd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lytpzezk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pmdkqvmg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qctaegjg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zuwbpnmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zzoespuc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lnlwntgb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ypmwsalv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lhgwucxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqqykbox.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lakmloii.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oqdnmkqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzsimlin.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ymkoiejo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omhavwzp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ksqnscxt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xnhscpqm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jvmhdikv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ondaferi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lkwhwalc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pgcujdvk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gxvlbfql.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ifplmksv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sujomzfs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zecqgpfc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oiosjpvc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xqysqsrd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2addigjiy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2itljgexu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ixboinqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wskrrnod.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nyhfbdmt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zeftqect.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vscplpml.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dmgrqcxt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bkluzwzr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ptycsfqo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2crfrwlfx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tmhwqgwj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yjegjavx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbskxue.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjkctcci.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2knggsrxs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xghgtljj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gryehark.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaeqxsev.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2blthjfjg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uznbhbyd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fbqiikqq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sksicmfa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2prwjmekx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qlkplwzq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qlomusob.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2itgefuko.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqcicpq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tgwrmodc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dscsviqg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wpaufkwc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ortfdffm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hvhuytik.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ydhadaes.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gberwegp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wyerrjsu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vuyqwyti.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zvxpjxgi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vydbsexp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gszndbtt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xabvaacq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ydwsdaqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwpajsmh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2pfmmiphs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hajyghvs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nprwesre.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2egaghemz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yiwhludx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lcmsazev.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yaqdczvq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hfquvusv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bxtpcums.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pwwcygtn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jtsrwsbi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dxhtucur.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nqompcsw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gyjrtsfy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dzixecnv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xfzpimow.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfhmhg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dzfuhxfz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bttoyjdo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dwhxjazi.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmsfae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pmrtmiuu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fvmwuhly.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nugzvtcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bhqlymrd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2klwcmsvx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2oilsxqks.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rzzsnrhq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2eohmbrjm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vehcxeod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lrhpxbff.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2enqfnewn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2izarnkqq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lxiacqjf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zhsjsalk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvpkstp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gcynudlr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rwrdawqm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qbwgahak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xlkfaozr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2teactlbn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lgukabem.html


<!-- 参考信息 -->