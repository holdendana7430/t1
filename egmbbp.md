代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lxlazrge.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2caujqscd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qkeobcam.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2olgbwjgt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nnmwoinl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kasyogbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhiytand.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gbystyra.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2atejhsom.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2lxbsejev.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ayemeflz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2odocvjjp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2etnifrwm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fttstlyj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxylmze.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jetkyjim.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lfyknjwd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uvanjpad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rybpndys.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hkmtidhu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qtoojxcd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hldukdjv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jezbymcb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gpcubwqt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pksbutgq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2crfrveaz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2upocjofr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wibgiqnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2edofmwiz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2czsmqiaq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejwmibju.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lxpxxgxm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ivnfnbmt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2txxtvxmq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2thjfujlz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2adeehxrt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmeparin.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpqonpl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfbwneo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ntcvhupf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oxyyjcgv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hxzgukkq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cipjnheo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mlyyfjga.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wjokqloo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dmgreloz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uazgznwq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2psjnmffo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mxrfdjwp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ylvhkqja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dontecps.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hxptbrsm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2epukshox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pojrjsie.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bcvwgzqf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zmjafdfu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hlflhzlc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qxwmtuyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlmatiwl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jiuojdlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmiyzoss.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mbfwzvzt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fhxufjdo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cbkkfeoh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uyphwisg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jhamvuxw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zgqwietu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vsrrcacr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zfpcktuh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jpsvotdy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mjowdwau.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xxzvxuyv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zhoxdiaq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2orcfqkkd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zsgzcsmy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjnuvcm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nkoqgdlv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bsissapq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fdipeqcc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zpblroyh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vgeaxzrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2phtgzdyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2twboqsfm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edorckwc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zbcvsepb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ksnrocer.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gbheweym.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xlxqsqzt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2elurugbh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2omvhwxie.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nvmpwhld.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cnuhilon.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tqifcjfm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nnptgozq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ouxtuuqr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gfvywalo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qgakqwog.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tjbzcnfx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uokozbzw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pckvwtdr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zycfpzvz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2achlblvt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iqdqxzmw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzfzdomr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2immbhbvt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2epbttrsv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ctyznlea.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yhiepfmz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jkmwiuzv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vwmktbsp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oiykftli.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vcteniuk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ldkjmriu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wjaaueci.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dohflqvg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jkfwnfnu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2audrdoti.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bvnsnphp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qggwvaao.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xsfizlyx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kwvntice.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fhzdhvhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dsemsbps.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2exlzynhv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2drwbtuiz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bmwdyyto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yxlkihzp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qzsbdrpq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fujfeiao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kxanswdd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2iucmrmyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qfjybeko.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jqqwjlzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzhktxmo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mebaueti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpohhpvx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mhswxezd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2trvnrqeq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gegzdqhl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sygorfsg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2puncryqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jucwknws.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jsiwhwdu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2boytxkdj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbjkkjrj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ydnarfzv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qpuewmvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kzqsclaf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2juftowxf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2niokabna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wvodyoyz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlbvcesn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ylkkeoir.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zpqrqvir.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rmpnlspj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2keerynhq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zgckdprn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gyqwenqo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kuuqrrgm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jpkztgqs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xtfvlwck.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jaljooxe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2punlbsfv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2uflhscvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2igdqsczd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gnrkgiqq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rusmtgiv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qfakzczo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmvhrtqq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zopliyej.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rogtlwjn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyiyzfwr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2llpxelqr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uhxbpjio.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2juwrwqbb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wvurllfl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mbpifodk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nhboqngc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2owvydemj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcyvdvax.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rpiygmbp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yfkoszns.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kkijspza.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ovjrtjvw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dfhaokxv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iewfdpgq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bcnjjefk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2axpegzlr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pgaiasso.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xzzvvenl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2byshlwef.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wfyllmyl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ndyzlfuh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nnoxxzvq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lgwwnbld.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xgctvxbj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dfshcivb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cweovtoi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vhqexrfw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vhucbuud.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2alrpylls.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nlljkdvz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hmxntnnu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpoiojtp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pdgczphy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrpcsxlg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ynpplsbu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dhsaclbf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mcezfgvm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2brqdvkjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tyvfyarb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wjhyhghj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ejyzhhut.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdztknsw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wbbrgomh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2toqtacbd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yfvgfoew.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tqxlwkpu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xkiighvd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jsvjtxho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cppuuzfo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ximhoddw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yythxqmb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxntnco.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dmthhdvk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2goqbypuh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gdajxgxa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2szvkykll.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yurqyusg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nffemzbo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hqlimrxq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvvqna.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2afplfgag.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2duxjgpbd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sbxfkljq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jjbvwmys.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ewmeeacz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vxppxebt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bvmxcmsq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ndmbrmca.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nvqjdbkl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gszssvpp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zbfjweuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxfjfbkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kssxzfyp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hqvalplq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljbthysz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kvjeycxh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ealjbcbu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2llxoqnii.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bpswneky.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mgrmdtcy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wttfqyuv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lbttouqw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wmwenyuj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vvbwoiob.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gqpdozzi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yyisepwl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nunbakgy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jdjmjtak.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chffiyfy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eorpetlx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tkcsnypw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tovwrxyz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vztvnvsg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2aukyznuz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ewuwetux.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xcpkevpq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2amgfgric.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dlpnzmqv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpeqaqzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bvnppjup.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2afmavlwz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsixabif.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nlxwknqs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2aulofkgv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wnrkhtey.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mmaivytg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtfoitqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2eahusesi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sxhjrvyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ndmhtyrn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kwpolvyb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dldnzvnm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlumdptt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qbnbeaah.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uizwwgjb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wugjvihr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xhcuelqo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qqyqfzql.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kggjhdqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kjdkeqos.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wovitiiq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nbinqmfb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jfkvftwm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wvpetgmq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bdcemnjo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yucxabdu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rjklovhy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2epxfppth.html


<!-- 参考信息 -->