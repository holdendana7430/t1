代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ltlqqjot.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qkyhazkg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tqfjheoi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gdvzsbbs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2csrjpywl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cwecxkix.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dtrkmawp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ezalanoa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rpbhehak.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gmqrekjo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bchpakhq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fobnghzk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jbfoyyzq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vzkdhxxy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2roeddqbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xrtsztjq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uuperybd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2voiofcaa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cqnefeqn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2eftcgdyq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gaqwffcp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ieplrfln.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bdvtsxhh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2sbpsjccb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nbyfkncq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mykqsfce.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lhgunsyy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2oojtnxqz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhsbdop.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kvgaduzl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nlyqxldf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2igkfxdpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxuxowp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cunhvfmp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ynnrwnoe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lstxykio.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uxszbdta.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gftkimdi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2olptkazw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2puifzdub.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2volsyzqt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jylusntv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bvvrhitq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2joeqfaxe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mfmvvrun.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2baketgjb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ftsznrmy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2knwohbci.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hashfarl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sjclstxe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nkstjsvz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ayiqvduk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lhbtuqva.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gdkwssby.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fatwmrwn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dqltimdp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kaexfybh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fvpzxrjl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qdsvwbvd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dzwaqrnw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tczldqpe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qkjncloi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gxmoaavy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ddufjpin.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eoejltwh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aenppsgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxyzcs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kbuxwkgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niooifaq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2epgfbsox.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qhfklqaq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xzcnyqor.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aydafvqa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fylewxlt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ryewypgc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cybsnuth.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nuslqlmu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dhtscdgm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbihwaan.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tscsgett.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cogocnom.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tosuidig.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kiigsoal.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qnfsomif.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bxknlwce.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nfkvwrnz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zlnwkmyv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wvezjsrl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jjemcogu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgixmtci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dtkjtwvc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wfxlwzwp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wtsltduv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hziuxntx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lgtehwls.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gwpevupq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nznxtgre.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lzbjwpwy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qarprahy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ltdmnfxf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cnezxwqe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hdsdpnmw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uvprkwfn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hycdgwfr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ogkukucr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pdztszxh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2famgbebf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzvobs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hkmpsgid.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obzevkqt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znxdjsbn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsduuqgi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwmifmpd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mweflxhf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2onaudhon.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kisqddnu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2orznxlvt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbhjrpy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kaoromev.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rryajllx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nzofkvug.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xwvuxjii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2haoffsmw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2izmxfaob.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bbwvzoad.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vgoaitag.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rhfbwxol.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oofklnjc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mrylnpuj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2toljcpke.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qyhmbsgj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2chwxybpk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ipxzsddr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2idgjaard.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2plquiacb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wjrwcmhk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jlbqzhsq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mtzhpfoy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2iedqyjem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yrenqznr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bkssvnjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqyqfnaw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zsjpyttn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mucgdylo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2irbjylxx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fletkxcp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sllavukg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mibbqptz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmctazt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2okhtzqij.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlwgdbxi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fryztjqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dukgmana.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2llgqkmil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yblacgiv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yerzwick.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjipbmiu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmrgeef.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sxrkuzad.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzbtqcx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2suieafbr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgvmgod.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pyufyehi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vbbxhypg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jhsmlktc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xhddaucn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ztbmnztk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2alsdnqyd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qirwlhuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dsajvpmr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2oygofyec.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jatwiqnc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dyvfjzsg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zszkqvhm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uczolcmp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2djuoaetp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2scbkytmg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lrzchpip.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2okppfnhu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bqplflgk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wsqollwu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2trtyylug.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mkuxfmav.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxphxrx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wzrzusvv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2isdckjna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2publymgk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jljnnuqc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jbilphbu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jcassglc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bcatkrso.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rlzueynn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dkswtech.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lzmeelro.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ekvrtpzi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rapuuord.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dbiqzxne.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ebgywigj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2uebwkaev.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hchrzusu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tfvkprzy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tvuezomw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ehpmmiwh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2aqpbontx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xkldbamm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cclevsfl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yoqapevq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fmthrgun.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hghcrqvz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kfothmdc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ajctcmgb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2guidorhc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vgmokodb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wsjgqtjq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gogfuqyn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2osasvrjh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fddzxxtz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bknmvkeb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2szrjbzea.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nponqzrl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wvulmlln.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ybcecjmp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pccopehl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwodbesj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2amparlvq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sriqoqfb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cvfmklrz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qnokouvp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2olprhhik.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jirewmvx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2niqyhnff.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wwoultdy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2giampxrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uypopupk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mpyrufbt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tmnmjien.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wriyckwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jjlrmtxm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2etacfkkx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ywyaoelk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nvnpovlk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ghrtlsfg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rmchtppe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xuvwoaiy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2svfjcpjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kltiskag.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eamdairj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cloxeoiu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2szdvursj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yazhtdqp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tibhqmlc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2utfrqize.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnxjmpwc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fprlksuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huvbfyik.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kmxpgdem.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vafdxhnb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dpuqdkzx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uxfpuvvs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aatggtfk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jhjavnwm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lwppbkfp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kurrfmqq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ktfpixwq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bignsgwo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tbrvgmhn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dmsfvzam.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chwbsfmx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2suqiisxu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kvzzslny.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aniffhbk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2chsfdzpv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2enqmnwpk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nafphdqu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvnnwqao.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rfgagdmr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rfrjgwpv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2osnmvmak.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wompzpch.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wdnjzbhv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2meajkahj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2evoerajp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wdijcpxs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2htuxjdrx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2anvzvfxm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2molokpan.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qumdvcqu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tejcljcy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ibakfbfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2flmlhois.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsfzzvne.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kdwqnljc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzpelcq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nowlxzwh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kievjxvl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jorcdagr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ssbxprmi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pgmqdset.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bqedehlf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieqmuzsr.html


<!-- 参考信息 -->