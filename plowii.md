代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uafctjba.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2godjaukk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fadhnhem.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yikhodwj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vaknngoo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pyjamdeq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uyhuphqq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rpcwsosk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vmmkxeym.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2urnsuszm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2enbyfeki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tzqnloms.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mafznhck.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2izoznroq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzrpwmk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2illucyzp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2oubyxahg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jrigqtxq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2okdfwsfn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rnhbwvkp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bigkoflp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zwptodup.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vepksckx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mtvjisxy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjaofixj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2upmlvipz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2smfgfyiw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vdqwyydv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mykbitwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nzjrsazc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kypnomuw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kqskunkr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kngzjiwj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kpffcvev.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vkpwfkaf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zghnykok.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mgifgwhw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2djgusmey.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hpextjao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vnnefprm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cbezcesd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ymoptpod.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2srsgyfcz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lypjkdwm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lmpoejmu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dkcyppik.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bmylisry.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zdlwqorc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qusefimk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2skclvlhc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cdokmrpw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rsncotwa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wwtgywlz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lyyaemtg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lwcazvtk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fpoywlqc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdzzmwc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wevzzfti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txoakubm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gibbesld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngcpicnh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wdxpoxod.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2neazdtjl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2eudqblhu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqtlxza.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrmwrcq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vdgotgam.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ciwamjjm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hducojrw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yjztvyoo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bxggojlw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rpolcxvi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rzfihwyb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tobasylr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wojexjem.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwgiaws.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vsqqfrvw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2szearppz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xybldwlt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jtchrhxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tvpiosia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uesovdia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xpvvcqvy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qkbpketa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2abquifqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2chxgbdif.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kymujtpl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qomrqchx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wzbxloak.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vysvtlco.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cndivnyy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iiwwoaxh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2erufnydi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qwdatjrt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zioomfnj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nybtvwzo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2utrcmlvf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2quhhiddn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzyuunf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ymhjcpuo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvmflzf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aqoqkvgk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2prgqbbvu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pougzbzq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fjcnehkn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vybboiwa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zcaqwplp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqliqtew.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jklfzqjl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mmduzras.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ntqqqdek.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qchiftae.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2otdifuop.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oudchnky.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2actmlazd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rcswpsjl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iograwpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ljhzlsaq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hnkzdarc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xcjnsdws.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kbixrwvh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qcdeivvl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gnrdfydc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lhawueme.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xaecnkxc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nmblkjvh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ocuxfenl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jvuuthjp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jkeyvaze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dooivhtf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ywrukutp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2znbdwmms.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2byhyqohq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iexfscqw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ecdlncmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvyykgad.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fgdcjmpe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyzbcng.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ssbznwva.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ijwnuwhf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cftgabwq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qafmszcq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xxsgqvkq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iikqprly.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qsulxkyx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vnkawajf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qjtshvub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hxrdktri.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nbobtqfy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qjnlrjgj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xaazgmsn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajibhjfp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gyolodjz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zbtmrrgg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gayhcgna.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjhoob.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lpqyttaj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xrxoaeac.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iakizght.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2grikvwha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aldwhdxh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hziepfxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2veuxdqws.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nwwlaeot.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjajcdqn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvmxqofg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krbssaqo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ivbcqeus.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwzizipg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wcrraatx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hhimgeck.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2etltftnn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sxucxsvw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zkxlpzby.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lqhlqlpc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mufldqwy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kohaxami.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nlblnidi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ulqaswfy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmqygqc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yxevjcgu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rrrrzlur.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sndmunzb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2thuihvrf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zdahbzzk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2boagsuhl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yxyffpfd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fokhfhbg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fvhjklgm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2auzgpgnu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zfglqkqp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwhigt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eynhwhem.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gobytskp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ljjfxjat.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oxdnrrrm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cuuncfqj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tbgppqbg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ujyhbmgz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yipatwje.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2buzkuzyr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lyeluory.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lxtptvgc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iysdlpsj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tzsegqjr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tlrotldx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ndyetfkm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2flitngxi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ujppcqfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rihlbyaf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmbzidrq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qtsldamo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ppheognh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ansxfsnu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rwfwwtpn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tgfleivn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kogoqosu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sptbmglo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vuekbkbi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2izdqhlci.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2scyojlww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fufjlgpg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nhnmrppw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2twnggayh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2snvleqfr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qlnukfdp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wewftkmq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ibqebuon.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvmgxgop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dsnkuwmn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wusrprbl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhzrghod.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jytdfwav.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iheiwpxr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kxaiyioi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gttrrdnn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2srdxulft.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uuujtsvv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2etrtpqah.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nxuaklqj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2takcxvvc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2sxswszet.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hpuobhca.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zvknzaxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzkxxoqv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2sdqvcwte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwsbkimm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tejirraa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qeeuftqa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wwxwlwrn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2weojhmhf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dkqaqrjq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dtoiusrn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oxkrpsws.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2meuglnrk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ydaxwqso.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jdxqqdxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2plkpytvf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2uqudfjlq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hbchrleb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qiimgjfz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2khrkjrxj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ywjqbwvq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jivlrggk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rsuflslx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2stncsnmt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rujrsogf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zkkppcml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dktjoyql.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zpawkesz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vhjwxoqz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2scttafvj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlhyvujv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ziawmlxu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ybmitnpf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ullpuupu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uxfrkimy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kojkjquc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dlyawgco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2quiekaah.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fxccpwzo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pdczferw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2roknlsha.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lgadrxcz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qkrnubij.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pcactmji.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jgdngwml.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cleedegg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2osumqxlo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qhydvizo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ttmpvlka.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2munmkopt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tfinfhcq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wiafmirp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cgwaymqf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2shaxpxbj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xunrxdit.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qeqsqqou.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jchmlprh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2syfixndv.html


<!-- 参考信息 -->