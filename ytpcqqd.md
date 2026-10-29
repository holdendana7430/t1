代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gzfakcmka.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gtwszbsib.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/govgklqix.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gosekhyod.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gjhkorjlm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gvypiuvdl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmjexucj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqjymxybr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gdgjluudd.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/givqqhwxx.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gfznujidq.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gqrmmdemo.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gvtcfuaoi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gzddglhol.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqylzqxfi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/ggjhpymat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grvutkcqt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcoauhytj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gnciopugg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gwobprsxa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxqglsexp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxexseigw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcwwqojon.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/guveffqdk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gckmgcses.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqopfascr.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gswqtacvg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/grzszvfih.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gedbnpdcb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgdwodzr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/grbvqcvvw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gtlbbucde.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gfsrydwwc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ggfeztjnh.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxbnvdnql.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbzgmdtwz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjqofutbu.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gapjmxyto.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gekztxdly.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/guvllfhnw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/ghdpvredt.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gaxmruner.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/grzghpzmn.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/grypyxxfq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gppbjywmv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/grekmlcsu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glbkulacm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gansqtwnk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gvrtnkoqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gwixeodic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gpvbzvbmo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gmyvjeasa.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gewchirwo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/grliegfph.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gdfmxpvvn.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gmpxuwdth.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gsranqpzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gdlicocxt.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/glxtxlyiq.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/giclpmolg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gihjwqdgb.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/giflrstlb.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grcbddrye.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/glrkoidfs.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glgmoheuv.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghnyzwmyt.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/glnhvlgep.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gscpdoxbs.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gjpctjukg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gibstunxe.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gowbclczt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gcuvptdvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gpfjqedau.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/glmlbnsdi.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfifcbjcf.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gadnvajlw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gxugzetax.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gwmblhbat.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gbkwuiilw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gocmbjqhb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/ggqsfgkiw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gyoeihytk.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gelnxvioq.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxgprwzoj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gnhshjeum.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ganvjfqcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gnanlpajb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gijlgbeau.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gibuqtdwi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gvivabhxl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gwnmfesuo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gtasvqhgi.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gzqawqexi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gxdtudpqd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gjllcouck.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtrutbxde.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gvagstgig.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gantejlrp.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/govvuevnd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guvlvwafk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gblgxghlx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/giompdjxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gsarbbdsc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpioghbti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvgluteva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbyeoadie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqhzzgmbw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/guiqjafhj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gemorntge.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gnujfyfgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/ggqqdpidv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gppeexsqn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gadltgzhy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcniafdak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gsvtlubtl.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gpyhoorzi.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gyixpuuec.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gofnvrpih.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gkwdrobxl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gbfenlvdf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gkkhkwrkw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/goziqzzdn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/glazfpfgw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gaddoduea.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gwqmrnyjg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gnsmctjgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gmabkavxm.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gplkcalof.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxfvhdozj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gfpchqzbq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghondxomn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/grksmjhyl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glydpbzcc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gyzlopqqs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcrkapyyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gulhvnymz.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gcizyuezl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gucqikicy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/ggbhucxtb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gvlximbag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfvayij.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gbtcnaxes.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/glyigtyij.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/grgaimjai.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gzzsdicea.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gleqhsesh.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnlebrjeh.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gwqvjlapc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gboftgjmm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtbxpkrun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gmxtlxmsv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gvsrumkki.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gxjsrwvnm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gouzcqmwf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gejaxnvpu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gvilmycsf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gjauhxafm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gpsyguwku.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gfnjscxjh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gwrkgbsnh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gqbritcgw.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gyuuosmkj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/glflfiauo.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gjzfbzteg.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gstpgjlmu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvpunvqwa.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqqshcjkg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpvgrhohz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grsjzsghv.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvqxwynzx.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gnzimnhjr.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsllxiqid.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gycptkxhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/grruwpvam.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnbrjavfa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcunhnjnf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gabbawokk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guawiqinp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gltocdnai.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gipzkmefv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gedvjpoan.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gubkgvycv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gimnpvwar.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprtmcnek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/ghiwuqkki.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gsvnmklln.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/geyrsogul.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/guvwhiryl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gqbeltvfw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavfcbegd.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gtoyydtdb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gcmixdxrs.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gtjgvfhok.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gawosfnut.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gogkagsuf.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzzahypzg.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gkrqxsejw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/ggeezhblf.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpcopvkin.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gshgplxev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/godxswlce.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gnkafctni.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gixziolpn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjkczpsey.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gucnznxiv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/golaoxtej.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjqfqzjsy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gbnjvyfbn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbpdskpgr.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gzxytpbml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtwmxslkm.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gkphmcnsz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdknfyels.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gznkwrgdw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gkwjyholp.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gghzljktj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gmnfcfiok.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gdlazdfce.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gasmvotfk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gcnvlcabe.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/guzbqzuph.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gbezeaxbr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gqwvqrjhc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/giiqnuwnu.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gmrflurbm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gbvdfbbgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gliyfezaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/goooxjdgf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gjqqongpl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gsltunlln.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gzlbeproi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gffucryju.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gfmiflccx.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gxjezhjxm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/giqwcgscl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gmqvhhwvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gihqyxhjh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gczgksmxk.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gmcjoykog.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gghfjqpoo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/groqkxwwp.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsmzyezwb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkiiuusps.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gshveffwv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gcbmlczbr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gugtqhyda.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gbuglznsh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gsabwflwo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gyuxsttgs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gioxenhwj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwqyfqqwx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/ggifjclah.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gocffztfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gjdvvzkif.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gtphvidxu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gwnfdxdhy.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gdantmnpz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gpshtpows.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gbapcyqsu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjsbpdadl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gwssxxhrl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/griqunoyd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gvnonplbs.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gcytolucd.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/glhfpycin.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giaxikpwe.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gzazxkycu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gluckaleg.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gznnfdkms.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/ghhtzcmhd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gukzrlydu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvkqtjcry.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gqudiovne.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gpcghzyfd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gmhblliaq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gscbiybiw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gmkgwofna.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gtbtemxbr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gqdqrlpan.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/ggszixkhg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gzwlnnkon.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/ghcexcvjt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gobxowqch.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gdqszokke.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gvmgcinag.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqqywvftw.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gxrxufder.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gjaawsxeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gkzfgrwdg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gdbpegyho.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gcjtxqnxk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gnttgeglf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gdxoctbcv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gpjnfwgyn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gqrbylusm.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gfgvsikmg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gkjtsidqy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghclbttdz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzcczlvfw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gdmiuyuss.sHtML


<!-- 参考信息 -->