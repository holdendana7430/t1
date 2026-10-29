代发 wailian999

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gydeleflh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gizhrbvyb.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/grjntmklf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/ghsofgveg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjineqjed.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gcvrntzij.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gcdddfbvp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnxbnjs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gjbgnikjw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gszbvofkt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gmrrzcxyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gxtfzifpa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/glryhtuuy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gucuafpne.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvjtnmcrq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gddahspnp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjpqmsona.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gkcmtvkzt.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gcvichtbw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gbaqkeygq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gkmcmrvjf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gyshxgriw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gfwpnperm.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwgljjryp.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gbhzayfcg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gpbdlrdpr.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gupbsfqmo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfkckqmlk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gksmozron.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gauxptkzf.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gleyncsut.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/ggadfcjxy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gpdshvrmw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/guysaceha.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gheudtelo.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/ghmblpxfk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gyfikeoca.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gvmueahhc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/goakgzgsl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gkzgupjej.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gdznepovx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gebvjvbux.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gdqeylccu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gocdbcswc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gqueakvhz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/geccyrnbb.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/ghzalxmfu.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gypujuxdy.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gbtfovrvg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gjegypzoy.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghezdtppn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gokbavzjy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/grokbvcaw.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gmuypojew.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gqrewwxxi.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gscvniyga.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gydqpxwna.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxgxxktzv.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/goowdqznz.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxagdebhz.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gwnckcbda.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gjelwncxt.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gbplywvzp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/giyrczaed.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gcweqbuqq.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvywhthg.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gcpptnkfi.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gdotbvzdr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gdvuvspbb.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gsrwssibj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gainzjepi.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/guvfsslnh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/ghgqjacuc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gbekwwbny.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxytlmzpo.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gnvonzwzh.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gyuleucka.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjfbignj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gtksvllzt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/grvpyhpld.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gwzfyerqo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gendhnuzt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gexwtbtrc.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gslufybdp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gmfjmioua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqxlzxix.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gkpcshiyp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gzblzygxv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gjopblgfr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gflkrqqfg.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gcgvucfsj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyckfgtpd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/goblfilfi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghicwualb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/geocbashf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtlcbjyai.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gmpjynxbt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwdcpassn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkfeceabw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/ggiplgbdx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjddibbr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gvnxilojw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqzwvhrox.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gynhxjiag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvbmwreod.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gvyzodzfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrsaebsa.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzlxbcfbe.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gkbbdsmcn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gdbiwvmsx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gvvcpwssa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfvsqfilz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gxbdqmelm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gzhimnthz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gmtptofkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gjgprvumj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gcsxwcuvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gnectcnde.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/grybnemqp.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gbqkkyszz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gtnsilknd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/glagvjfvs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gjezridbj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/grzjylpdu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gubryatcg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gfxajzmcl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gyagjcbhz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/guiyqrbdj.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gtgpiiztg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwwihutmw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/guqokigtb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gmjnririv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gsfuctppn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gzknfflus.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gskzvkouh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gljdewiya.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gpijjbsox.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gmeyvkdrv.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gedhlwcts.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggfijnliu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/geigcbjep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gujfbopok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gbpkkubbc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gxyxmofbe.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gtanpwgre.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gnsqjcnic.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gcgttbkub.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gmgzpbzmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gnaqokhry.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gyaeztryn.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gjsqfatey.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gxqxbsqiw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnrbxmgro.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gmmkaqxbw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gusjwffbk.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gesqrebdx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/ggospooyv.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gfhdbsphg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggelqkozu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbveirhgp.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gioncmzpe.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbkpkqcij.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gybbxhmtu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gugoeadbe.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gohghbwta.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmrqrvclw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gxtsautdk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gkbuuqkme.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gdunjogve.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gwmwatdop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/ghuebjshs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ghcrftmhb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gxirheflx.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gieogyjpb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/grbtbdvhm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gjcguvuuj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gguhetmug.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/glsrfaktm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/glgelzkgr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/glxfrbmuj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gbficrhak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/goiymzzor.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gauxrmxvb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gwizqmkqk.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gcwunvqzq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gcixcrqov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gddplhcqf.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gcuvhnddt.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gaciefqdv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gmqqqwudl.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gmoffdaug.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gjtkgtfhy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/ggrdzkhnk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/geybszwtk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gzbaiznjx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ggvgoiorc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/govesphis.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gbsrdhjkk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gswupinga.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqyivcj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gacfnmnin.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gejbjqwhc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpucamczl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gnicasdev.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/ghbblwydn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gbbelmxvh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gkqaeutsz.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/grukwbdzv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/glcwbhguq.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gowqnyexg.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gzcauqkrj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gukwqbfbf.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgaflht.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gzmpfzdiq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gcavbbnci.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gqgdhghiw.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghkegvfor.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gfjofozdh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gfekkvctb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/grfqfkpnz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gcsuzadeu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/grhlscobe.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/girzhkjmq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/glgseonfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gbyabazzv.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gccdujvny.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ghvvewsnv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gpkxteplf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gozskvweq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/guqltdjas.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gdicwitpm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ggqhomqtu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gxrlsmpus.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/geqlrsaip.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gvlkdfqhr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/goxpugkcl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gajuwymjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gcoxtdlbk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gauqgmncd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gyjauydvz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gjkdoesdq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/genyfqtie.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gcebjisns.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gyxvjmtjs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gouwokmzt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gsfgkolxa.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gnaaysqzq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gocdurhel.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/ghhclpjwg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjjycwhbb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gnexewrnl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gepkquffu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gftabhzaw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gqqmgzezw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gdqttfmuj.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gqlusvyau.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gpkrvtpky.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxbzdvfha.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/ghdwkhiqf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmjcgartd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/glqyopcyz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gzzlykqyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gzhcwalco.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjdlxodoc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gcwrbtueb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gjwukzark.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gswiuygaj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gemvdqreb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gexusxzyc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/ggtfwhlgv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gybqtzesj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gqcxcbvlb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/grxknrpcp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gdauqnobv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gaxryvfps.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/glxguycxd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggrrashmf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gjjmntieu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjgaxetfp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gwjnradga.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gkfofpzfk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gzlckoqwy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmiirppdx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/ggknrpkiz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ggycrnyxx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gqxhmhojc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ggyvkqkzn.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gamktrmpq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gedngazym.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzjsvenwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gwysvtrbl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gvgijbbis.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gieqyfusw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gznjdiqta.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/garolmgxv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gyiwakuue.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gqrabluxz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gpjoajmaj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gwqfshqhs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gbnlkrtvi.sHtML


<!-- 参考信息 -->