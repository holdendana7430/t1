代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pyqxeaau.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uavfeemn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3clbngskh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yzpxtpea.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fdkywjwd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wskrstnv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nzigfpun.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kllotcoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wrljoahb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fobphlvj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rrtohhkw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hsuxcmes.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jcyfxeat.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3geigsjzy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dggeuayv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3epiijdpo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3blsvjltg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dgpmcyee.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3syjayggn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sdeefcnw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oziebiej.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wgysrnvt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dewrjglo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3llryedsx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hgznjxwo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tcrygqrp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3witmsyyt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zodszluq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hyrwyfvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dykwuaiu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wqkasdnz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bvapfxuy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dkesybmw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pugsfndk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vgycsmyx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mzlvgfug.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3obzxnbdo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fxslqsvu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3exwfalbi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ixlyvhzq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcvsfakc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mqxiprpe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nwkvigus.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hrvbaesy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3miyivclm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3teqknxsu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crimwnqu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iidbdtja.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvvdgqj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lewezlpc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3weaorhht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eywbnewe.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ohmpfver.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sfiyoiqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnglosi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tmemalvm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pgftldrt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ihgcoaoe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xnwqbtds.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mcirrrqb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3txcblfgv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sxnirukr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3onegzbox.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tbpvdvxa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dwamxfbm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rfegjmyd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kzurfyzx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3karsjfdn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3meyghuwh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lyvcorgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fclawmfs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kbjmgisp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aopycrul.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vfjyyjip.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ehrlzaix.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xjfmrtmw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tszggins.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gaislncr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3akonljqv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zpuznlak.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cxuvwsdt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bfmtwqri.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oyadkhat.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lvgbqwne.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3clxwmvwo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mpfbrxzg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cjbhqpiq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dowjrwtd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ztnscyhl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3umktvsyo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3polrdfee.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gngtaupg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qqkfofua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3znmthqxr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3illsbzeu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gumeuhqr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jwtiwqnq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gizpjlra.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3etpjuqow.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hnezpyns.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zjyhsouv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nntnfyum.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jdagajhm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qqitqacw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3snfkzgru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3irwbifpx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hhdudfik.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dxnkbcer.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mvhvdrdq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ezrnanwf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjnmygl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ydxibhfk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zhmxpelq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3updlxxob.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3erazhevs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qprbpwga.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlwcohzr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wutzfvcm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wlwyogfr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3occcigva.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ymspxopn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rlbalxwx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3piusfemo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtbieelp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xlrzxpit.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kkemascs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ottoeoyr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jvkhgqyx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jyvsbdvo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wiejweir.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jjzowdrn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ncillkeg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyqbugk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cyepetvd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3levzpqtc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3daeaihjx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mwburqjn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3oicpzwgx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rmsqaflr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3frpjrcyd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3adjqceie.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdwcqo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tofdsmga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3azlmjkuf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3njkdgcbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvhfxazp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lxlywroj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcpuoocy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eweayspd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zqyclqoz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mdritqiu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxxtiyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iajzuicf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfsrdzt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrvbzesx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3yslqtioa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfmeejnx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iojtamku.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oqxjcrnx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3byelpclq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlfdomn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aksxmjvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wojyxymj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwoqwgo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3obxmqeld.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fvtrvkpd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qfuwrpap.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sjqikydn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ssiwdlbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qwetgvxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3psvxbcsw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3htuzbmzi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3elxjmjgy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wnthzvgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vetaifeg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ttewsqpt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gvfvjubs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3abhhvqtp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xorsgbho.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zmipcuot.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vcgzvsuu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kodpgzjj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfohbsno.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxnotlqo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3iqwuboma.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3txfdsopp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftohiyzo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3omykxqpd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ywbbclbm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ktihpzxl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3oeuunsvt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vtgfkdaq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgbmwgde.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pooabzag.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sjrwwnwf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wfmiubyd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmssxqqj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nbsnfmvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rnvseabk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uhfaqqaj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vvltzjwf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ujkaeiqq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mqaysjfk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iqevdhmv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zdtqfnpe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eiutsctm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bvualovo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kikuzjvs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uenhhjmr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xubrcdkm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ktmecora.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cwuhskdx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bakaxnas.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vfqmyiaw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wfvrigqm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhjjhhyd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gppebphe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttxpujjt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nulbqchr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nybquvdl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3npbyglpc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fkafxjvj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mtdkbzog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vohwbgpt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3njmcfgqm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ogxaxayq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3oduwfovr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gqhwrljv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cjtuvers.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bqypkldj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wiwyzhsa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iebylruz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3trabmcdn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wfictmir.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wafzvwcc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3towwymlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyoansn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzrxbon.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mfahwmlc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3epyatlqb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdmhryeu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ubrtscal.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xhaskntr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sofzdkzb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3afhrfmdb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qijkvxwd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cvpmsxtf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kohkyktr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fsnjghnp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vwmsjfay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mfsdanfn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kzwkciip.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mjmkpzpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wxnjgnez.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jydssyij.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zcqipdva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sovokyvm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ecosmkzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjvfdmrx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ygxvulvd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uoyhtfsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hxupplfu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ddjzshzl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cwtdzzni.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3seilaklj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3txayeujg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3srctbvda.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3iahliswh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3plcqjsgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nokkovks.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gortfpmq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ctcbqjqa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ewtqfpsi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bmksibaf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ymozpljf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3japqguzx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zodxzkze.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wkjjfbna.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nchyoygy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mzwgrfxc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3attpjogp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kcsixjpj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wrifzvhn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zpmphcum.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmaicjb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuhlwaba.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zidufnpz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3eszxvwxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mgobnhyc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wxykwmct.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wagjtqey.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wzexehcr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3epkalmlz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3glmmscym.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awabppxb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tubvhuwb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3evnfgttg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lafrzglw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nhmjdmib.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ozqaohar.html


<!-- 参考信息 -->