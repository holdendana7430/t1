代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tjhfmbsl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzfiwvl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cinsbkue.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3mwozjwyt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bdeyxyyp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uacnfsyv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gvzcaaqu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iepxpsce.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yvdoprvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vbvnqhuo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lwqdfoig.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gtrndloo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gnxfnryf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mhtmsuex.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qrjtigow.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fgjwoysg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3agxvxrue.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qktqcvdv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3macgsdjj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cxddlrne.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zfthrbed.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yydkawhu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nubwmhvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3arqjtrex.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zbnshmfv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qfnqzttw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rmaobehj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yqxatzpd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zidkifwf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hlmlmnnn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3psdmsmag.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oqhjdlen.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ymyzgezb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kyndwbmk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pgtnccsx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dgmxjclu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xgslzzpz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kbkjvyxs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yuzcyhsu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xqbrjuvg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuizgngw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3onwtamiq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3schhecdo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zipmbomp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qrlecupa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ngomgipo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrengv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tpatdftk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qfwydzkx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjuagno.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3eczbrcug.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3arjcgzjk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cdisidvj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uzjoolnb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gsbkniyw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ztrzbevc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wladxbzd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zaukatyj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3effqskls.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3oupqzffy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tbqbdhww.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nashxdyr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mlbzxxtg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gpfzqacl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oammjvei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ocetarrw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3irzknkig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lfzfwfya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pdkssszb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pxiapwpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptmsfcly.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3danqjwjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcuysdik.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wtmmqehn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3buoihepr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3puxlxhkr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xebortnu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kbazszum.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fhyeijvr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3innzgzjb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qfvkahcm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gyecdiwe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ozwqsuqf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gvxblmst.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sijunulk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kmmlzaew.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fiukpztx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bszcyugx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zgeggzij.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3knkmibhh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjvgnyvv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rwrgtpwj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ntjrsaxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hmnrzzcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lamjgkof.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tinvscnv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xrwfcjuc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwkvnyq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3liucxrmd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lbxsrlpm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wfjzgrsn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jagrggwu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ymamclyv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wyjqevms.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ulzukwdg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zpepisfl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qguzefsd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3imriluua.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uadshcdy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qkzzzqxq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzizlgw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3djtabeii.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3smgxjrzq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3djleuhfb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wmybpmdc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afvujoiz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3iliyzxrv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vpmufxxu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ampvgaya.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfffukur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kwusuejx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zckagtks.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ebbdgarw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ywbjghei.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uwfknxlp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qaefjbxc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3apcjztzv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ppxdvsjd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dwqihdqy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wcdywdgd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ksfrfsyn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3izubmzkz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dufrvhif.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhiqhkh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dsuuumwy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fygbnwpm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nnuaodhn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3oqtqxzjd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kdzjfqqv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bqbcoeaa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zjwlyleo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3prgglpwa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gcdwtxrj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3okqfpjjm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ckpfevhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlxepdmc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cnhatldh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvujyxao.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3blwsjlnj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3crgpovyf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nqhmefot.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vtncnpzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3stmjopqy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkjexmwh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ppzymoym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3expepyuy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjnmhct.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hhbajeak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3duajpxqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nflqgczz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kiorqhnz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xrghirzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xptnmdrg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bnsoypqh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kkfetuyv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gvbuysxu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zrlmewxx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tqypsuzc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bkymwypb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3svznvund.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fkxaakei.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3didcgltl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lxytljsx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ykrxceyc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fbctrtyo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kjrrxiyj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvcvbbr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3idgjvgsg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tugywxyv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glkzabnp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3znwsrdbo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lgbryyjd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rddgtwzk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bijqmvvf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fygqttmz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpzdxlg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wotaulwp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rhsmmycr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycqzwvwc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3svrcupvp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ywqbnnav.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3krbllula.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3abnrsbic.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xtogydcj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3htdtvaqy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efpionwk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dnbauiyd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gtaxtzjx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wgsjuhhr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfktwskr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lbcmmwxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sijktkzz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wxypgcwn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3quionhlr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3deqdqzhy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hnvkuduo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vbicbljj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hazgvtnw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3njtzzucl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3cqfrpddt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kraedhyz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oteewqba.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkvryllx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ybaomgoz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jwdpdtpd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3msakbnmw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tztrisgh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dihfyaun.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3frxgrgov.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hntenuxl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gqptykqj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzuisj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gfgehlbi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rilxlbuf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xhvitxqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fxdsnpyw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nsbkqeqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ytnzysrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xeffvixf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vwwwlefh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3txajusjv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3otrcfxvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lchgentq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lyushcom.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3aetlovqt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kognhifz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ztksgomx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kgbwbdmb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yzvkfyxl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wanvrwni.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aqcvvrhn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cfrgqani.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jelaajxt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3camqoctk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rcqvdeeq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rtugvowt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vfpwddmp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ohtmlqqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3braagqyv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kzrffulm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3thdofbvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmpezs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iunbofen.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsmgdri.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqszdmi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3odrmacfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqvfauxh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bbafftsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giujcuev.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ixtbejpr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rlnmjuhs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zfbgzqtq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vywnzpgb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3djufdyof.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zevsioiz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lujgoptr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlhtfoc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lcgbfrsl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qymclxdu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zezhbxap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kciuoviy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3csnxhiun.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wspadsji.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3urgmhzvm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3atrsafrc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eoatgpoy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3srezpmxk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3sikcqdvh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3veizxhfm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vnxinvdv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gjqatart.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tyfqijzu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afsbujlw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tupsiafh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctxadcih.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aagirriv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3opgawvws.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pkhyqaed.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wrfloatp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpvgmzfo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgaujiap.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3sfjpqvag.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pztdnyyq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fdsakmoy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3thwpuosi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qcluwkgm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ppolvemv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fczugfcp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bbnwwplv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vfrtshmf.html


<!-- 参考信息 -->