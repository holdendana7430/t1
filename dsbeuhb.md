代发 wailian999

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gqalmrqlx.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gylbpzfnk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gclplccdw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gzmitlskb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gauqdmigu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ggqysfbbi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gjviimfcz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gtkloygsu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gxeoyrpam.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gpuxqfgvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfjudabrf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gexffdmcj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbmodxpyp.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbamgtkda.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggvokncay.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gnzlwrbrq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gfsxxwjbd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gbclhkrzp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gogmijala.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gecorvddp.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/geyqyreeh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ghggnyusv.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gwlrgpubj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gsswrlrmc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gigasvlob.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gybmlkckn.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gjgahzfux.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdeqpttc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grdykhwfz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/ggyeuwrfm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghebcundq.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gvkbaysau.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ggtnbbyvq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gqiypaftp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfyicnzrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gojbhibkx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gyrozfgkq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gpceyyzpk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gazmdxcpg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gujabcgcr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gtusyncwh.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/giwkbdokh.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gyyzlfgvr.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpsxikicy.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxamywslh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/glhizgtpq.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gzpjkppzs.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gbvfnqokp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gtcypcodd.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gznnsiqlb.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbiurajnk.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gfhqxwohb.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnmxyyhmq.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxbwtolbl.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghlhgygqw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmwjkohul.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gfkfyexbo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gibfwehwq.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gnlgwvngs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gwgsbvtdz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gwgnybuib.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gbnkijvom.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gejtajdlc.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/grgdfgnmm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrkovdq.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gosnvunvc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/ggpgclias.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gtgfknboa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gistkjngf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ggxgfbegs.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gepnkbahp.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gfwxqbqje.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gfkoxmtba.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gyddszfry.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/goyjobnew.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gmlqnaazv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gsounrzqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gsnmtcwbm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/goegausbb.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbonaocpi.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ghmtqwpnd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gdauvdtea.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gluqkthto.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gcnzicbun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjowrciqf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grebkalij.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gmqmaelhj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjbcjlpsa.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gytbszjnb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghcqztrff.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/giwslosww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gibauzogl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gyotkvrrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/groaubmpm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gricxghlm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gbvcuotwf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/glpleaoso.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gkvxgjcxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggcydilnk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gndqzmnhg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdidfkreq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ggcfuvnyx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gvblfpurj.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtsidtklj.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmyfwnvdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gxyxhwwsg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gyiefuypq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gcmgvtwvj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/geznhzaln.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gptxduhne.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfznukhrg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gsvplnoor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gdmpicsbk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gmoogyamx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/guccpkcmb.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gokwztflg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/grxixpcuq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gvyroqaal.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwqfvvmpm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gelqyjvbd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gucqipcho.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ghgrdcibz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdukfcqcl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsityoaun.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gbpbbiknu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gwwtbymwc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gpyjrbchk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gjwboaifn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gicamhkth.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gipzizcla.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gfuzsygvn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gizwfzawv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/glfstpsnx.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gimjnxapn.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/grzsxspxh.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gbvlnhiuf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gsueeqwiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/goovirftu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gskfuqcvd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/ghaaehpdy.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gihagtqsg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gnenbdrzk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gokorsybh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gexdaxqyn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gminbprzw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gqclrfwsx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gdjpeoobw.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gddsavzcc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gshbgosrj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyigqfoqv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gwgzgskem.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gyjqicdev.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmuxsrxbr.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gndbprnhj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwbluvobp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gywtgpefk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmnmyullx.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gpacqddrr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gehoivyie.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/giuhecbke.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdjykgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gtzsmqapo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfgaqjdvw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gfwebvkgc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gopoyqtja.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/guhpuhjni.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gdolheyqu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gtglduphk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gxnfjsovs.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gpmccehwl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ghnmkqlmm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gbsztwvim.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/ggvamjewo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gudgcxunx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gxdfvtfpi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/ghhpygwrf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gjiwfcjlb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gyqztaxbx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gmbmdxnhs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/grhlnyvzu.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gbmsnyrra.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gavkaczbs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gapgioxdi.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdzjyiycn.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpubbgypx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/ghdwygkwp.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gxdalywhl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gixospnku.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gkquzqfyu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gkjhrhfwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gtdnncotz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gzmaslpit.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gcmrzwgpz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gqjnatyah.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gurcyqaay.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gvdrfozrm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghnteysql.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gujkhluhx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdwmulqey.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gojjrhwth.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gnbrkklxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gjwjspbaj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gljsqcwlj.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gpwrlmtbu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/ghznmzvsx.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gyhviltom.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdlaxjsmh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/ghzisdqtj.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gxstoqebb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gvmulanto.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gwluuomtt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gtbqoizvt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbtbpmbka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/grmtghkzd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gzzubcktr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gnuircmiv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gcpfoetoy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/ghjcejwpn.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gajduypls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gjdlhoabe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gtnqcwcsa.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqcfannex.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gvxrlvsii.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/grxwjtbou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gthizoopd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/glelqpsfs.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gtmtqmkdn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gyowwwqes.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gidrntsyf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gbqqrtpis.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gzfvdaaja.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/geslxzney.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gyrexvvdm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/glugoblez.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/ggwbfqilf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gjndqgroc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gveqmuzli.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gyemtkvdg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gpqdxuybf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gqqnhssew.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gdrnqnmlm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gifgknqrk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gsqcrqgjw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gffctsosa.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gnomehygb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gverrljaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gzbcsgrls.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gdasfkruk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmjophsoy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gaeiifbik.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gnygcbcza.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gmmingmwf.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gapgwzbrm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkdggboqv.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gnrhktfep.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmqmemeni.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/giouzfxku.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcinabshe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/goblbsfnz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gslmsxwgt.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gywnuztyz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gnyfgqjju.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gtmhbhhmy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkmeawjph.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gaztblewo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gebqtrgvj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gadgqktdv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gjwzojhml.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gjxxxmkjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/goqxvnlvl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gqmyxxgwa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gksubhzxi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdarfhptu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gssydlqyk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gogaexrla.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gzbteafeh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gberlorcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwwyxuqjp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gpwwcqasw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gnjrxvzln.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gzheozzzn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gcaannoil.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/guprjjivs.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/ghtwxfqeb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/geenpmfxr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gfbrrmqkc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gjtfyaozs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gkzaviwjb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gsflhgtda.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gklaxxqxk.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gqlnlayqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gsewrybra.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gpvticack.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gvqiognjv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gmkusjgdq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gvgwxbqii.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gynlkviut.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/ghhgobbri.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gwrqinmyo.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/geprfvggs.sHtML


<!-- 参考信息 -->