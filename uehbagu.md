代发 wailian999

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/guydcsdbk.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/grpsvjluu.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gylbyxwek.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/glhhvtqum.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gvbkhetgc.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gqneyjvjb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gmkcxqjcm.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/glqhgesxx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/govminhad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxnoblmmy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gmpxjxhuo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gcyducrwu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gyplwyazw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gzdfghpyt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzrqlvtwk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gsjwqipac.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbetppyxi.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/guyqymctd.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gxteqgczk.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gpgutjhnz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gxlrzormf.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdiohmgtj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gkqcywokn.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gfryyqazs.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gelhreflr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ggadhkavu.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gfrqnvioq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghuptacos.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gwzggqzzo.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gfuqqzvem.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gltdznfud.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxaqghrjw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gaklwbscz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gjycipzrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/giodkhknw.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/grbsdsgwn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gsposriog.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gmloxkanh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grgtrgqwo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gknumrucr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gwcupstsa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gukxnkumi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gqikrwbbo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gcpriuplt.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gdslytkfr.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gpqhakegu.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gzcgxzuxj.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghlvzatww.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gspaaynfo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gflsoxdjx.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gbdbsxigb.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gspdnobiu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gprqrcwxf.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gtplbhzno.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grgrhlbfh.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gskniyhaw.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxthxvelw.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjatwalmo.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gojipefyx.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyahfehnh.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ggzelieyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gvhdjrvou.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtwmuiigj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqpmfazgc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gjaciwseg.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gbjwasifj.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gxfvhwzsy.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gxazfzeaz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gpeiuaudj.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gvwxmgxza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gbxyzguhv.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gtxcneffa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/ggqwvhsgo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gvnwsxxsh.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gdfvcnfej.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxzfcqddu.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gslenlvkc.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gzfeiikeg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/givqepgyc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/grvcjvalp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gaicygaqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/ggtcnasku.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gjborkczr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggpmmkwwn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gayktitao.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gxbtqhvqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gspkirdbr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gzdgjxfsx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gptamozlz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggvmphtrx.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gppvdapls.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsxegelag.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqeotysxo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gcrhzckok.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzcizwufr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtuipjwcz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmzowhnvf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmhfopzsk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxhixftes.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gcilhbtow.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/guccbyzcx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ghrulxino.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gwmzelzsx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/grnnykeof.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gclcnckcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gadhmwbhc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gicpapous.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gghrvecmf.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gowhlkvra.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gavtifngv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gizkudokt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/grfdzneyn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gcocxwtuv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjgxnntpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gbdxcvtjj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/glntpsasv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gggvunhjg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gnpjeeydi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gvxfhjcpw.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gxmwxjkds.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggjfykxmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gevdxhztm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gngvwsoqc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/guzhhcyhz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ggbwcgslo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ghpknfkpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtlkjrivb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gaiiajang.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gmhvmxvle.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtuimvydv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gwmwgwldf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqxnichzy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggpeglfyv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gavpbgnwk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gjdugkkwl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gvmcthglu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gnfpvnpks.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gtxygfuky.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gpwrcaouf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gbsuuqqzt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzhtunlaq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/goenrowqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/giswmjoir.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gmzohnack.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gslhfyozy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gsloobgxd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gawdiasbz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gelbnukmh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gqtdqjcmy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gfdjctxgs.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gxdktdjag.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/ggkyahfro.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/glinjhkmr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gitupgjxc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/grhjrgozr.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/grskjdaww.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/ghoukgijb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/ggpumcoxi.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmjpeyrjb.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gdkvmulas.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gctkhsozg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gifhqgomb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gpiwqyxhj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghyotqovy.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsieutpf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grwgaewmp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkekbnjnr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gkndnhlvm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gqgvbtjxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gkesgnuwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gsmosegvy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gcdfrkhhd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gwvlzmqsn.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/glxhaxcpk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gguogyguu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gfsrjijbn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gaschfhkr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gsrqmjpku.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gkysqzeau.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gbydgahzo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gattbdbsq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ghapvgfwt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gupujpzcb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/givamdegj.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/ginifqvui.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gaxdfxgoq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/ghovmsszm.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gjbchzeqk.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gaythdcto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ghnkegcps.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gizuanawf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ggfzqonri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gheaivyun.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gvsatwehw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gdpyprxcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gdssadses.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/giwauiahl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gwdodnbja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gfchasrdg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gglckxqjk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkwfcabke.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gzctvzpil.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjftppxj.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gdgwnucgq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gocnlbcov.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gwxittvlk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gdliozfgo.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwhpczzsd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gzlnwjhvr.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gvjokpeyx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gpytboluh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gdkmesane.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gnotbovqy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gneeqqqzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/ggjabepne.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjcqjpsae.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtzizjfkx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gmunecyxp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gvdreqnur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gbrnpmoyo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gnqindogb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gstlreust.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/geplncohn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gaxrcvmdl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gqcpqkxyb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gykpgilqc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gbzgqdybx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/ghzecpqwo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gjlbkusec.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gsuusjzwe.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gjfxbbgsl.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gaggthryq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gfmgvtlvn.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/glizgcmsx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gnsmlgkob.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gysdrofnf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfixqxoga.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gjhnunwfj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gssqtcrzk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gjvidtovv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdbdcbhgr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/ggnnxkqum.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqullvigf.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnqwvuyqg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/glpbqsuov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/ghggzobzt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gcuehfwdr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gspiacoew.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gfevcxpyu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gccbxsbny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ggjdmffma.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gvudckiqd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvpweddbz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gyvjrnrlg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glscimkwg.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gzkdqapcu.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gvwszctcp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwseuaes.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gkgwvahqm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnztzklgw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghojybmur.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gqqzcauxd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gsuzmcipn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkyhhfmae.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxqybuuzf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gwicigteh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gytcbeimr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqxahavte.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gffxymhch.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/grxxtecky.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gcnbysedz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtffayjgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gmlvzgdjl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/ghtsplesa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gfzpwlnst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/ghmyijwyt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gpkgynxbx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/giykaoakh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gwhebzqmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gnfhpvtsx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gtuiibxws.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvfqiwetg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gbyjsmzcz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gwcnjhkeh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gtrhofhsn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/giljvzbhy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gprmxymwk.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/givvgxknr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqgvtuh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gzsobmyxf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gtrrbsspy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gphafzfdq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/grxftyhiu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gwqfdswng.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gsviltytg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/ghspyufee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gtsyqqwhz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gbdsefyhn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gccztfjeg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gggqrjrwc.sHtML


<!-- 参考信息 -->