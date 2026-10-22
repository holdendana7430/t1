代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wlybbpgz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2otpbpoxt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmgaikfl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cbipijmc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jklkqcpn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yjnnxnht.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wpovanpa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2duhwzpad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zztoftix.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jidirnmx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dlujnoxl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lsvywpge.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2acwgnopx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ebexlmxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lxjorleh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2psjqdbmm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pmmisafk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ejrqeiof.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mqtforsk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lwxzwhvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtkvfexn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bcbfxflk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ggxwdzcv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mhwzwanw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uorhoozl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2czwswvdq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hseionik.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2flziplry.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lbcinvva.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nwabvjpf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mctgolwj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xpzlcmzx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuoguze.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gypuliwo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2szyqzlpr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tsttxugq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iwjfdoqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ctuvjirg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2czfufuin.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jxjnfaot.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rapaobbx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yzalmizl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wpmhvwxz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2eenakwis.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pioawlqy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xctpvywj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mxjltkch.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bdtamjec.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dpbibvha.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2glhexoib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wlwjbizt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yntjvofz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2clhoxpgo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aprxscqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjqvwlwj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2dgfkuaqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxygyzkn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tllhovzm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2oavpsfsy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dsbyxxtp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aobyvdea.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkstgdpd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2acbervev.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sbfkmwoi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ezgqyrwr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fkheizve.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gdjonmbx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nmfkhhce.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eyvdduzw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jvzvfnli.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xyrlbbqo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yyfhjsgt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ymouwsmr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ijckylxz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zdofqiwq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vwhkawjl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yfsxalis.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xcrqfqnd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bjmienmb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2chcvapia.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ajbfvhlf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2shupviba.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jiqziswr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2aqtdpiqh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kunwmmft.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sbptryji.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sytbzxhh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cyljphyc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tdgeyhyq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2iybwocby.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vtsxevrd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vmrvwdrv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2umswcvsk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wzzoheoz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhqaawo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dpdxirpy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2equzfckh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frqplwrq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmqpedow.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kjykshqs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2buzexdpx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pmyujgpw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ubkanryi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vqotsxmr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wyvyrowi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gqhokemo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hwuqshmf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nmptshyu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yeazxnxz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2arughzhi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbdhmndh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ilnssxcq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ixudknzj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mvgtwqwo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2avloqaqr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uupzpayw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wzpiydii.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wdnvxwml.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2miyxzawh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwksqda.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xopfefmz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tennohqk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dkvzaool.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jrylakbo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mmybsset.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rwnjcmqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rswgxrkm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tumscocs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hlsjzsiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgejcmxz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fowwjyig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiuzazeo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jyqywxun.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fddaezdi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fxrcndjv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wtqkueup.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yrblbatr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zayfhajq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrpwnvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tokwfjoz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2shpnfszz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vbjqmzyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ollbluxb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ntijhlss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stecebah.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2smpwtkkc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yvedkosa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2okpbubmk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2euilwtzs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2psxlxrey.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2slastgoe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tminmhdt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2osrcmrio.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cwevejzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vunrxogi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jzrzopvp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jcvsubtt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2muagewrz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uvfeylvn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wbvmvguo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zhgedyuv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jysjuvgf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ygkfnoly.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yvowaeum.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2feahvjdx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lzhalzof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ustabpbj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2onqcdwhw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2slcgkrzc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zyfzuxzb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wotwvpnk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rpvesfwc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jcgrlzbl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xdtggyxx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uewpwrjf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fehwihir.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2efaniatm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kfwolihq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2heykszxc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozxbgsmo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2afgmfquq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2megrjtxv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yjkomjsr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2byyifzyc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dbiszoqg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hdyamgxs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fkubpcfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tqognckb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fiqpwlfh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2magfqugu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kvycvmfk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2agefumkd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2paakwxfh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2svpdvgyv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2myvbmyik.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bbsyeucn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bciqjzms.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xcntabfa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzthdbbs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnxdebgu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2khlfwgfg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2whirwmzl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lvwkvmdi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lnbyidox.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgyvpaxr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rovpkahx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gmstwhqx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekugwbzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xqygmbnl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qecefqpy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2thlrspjm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ytwsffye.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qddbsxee.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rssdpvls.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hjzudhyl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dzziznzv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mpzydsmd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2glipuljj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xwkbrqjz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pkavkifv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ltfetjig.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2owhvslco.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ooheffkl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nteryqzq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnbldxlc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hcraewks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gukyzjwf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ujkooxnp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ajrbvyax.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tmqivsgp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iyhsrioy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rojzwbgl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cttlqmgg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hxblqaog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2weocehfm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yhcttmcf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bnwruasm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lovcvefr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vivlfmxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2llbtycjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdrxealx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fbvkcvrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iunmmwvz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lqwquxnz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2acwyufgb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pbhctifu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zjvurdbf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tjejgfiz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2oswbztmi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fqqfpuye.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vsgezdqf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sprdtmti.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hhjkuhme.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjmswyv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dpwpczlm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2khxegkdb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2potiivrd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhjqze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2egydukgm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yrlhynyh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mwklhdmj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ytduczwx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wahwsdwu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dixqlevq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2slyltioc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ugbmlqwx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcpuuvcy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ipcfzfsh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qwlcsjnz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkefsazt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vebbdmre.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uniavkag.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vxfiiewh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vuozutby.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lqwsppam.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tqzpvrgp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wcchitnt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rqubhsoo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsultrrh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ootizwbk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjentznt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jlowiiig.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ukitbocd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2osqfntxr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wfvkydiv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2urwtzhzq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2randiakx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hmjphimz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2diksxupw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ferbquxh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kxutcyml.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ydcblxql.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tbhwunsf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2umxausta.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wzgsbkwo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2unyhglbw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rnpxrepw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpxqgjhi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdhtwksw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzyizyod.html


<!-- 参考信息 -->