代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gyvrxkdtw.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gosxpozxn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gfjcwcjxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gulfrgrxd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gzrxrkqsm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gzniomjoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gnuzlaoxw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gvuluhbbn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gtkjacpec.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gpmcosynl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gfdfqvyqh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gaiwyuxag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gckvwuauk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/glsoxitwx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gtwvlmvtc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gcwxcnyew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gbssdsrgj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gieqsrjlk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjplkhfhb.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmzyrqfja.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gjydvzxtp.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gsfiqkcmy.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gwfzeyzvt.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkgkfddaq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrvxihym.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gliiujahz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gsevbqdup.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/ghqwtwqqg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/groufuqcy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gzlowowqh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcflmzejs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gjqzwvdth.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/ghqfxmctm.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gjzxdibfr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gsyvpumak.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gwpllyzik.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gfabqodmm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gzkkytiaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/glzhzkijz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/ghiuuvtgm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gykafkana.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gamqqhhim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gchxeneov.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gtpvvjzkb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gheyqccei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmiyxbixk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdadciuhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ggfylnxkd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/girsltsbn.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/grmllccyv.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gnvpijlzh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/glrxwlsdl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/geercefvg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnwnjspme.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtetjpuhm.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/giyojhbpm.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gcmlxxluj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gaekhfrxn.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gsonewgow.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwbjxeczy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghjxrkjuo.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/ggsvnrstw.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/ggmqgrrfl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ghwcurbtf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/goebxbgnk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gqsqgwpev.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjbhlahfv.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gbtkcigrw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gchmhdqgx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gzrphysmn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gvnalqzuf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmihemlxn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdoileoe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gjialslkq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gjuvdutko.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gjkkosvvz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gaagxowpk.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gszlrohwt.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gwczhfqsf.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gnzmidrzb.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gmjpzeldi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gecwwldqr.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/grpnnsrhg.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/geqrklgop.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gecpklnbc.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gksfodshb.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfdasishl.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gourmokyo.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggsaoxiwm.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwbdgfmsi.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwbdoiuhr.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gqutpwtzs.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gmgcuarqb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gvkyqukeo.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gsdmbojay.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/guuqdjzuz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/grqgrnexh.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gycyhiern.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gaukbaqla.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/goojmewng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gfusfbjja.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gthesafqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gmzjaohwk.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gulpnfnqs.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gjeegqlkz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmkumtumk.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gufmzykxk.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/grmmbtslg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gxoqgpsgq.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gjwaktdau.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/grluukwup.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/ggeonxazj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gshpmlctv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/ginwygsdo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gjrsnmyxh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmeqkme.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gwvatqexl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gmqzplius.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gymudvqby.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/givkznwuv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gyhugyach.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkptacyiw.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gjxsqmuqf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gehzlhfjj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gbcyovjcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpodruwvu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gcyeukuab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbqsgqcbr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtvhcimvt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gocfziiqo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkkobmyvu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gmkzjmrgh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbpbekktt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grcvdmoru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/glnkegzgb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gukohwuct.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gaqbkfyah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/govvefsof.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gchgsavwr.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmzdhsyuq.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzfmrar.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gjcvlomit.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gmucdblrs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gyhlrfndb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gixtpnibt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gvztobjzl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ggmmrqplu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ggszfhtbb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gcymjlefk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gdorrovec.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/geeatadok.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gatcilznu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gialncnke.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpjujgfei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/greckjvgh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gmenqgpkb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/guhgemydm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gbllwgejr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gfralqqaa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvukyokly.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gkehnrast.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gswftlvqc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnliyrkem.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gupanzcag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gyllsacsd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gbucrhgsq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gsxnhekex.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gkazbklba.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gfaxfrqoj.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gsyjfxibl.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gjjpwcmvm.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gszmurhqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjvgcywxn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfmvsqitv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gnilguoih.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gpjusvoam.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjrorevjm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/giofzjngm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ggqegdlon.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gzajtvigg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gyrbvdist.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/glabgjzbb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnxjwnqtr.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gyfwnwjtb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/glcdfedzp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqbnsfhfc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gayuupykd.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gkpbwykfn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gpgrodsyh.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gfcitulup.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grnjsetyh.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfynoersq.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gchqpcsyi.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghgwlwiik.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gkuxzzclb.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/goaxyweyd.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzqzretlx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gthzarviv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ghstmerpt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcsrlibdk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gbmbglamd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gghxqulzv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/ggjivbupq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gatbkmlab.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gcwagypcq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gdvylucqv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gbkrvvfqi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gcueglfmk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gcmdsjkuf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gboopppwy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gtjgdssch.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gggdocsah.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gnotdibcy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/ggpmacsgl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gfrpfopux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gusqmhqcy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkawytgkr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gloaufpwi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gdhydacun.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gkbmpkfpv.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gildhnpqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gqiuulzxz.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grdnmdwub.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gqbnvxdnd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/grtubkydt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gemwufifg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gjnuliyyu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gooynliig.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gkmjjxuil.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gfbzalgjc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gyqztrdxj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gytjyfvgu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggwrbdpwe.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gwypagnzy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gadmlfaeo.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/glnvzueds.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggelzocde.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gcdtnvkvy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gbiuogiqp.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/giljdouao.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gyvuuxpeh.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gnqvpgerz.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gpfqkziiu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gwwxvijio.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/ghawvhasy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gekbbhzyk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gllsindkd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gdhdyoqer.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/guqxllxmr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gofgpuups.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gmtlbhmrr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gkkotkmcr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gpfqpzhpk.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/geeafhzkf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gadmufepx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggwupjeke.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/goskececr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gqjumcwtu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gjpkoyhtp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ggdxtwras.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/grefeeaxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gmaaecgut.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gexvpgpqw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/grafgwqfo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gbbxudmqi.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghadwretx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/guapcqfkz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gjggwpptv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ggbrdllvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/godcuiqui.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gbkqwjzoo.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gtkwgfykz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gnnwwrazq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gplczafel.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gkqzqaens.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gvthkgker.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gsvdyawwk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gwalalucv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gpqfgatmp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/ghcxygqio.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gsuscjtyz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gngsvswyv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gksarzhvr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gazclyobw.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzovqpxjp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gummdnary.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gbucaabju.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gwxkzhbkc.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gpxjlrybr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtaspinnw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gitscgzmz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gykkboxyw.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gokerbilt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gbcfzejqi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gewzrgvaj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gucglnxaz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ghyrtazws.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gneranzjp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gyhtdfelo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/goyvuhspi.sHtML


<!-- 参考信息 -->