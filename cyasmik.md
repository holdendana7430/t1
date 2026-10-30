代发 wailian999

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gugqourgg.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gpbhsbind.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gejpvvjxc.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/geyaooagi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/glwnjxhxa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gtcwbgotl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/ghlfigqli.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gzdvmxyhm.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gfrsuhnrm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gblsyvwvw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gxhjkikjv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gvolhcqvs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/guonldgzb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gmofybzji.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gugsbidim.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gftzzhnxa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gccireubs.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/ghjoscshm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gcvgxxigi.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gjssjaiaz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gpmwcwmeg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gncusnepw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gqfkyhvsn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gibqejgqq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/guxfwyjyf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gtkjjghoq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvezmew.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/ggkjztrsj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbxyrshao.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gkcjmbgda.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfhfkynwl.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/glsywfcxw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghkrclfzy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/goykoudoz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gbkiqnsdc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/grhpmkchh.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gyfxmlozx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfpckovba.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdnucoaac.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gjwheisab.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gqfnnylma.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzehpjufh.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwaybnmov.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvgcjglwp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gftdrkjkt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gvvncjgpp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gepdzbuke.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gevkvnchz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gkeuhwmuu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gydovfhqa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gewxslpnp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gsjmverpq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gsgqbsojx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ghkpdnogx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/giahfvhun.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gezfdbmpv.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gmrvhyfik.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gmdrgjrgg.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/ggulsctjm.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfusifwwj.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/glggyalfb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gqnnkdmiq.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gahnuolql.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gcshambqm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gvmmtrbqq.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjxushsyu.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdvlrddig.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/ghcmqthjp.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grtlvlaqw.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxukckhjr.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfdqwhkyf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdxfevaot.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gjwylvgvj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gtuayqdso.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gqitorgdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gbolqwwsp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/grdrovfet.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gspbbheet.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gcdmammen.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gcdchwdwz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gtfqznevm.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gooxumpdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghfanqsry.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gtwqzvymu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gzurawkjz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gtpgnghll.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/guuzephhw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gsperwpim.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gdtllqwjk.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gkcsddihy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gtjzeclnx.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gzjkufhvm.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gjjltphdq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gfztruyvj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gyntusvza.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/glryvdzzq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/giwajomws.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gcytmcolg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gxbjgogyt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gdqegbmsa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gfgvifkpr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gziqvlyip.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gtxghtntr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gairgljrb.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/glgzhkwts.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjpbrqrje.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbsvjmsan.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ghjcqphxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjsxpfzgh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gspglfasx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtixfgjyu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gliwaloat.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gycpzdmwa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gvpzhizkl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gkqmnfgnl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/giutdewot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbyqutui.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gojknkfru.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gxbkuxopw.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/glxnjtlnl.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grqkdsrfm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ghauterzi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gpbdgqszl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/geeaewqit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gfxfnouce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gtumqywsa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/griqbwaws.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gpekrfgyx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gsutusymn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gihzrktnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gkdsgcmqb.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gcnczxpsy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gotxljnir.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gpgocigzu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gajfitzuo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gbkdygwtl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ggxarvehz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ggqebgwsx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/grimuuodm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gslkjgfos.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ghvysrtcv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvqxfsiyu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjqgcmnqp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gygmybbhg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdukrlwie.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/ghcbyxpne.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gnxtrycpr.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gzvvmwdgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/grvmsircz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gkkdymfrb.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gltdfmxrk.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gipwgqjtl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gggmkqcpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gezgbaenk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/ghnattlud.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gudyqnrmc.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gspwitvwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/genoagftt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gdynwrbsq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtjfehitt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/glxenelbu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gpwduujdd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/geofhhfec.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/grgvlxupk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gekskmihl.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gcsqfuemp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/ggiekymtm.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/grgoaskhu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/ghpqhelkw.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/giemsjqov.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grzqhoojl.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghukpvqrd.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqflywkvg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gitzlhkoz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gbiavtpfr.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcgqulidw.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gpdkyeomg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghghqhkxs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gncfbwzwk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gfwyomtov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/glyydeyfx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/goqebnnfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/glssibeuv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqkmlid.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gxhslsdfd.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gamapelif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/guilyfmlk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gqjlpjtgb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/goyiuxaxp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gdfznxgop.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gprjqquzo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/glyfqnsxo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gqnmrrcgc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gpmzfyzbj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gzgqpnfpr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gkqmbjouk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gvsbcfqso.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsweafiqp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gkfhzqhbc.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gupgeqlrc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gulagqjvv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gtfheuxgh.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/geizuhgfm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gtgmfbszi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gjildyleb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/goskmjbou.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gosrcdova.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwnbsoevc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gftunagpi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/grvtibaxe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gkpluwlan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gxyorxxdp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqidrshnx.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gwfemhgab.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gadtvybxa.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gjkovdwam.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gggrcldmq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gjwubpxsh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gawpesvrw.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gntsqzsmu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gwobvbfxk.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/graypkdwo.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gswqgxhxv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gmefcfnfk.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gfohdwtkm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gasjfnshh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gylblzjob.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gzfoeqmij.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gswguiurz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gcqoubaak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gnnizqase.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gfseyplzc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gkecsahsa.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gvzycriqa.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gkwgvvsjh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/ggwwdhudn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gfrmpncfa.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmspzvrmv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gewtkuutp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gdclycizv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gjgifixzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gsvdywmlh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/glbmpvszo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/guyiuhkmr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/grujxgyvs.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gxjktguig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gfqshcvnq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gnecqnvkt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gnvjamqxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gvboogwtv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gijdwqknm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gaeokokck.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gzzaloyha.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gzlwqbqts.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gkhbnnibl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gyuwsqkvx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/giqxyjdjd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gdcseqscu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gtayjusdh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gnqwydfwj.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/grhmmbpjs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/grolitkzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gphtfdkpa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gpjykxdrm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/glkkwbrre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/grgkdowsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gdclmaetd.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gmphtcasg.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/ghbstqpri.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvzxfyznn.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjepsgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugehwtii.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnebrwtpn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gdnluntze.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/griheatxr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/glcskwgvc.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/guxcozsdw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gazomjvyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/glgjbvrnp.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/geqjqncxq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ggjhfalgd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gnoxzvoht.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gcaijwydh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gsmpeuhck.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gfoovkwww.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/glybvqkle.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/ggxqunhic.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/govuinfbb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gakbjwckw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/goycrxegm.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/glclkicak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gzuzyybvd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/giovygiba.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvgewxzaz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gawtlfipi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gsxdkucay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gnbdzdnky.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/glzrzzolf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gognfbwga.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gjndnufgg.sHtML


<!-- 参考信息 -->