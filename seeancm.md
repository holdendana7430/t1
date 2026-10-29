代发 wailian999

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gpkuwdedl.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/glhbwfrkl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/glindburm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gbiqlnbeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gbyoxjquw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggkufrrbc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/goppeophq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gptbcbszo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gxcnkiqzt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gecwhzttd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gutpcjonf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gbaqrprjz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrgqifbi.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/ghodjhlah.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gonnhlusr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gykpkofog.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gehckqxkm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gvzsgouli.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/guitghvfn.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gxfurebzn.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gqmvgnmxr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gmxnqbcbm.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gkqmpombr.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmbthutju.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gxtiamxve.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gejtdccol.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gpawdjzcn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gtnyryqpw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcvgwvvuy.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/guvjizdcw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gypyoxkgy.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gjgapacfk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gjmlvantt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gqdeagppr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gtjjaqvrm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gikicajyf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gtmumbjtk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gvomaxwzz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/ghrvlzwzj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gppzvzkda.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gsfkgqosv.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gfjhbhicb.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gtezgugjf.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gmxlnbekn.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwffbjpjk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gkzjwpwqq.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/ggexnhiqo.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/girvkdebo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gvehsvffc.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gdflbyedq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsfmnwoxi.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gwccdezou.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/guofzccoc.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqjtwcagk.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzcdqipvp.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gikkzvlbe.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/giclhnzzp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gyrbpwxws.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gsvtmpdqv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gxregosqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gpkjlgqpy.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gxtbwqucr.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gwknzdqky.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/ghpeotcxh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gebcobhuu.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gkaysbaqf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfwftuaet.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gjkspprok.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gakrozdew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gzxcsjnyd.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyestfokg.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gmrdaqkmq.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/grgowybdh.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gjjzljztj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gvvuuemdl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gtsrcyila.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/ggofrwvhr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmahairg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gcbmrqzsg.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gsrheoivi.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/giqopigzy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gbiyghzgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gmkacstya.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gmwzdabet.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gclmzuwkv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjrckiyqx.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/grcpyjttz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gebbrszdj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/guthfkfih.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvlgshvuy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxpavquuy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gnfdriasf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gcmbiubhl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcvevvczu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grmaqyhua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gdtcydhlz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvtnytvnz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gajmzlprz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gpvvboors.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gakpjihpe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfbudpepb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ggxjpfuhk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gbpnipbfy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/goqadpbbu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gokuvxarl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gzfgabpdv.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gkpfirmer.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gnkjmczxx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ggqapipmd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghushcrgr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gabzvztho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gnxlaznus.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gpboimjfh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gsrkdcoir.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gtgtrmszz.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/geenqhzek.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gxhvfnhlk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gylsirtec.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gacfgnvuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gqbddpwul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggbxsaoet.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gkgrunszj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gkznjyvne.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvukhwnfx.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gejgrvejz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzwfanssy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfmojzxet.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gerfxbbzn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwomakmic.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gulysfdir.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ggflrykre.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gtbjhgyxu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gdxmkibwv.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gqqizwjgo.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gwuqcomvd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gidgqylbf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdrobaqso.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqcpjmayk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gqurlwrop.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gvcdqjlrc.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gsmcmoack.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gbmuovdxy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gujrmjawe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gqhcflfwm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gxlrmiseb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gkzsegkcc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gpuosvuoc.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gtfdnbdsj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/ggmsmgike.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gkwtmgkdb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/geanwoxqn.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/ghiddfudn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gxxjcsltv.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/galbzmnpk.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcldgjyog.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gznjblixr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/giioumgqc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpsqretla.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gkzfhbban.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gylbutxnt.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gljgjthuf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gnyegjilp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gchpexofi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ghvchmxem.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gprzwwhqt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwkhymogz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gclzfctqr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfvjbetqd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gciknamac.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gfasiokdf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gbtxhnbsj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ghfaqogeg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gfxphaxgt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gbmumdzaf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gihvptlha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gjqiavpny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gpjoezwqt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gwmdzzkbg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjnreonht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gcfdqomfj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/ghfukuuil.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gybalalwe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gfvcftsxk.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghylwehpw.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gmeppggeh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gqbdnjjlx.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gmtqzcfcq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/ghdrzxpwb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gxaiylmmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/ghgopvdqo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gtuhdbgto.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/glbojagma.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/ginindmdf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwptciuzj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/grnlkihfy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjeyhpzct.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdwrhuihy.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gxadiquom.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfyperwjm.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gwtqaxwnh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gtcgtokye.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gwzrjhkna.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gzzearfam.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gzgvhnxsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gyorqyyqp.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/giyffpfzi.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gaycrcovc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gbdpqbyfr.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/glifbagtp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ghvhsdqal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/glqzrbzsc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gqksnlumw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzydybybw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gyjkiwzmw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gtpxxpkzj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gesqpmzyq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gkipupavk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqnylbm.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gbktwavub.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gguvwxzxf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gzbsuhwjq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvdfjclae.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghzjheenp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdadhmbqc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gygkfmuns.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gsnujbeog.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gejnkcbio.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/ggiwthldx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gxzlblbyf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbnrinsxc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gsqdovuvx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gxjxggpwa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gukwkpicl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gbsotpkts.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzzduocfd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gyxrldgpw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gockeasur.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gjsrspqyf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/guwcidusg.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gztzqbdod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gdyzqnnuh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gzlawvwmj.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gwrjaavrl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gdioilswp.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gleqdcygn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/granhcfez.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gcenmuihk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxaaibjrn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/grkoqhebm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/ghjlhizam.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gvinthnry.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gdkdtlfrf.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gnbdqtdvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpkjxhgf.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/glavltrrt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfkufjfjz.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtbgyqala.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gwkzqgnrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gdesfvirg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gjakrdtfz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gxbuofpqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/ghievbbgp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gqqcnrtqd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gfmkcxmno.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/grwdgvecd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gampxcdqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/ghscjxsmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gxvjfyewq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gxwtpefdh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/graliqubi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpfzogv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gwdweceig.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuptwirr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gehuswkob.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gwsjuutpl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gyakjeppt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gzrhucsjb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/grriwrtvy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gopuyzejv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/ggouujcwe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/ghbhqrgzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/guevblnnh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gxrndtfou.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/glonwiuwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/ghnaluixl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ggmybfmhl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ggfbppcfc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goewohscm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gciehanjw.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gyvsfeiwc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gczxahvzl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzlrmunlo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gzwjslild.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gbyqqsiyb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gzjfzgfuv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdxvhae.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gthsykugm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gdaltygzn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmvdbjlif.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gyzoabiig.sHtML


<!-- 参考信息 -->