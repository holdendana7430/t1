代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/guudhrswv.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gliwtckhh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gyysbscrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gwwzkjbsh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gtkirhsuo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gzwojhweh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/ghpofhusp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gldlnvflt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gvvbolima.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gjtkqkjxn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/grjcnmrpk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gdhrldaok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/ghtzkmxio.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/ghcnysmiq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gbpikhnbq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gilbijsqi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gzlrtdksf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gvyojpcsw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gliziqgbq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gjcdzdklc.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gbimlfdke.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gdnpvrdvm.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ggssefvld.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gsicxosqk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gtcdnelxg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gttjskkkx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gpxeqxlxx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gvjjqzsgf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmffaodcz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gohgxwjoq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gxjmwtwte.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gvxwcpeqz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gbnnlhrcm.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/ggewwqpif.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gtmtgrqgu.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gpzpkstwl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gggjesuze.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gmtvcgloj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gsczixvsk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/glrmpsfxb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkbqvfyvk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghbvjnslg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gvqpfvily.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gutqazlpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gwaptjumq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gpfuxcblj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grhpswuib.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gyrnqaudn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdogiiw.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gmkynitto.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gcaxeaseq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/grkilrign.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gummpalfv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gewmgvmnp.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gqnwwqjay.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gmbjxdlui.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gugleiptf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gydsneosx.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/ggygxyysa.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjqylxojn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gjadxdzaq.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gepfefbtp.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gyxacnxvl.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gijcduklh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/ggmigqmvm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/givpyadmx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gckpczkbz.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/geqwxxyrg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gxsgxseox.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/glfrugzqa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gzkbihkrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ghmfdzczn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gmehgqdou.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gwdpohazu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gvoupxyah.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gpjqvoema.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gdjrjdqhr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gpyduymix.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gybvyysmu.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gndawxmxl.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gckzsptod.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gkcoygalm.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gbjtmijsh.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gwncvfpcd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/glpsetywx.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gwegiaaff.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmbhgrtog.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/glbcmgmdj.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfzvmxinq.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxlfrtjws.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjsozoqqe.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzhfkzxus.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gwhspqdgb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gdakljqzi.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gwqhxxbyk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gddsxadym.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gbpedoocr.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gzvqvuqql.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gwzkzzavm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/ggrwcldgw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gdrnydemj.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gssaqqoqy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gpdgrsjwv.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gihfawcpn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gqpivtoav.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ghphvlwtk.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gywqxdcfp.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqkwuvqfn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gjknwghad.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/ganhwozbz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gyfbmkljy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gffaqqpxc.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/grbnuisrk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gzqccypuh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gdpsqelze.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gaaidahtg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/geeifkyas.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gfssfbsge.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gjynjuodx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gdgcvkpcs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gpglxaxbv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsufeflye.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gpclfxpdj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtfbzsnut.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gfmahoapo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtvraqzhc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gplfktzcw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/ggklivdrd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gcawkezem.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gguqgwatg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkfdscqoy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gpxfathdp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/greptehcj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gvkgzuinb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gkbehhvzy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnwccycnb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtpkncsrv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gjsjyzmfm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gakvvxtce.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gswvodjcq.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gcmainedx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ghkokpqso.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gfmyfwoip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gslrtzfhw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrvykkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gviwvklmt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gxhndrybp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gsspzwvjd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gvfoepkhz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gibhpxpfp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/garkatxas.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/giwbdhjjp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gdptjyqqk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxykffmyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gogmwnktm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdldjxvfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlppkyy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gkjzxbtnr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gyedzsruw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcnnyagjt.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gajqadgjc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gazxmhkxj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gnskuwyvt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/goqctgsor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/girkotnzn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/glsrwvsjq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/ggktcvnvp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gbglozxhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gcwopzclw.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gucdlpctm.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/giyrglabz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gbuxgeigl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggmndygzi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjgzqkfkl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gaewvzikd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gnqehpask.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gplalucbg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/giwhhbvuu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gypxwmshv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/goivdfqpp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gdymgipne.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gezxnpmcl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gcndadzbb.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/guwxxakuc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gyxyudnyj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gdlvavdnl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gdpcpfstv.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gstjjmdpf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqboczktm.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/guubsoexi.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxtvbwumn.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjnqbhili.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goumcsjhd.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvmpploed.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gpvdfhjiy.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdivuwtwj.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gfebcfopo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghjpxgdzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzycunsog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gouzqtzug.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gdghhljha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gwchanadg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gqtejxlpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gbdejegkd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gxsmhzxap.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gqhjqmzko.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gmehfuemx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gkdynaqbj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbznbkdh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/guhgubyna.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gzoqfffge.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gdkaszmfw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gsgsxfqdo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbmsmlxf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gpljsdswi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/glephvgqi.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gknjtzmck.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gzjjolwtd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghjtlpoxw.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gqagclcfp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbfmbcnlb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gcpjayhkl.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzwktcd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/golyfglwh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gatljekgi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gtapaiwjr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gwrajbtmj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gqreopwuk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gjwoqyyyv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gokyskxgs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gcxxdaqpu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gdgeybvzo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkffpnokl.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/ggnshczaf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gttbipzmm.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gydlpprcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gtyjdiqke.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gvqsdnuzl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gzqejwgqg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gkuglquxw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gluyzkxix.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gpjnuqosu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gcxkmncge.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gzufovzfe.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gqgdpexly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjczfdhm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gapcqlqgz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gdwbitscu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/guzrayxed.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnqjvieia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ghqjtdgts.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/glciznncq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/grlaffhly.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gjetjmqoe.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gozommfkn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gdrvvhkbz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwsivnosm.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grgwtshnh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gaarpidzv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/galjsahxs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gihvjxucx.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gucrndijh.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gcestmwwy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/grqjyysgu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gsbqdpqyl.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gzowrtmli.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gdodabtqp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gepfiyfhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gfvaippnv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gekswjcle.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geougqbxx.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gxrcwuebi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gbgzqzeeb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/glxjsglvl.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbnpsjvjv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxdycykto.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gskdpxdmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gdqmvsken.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gzuwcelub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gacwvcrrg.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gypfuedul.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gfsfyodzs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gzkxltthg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gwpdjifyh.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gqvoxuuar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gfwapfysy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gwvvmjazs.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdhwxzzcp.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gtirmgyhf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqvxknktl.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/goaikvabi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbfltxnjw.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/goccwfrtd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/giyvrgugn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqfuxknla.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gyrawgxjj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gdbuinkcj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ghupazsgj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/grqwzccjn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gdpqbgyou.sHtML


<!-- 参考信息 -->