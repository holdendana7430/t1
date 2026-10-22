代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uritsshk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ktzlrtzp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzvrsj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wonuceac.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oackllqo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pxbmlagk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ikhubbxh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iqiwjgrv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yqednxam.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gyimifrx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lzvmojge.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oodmdcgg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pvxrmxwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yamcyzns.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kjdqecvy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2amgqtruq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rdbjbukq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zlrzufws.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2sgttgjeh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2plcgyuim.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwnneo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2oszoydkb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tymsnspi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rxvurfwv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2syiygckm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2sbayhxqx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2eijdszhe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2azxygdnk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2adsiphxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2alsaiuwc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iunoyack.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qtpzilxb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2udwhwvzh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qrfwfeqs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gnikgxvk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bthkrxwx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ermnecxp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gelhmefa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wrweiahu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2myadgvsy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhtkkic.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xcqiyait.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2duqigyad.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mxowpraq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kjdymhww.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xrlxyost.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ujoagwgh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yjrooimg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fdagyfcc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wxtxggtz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aqzcqyde.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dcxvwduj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2smkqpqye.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2paehemfx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cckviobg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dmeelkuc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wdwcqfho.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2driltxku.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2twwgpxpz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jzrstwfe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2axgjcngo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vusljklg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyjgfdut.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fcpqzkix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yadmujvd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2euebfgup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iornmjbl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mcvucmzk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ttbctajh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcpmqon.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mtrcwyun.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lzmuwreq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2oonwgrqm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qbsuvljh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vambaver.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2osnnfpvv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pqmeagjj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2awgoersf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ypxomgjk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dyfrsmik.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqvdyc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2beuwrupy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fmisfhnm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2updahhgx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qscmxnpk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2imcmlcli.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddqzjmas.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvcjkrfq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ipoyckya.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2msocfkad.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ogoxdqtr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aamauffw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2umykpwsv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sxngsmdr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qczxvybt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wygleydk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gxxipsiz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tjcwgmvj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zlyoebyn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2axhxilhi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2udohnztr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2defxacum.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxhxzhr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ynghmogy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmioiyhj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hnqlvatn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hnwbcrsy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzthfoou.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2owtcmakx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqbkft.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2usxnjwhm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lfhwlrzf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2reoybili.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rrwkqrhg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tjvwrohv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2npokfcpe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jdkvqrqx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iltejaiz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iradkxaj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pkykyeek.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xhubeoya.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kmindetb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ejiixcxx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ucbizalo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sykamdks.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2emeisgto.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gngwmhra.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ivstpdci.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mwofbkpu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vvjdlsva.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yqnstejr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tisqgbhq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aeluyrow.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uodckvuv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zcfqdiah.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qvzqxuef.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hcykrfxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwjoxjlw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xaoxffkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2impudgmz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2eaqqfrmp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kqtihwwm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fsnuulrd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2icyhdocv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ososepcl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwjazptd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhfkrbj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xzonvedv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ethyikml.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qwqaievx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wzxjrkax.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xldqpncg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wqnnzwof.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hmaghkpt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxzldwh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2crizegjn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yhohfxde.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wlypaghz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ogqivphu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zwfssyyt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ktsotezx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ykwqdfen.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rjxhttnz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2akjwnvfp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ozpdaehb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xyiuszov.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2exyeowpz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uaihgsfh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddbzdxup.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ytpreiwf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ituibpwx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oyvllwvg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2elawvacz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zzkcbnuo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fogypmdh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zmuaiddi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2toshdqmd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vqltlrac.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dtolqkrn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2foszypfe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssfpxujm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jqltsemk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2stemoisp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuxmasa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ctevrhaw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hhmsghdz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2myhjsftn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zqorcnqz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2crozzzya.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mcmdevqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bafqoozh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mcwlpgba.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nsavpplz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eveczxep.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gddewdob.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2eanrdcca.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uuaaogfb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rtengbrq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2osqucqbn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vzmujbkl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2owgurstq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jqxhwanr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qalgfpuk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ztywqggg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egqqmiws.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2okosntan.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhjtgbck.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jrkfgeuq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fexizsif.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tdhthuna.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tjdatfsd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2upizgjsz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zmigpblk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcngukog.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmprzcup.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2unsfxpkb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2geqxjlse.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ncmiksop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iojakscx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2febulihu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mixkcezs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2udbzqyna.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tymprhtr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlzadfnl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkemnet.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zncawvkx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nwyvmobe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xmnwyumr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2svtydvhn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hrwszybn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jqnvpomj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ngqavgqb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qtcjgydj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hxtwzwcj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dpdsptvg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xywibnsi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ygoffflj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qpvpxmcx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfkzqqei.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gnhskucj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vqvvaxzr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2msbgqqgb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fqovhhqs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fgvxmnhf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qjnflhyu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tegwhjkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nbcfatjb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2opryphpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhtkhxrn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zdohasbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdsevlev.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tjciynak.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2veazdciu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vlabeawu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2swlkabev.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wbzivbly.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bstqmjck.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2decddjsh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2diksyxyq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xjtbeyja.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2cyvzxoff.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ayncabol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bcnjqduj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cvwbflfi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2omdqgwfo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xizckdsk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rujzcimo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2aclhcgye.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ncvakyib.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bvzjwgjy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsfrqyya.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ijqgfsas.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tfoebhzc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bkigfzby.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlwxsgw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qxubrfgs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sfpaurih.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aorkwxkf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kldelibh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pwuyrura.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2shtzskes.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qyudiuiv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmyqakdf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nntdzvme.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2umhbmpdk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pwgkmqmz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2olrdduzf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2noybljqt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzckrxo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cguufssn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hixpqjwq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2blvxcpkm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2smnmmlik.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cimymbhf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwoalbt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyczypuk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cxgpdkxa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rzfnkwxh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajyhldoo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xarsaypg.html


<!-- 参考信息 -->