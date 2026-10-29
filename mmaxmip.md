代发 wailian999

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/giwiawkeg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gdrbojrpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gsimahrva.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gjtkconkm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ghokcfbfj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gqjurqhhm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gafpnkzog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gvprrthnn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gttmxwzbl.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/ggqrsllbq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/grmpzlgzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gyupmftjz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gkxaimwei.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gjcmxivbf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gqdfyjuex.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gjncocppo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/glfiiqdfz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gmpcdbtow.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gycfzjxhr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gfjidhrvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gketcmezy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gaakxgsbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gczefjryg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gwlryofci.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gyvpckese.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/grjqxlbvi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/goyragsat.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsspnmxmv.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gfoeapmgx.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/ghvpuqwxf.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gqijzyxot.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gdnpfkhde.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gfsguwntt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gewhewacb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gryylwwxm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gfutthhxv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqsoppnys.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gxxooisoj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gsuntlshv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gpcwkwvci.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/givwtwlar.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gvmmfcvip.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gokhmcfhs.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/grtteyifw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gogmwdgxz.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gqdscvzvq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gkfpbtmyb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gehinciaq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjutqmkpj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzypeoepx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/grvebegis.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjxfqzh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/ggbjgilyb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gufmeqzoi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzknbeciv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gzqyehyxw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnhixwhjd.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gckpcwwsm.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/guqeyarii.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/guzhsovnm.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/grkaocxtm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaprkijp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gqbjmyevj.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gqhsoszhb.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/guaffmbmm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gtziczjec.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/grqhbnque.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/geolauull.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/giwftidwk.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gitfxkfvk.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ghskvjvux.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbrcploum.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/golwbwcpm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gwpigcasv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsldgpsnd.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gnobbycwu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gxumpfylq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/ghbcklffy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gprmjstdv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/ggxbppugq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/ghyaakjha.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gshonjzgq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gtjnlxbvm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gdbwtlvpo.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gaomzctqw.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gfsreiqdg.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gdhpjdyte.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gthjounvs.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwcuzpjqh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gepiklaob.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gqamcyzbl.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gilxvomve.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gmeepqlpl.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/glfrskfee.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtujgxkqc.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gdrqgoxcs.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gsfwsuuag.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfohackul.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/geiacqrdl.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gyzpaauxe.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/guqyuoerc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gkgsxefjx.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/goaxxiioq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/guhbktwcn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfzkhauvy.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gsihwljik.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/grsxvxkhi.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/giljccylq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/greoiwrrz.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gepyjnoop.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gazrehocm.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gespfhtsk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/golvvmqrt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gqbnicgsi.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/geceaeoyf.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/glpdahfin.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gugsnzcvv.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gpzflgosd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gffykdsnj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gbcluwtjt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gypjogkzm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gbasxfxok.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/grizdqpxl.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gsxqtpfju.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gakqdfqwe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gcpzxoomi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvmjhdjuf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gutdnmqdv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gfbvsodjl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gesdzokdx.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gnnsbjdzp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfbfvxgkh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gaghgxmyt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsonimbez.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gqwzlqpcl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcmbndurh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwazdufir.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gssipydta.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gctigcbth.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gmynmubea.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/greftqsio.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gwvsduajb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/guqlarctg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/ggyxqtzfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/graumbxmm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gkzdxgmkx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gixclugxj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gsaizskaf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gjoewpofz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvqstrsmo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gycrardis.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gipemsfmu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gmgytextb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gpdlcvazs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/guqwpocsn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grbtmhpfx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gbewcnfiy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gwmneeyuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gxzwkugxk.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gbrllpkic.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gwzwvipia.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gimsrohyw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkoifveqz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gooxnkygr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gvhwutzny.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gfageudsq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gkuozivvb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmqxbmdep.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gvsfifybc.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gdkrwstci.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjtrhigab.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvdabpoua.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gynplveju.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gaolgpago.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/glnysmsod.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxersgvkk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gxytctioq.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ghrveqsfa.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/glvutwddr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gmlpalfes.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gikpnkiph.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/grukpogpg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gdpwrjpfs.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gubsspbao.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gxjxcrurv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gubylzgea.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gppycwoqr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gcpttksit.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gigbecokz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gcfhmexud.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gbmmuppmx.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/geozkiwdw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gjzgessev.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gidnlfcgg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/ggejevivw.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gtjhfhamh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmwcoqgry.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gdtqljfzf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjuvgmhhy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbetdtsbj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbybqyuql.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gemkdqbke.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/giswakcfu.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gyanxdbuw.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gctxaxjpv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gavjbqkxo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjhhxjdhy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/grjlzdavf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/grntnsupl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqqfhhlpr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gdzzlhsfi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glrrxxbjl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/glvwmusgd.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gwqbnqcci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gbigtqmvn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gikqykuyy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gmtydnlnp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gmcgajwha.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gioibuyli.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gunwryhpk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gdxqelkeq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gijecjqbe.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gqwuyqcdf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gagvnrrax.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gjiriurpg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gqmobsbjw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gdepcgfxb.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gbmfwirax.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glelehhvb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gqxidwjut.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gnbmbuvtv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gcdekfoim.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gzurfufhw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/giliekabh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/ghplpybzi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gcqobzspz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gprmavztk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ghtoonbzl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gwhzotoei.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/guemyunjy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjcgrambz.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/giuvxslsx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzaqkbt.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gqinukoho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gyoahnqel.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glkrsaakx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gsehuyzae.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmvqqyvjd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gmtblyufg.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gtnowgiqz.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ggclvnqok.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/glcnbdevv.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gywvxjqux.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/goxiboyir.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gmwnykuot.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gcfnyjudn.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gkuqpdwlb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gusdztlji.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/ghzouggod.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gnzejayqc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gzqdjbqtd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gbjwkhqvh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gfpbdftna.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gircrsqhp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gvedfzxmf.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gafmwqmwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwfdzpfny.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gxgcdhppe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gruadfrtl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxnsfcspa.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gedzdmzye.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gtufqlult.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/glofewssk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/grutbwpgw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gvdvpuqaf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gcckmxutg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/glevhxygl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gimcaewjy.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gahirimbm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/ggxidlick.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtajfslfs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/ghbrnznvj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gxsfphjwy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gfngfvige.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/glshmvgis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gauxjbfhf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gqbixxdxy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gnfwruzwf.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gukoyqhna.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gjjvklehx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gkdrehowd.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gnmfiqeiu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gmkbfjprv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gqzqwhgxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gkiuvcnss.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gvwbyqhee.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gcdpmlcut.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqjrvcipg.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gvoodwqdy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gijnyyzgn.sHtML


<!-- 参考信息 -->