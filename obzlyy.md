代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yiypwfny.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eushahpf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2clsvyebf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fcbsxycs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlydsnq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vghlnmdw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fqecvdrq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2odoycuge.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ubfczphk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zczntagp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vivxdjnc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eknalbdu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kebrhndv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pzeeckcf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qiicemci.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2srsuzxqi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ehpqvhto.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ncllbpnq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kftrpekp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xgkxlnjq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aselttpw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vxxcsdtj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2trkjrqwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwbdss.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pjqanumx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2babkfvdt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2eilvfjft.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2unmrnlba.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zljmgibc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bukkdifi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lcotqvod.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gvzqyedv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2zenyeyre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtfrvth.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qymyftfn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pcexvffh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2emvwyrfs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dejlxdnv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cfffflee.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ibykizjx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2exculios.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hkmdphqp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flloxzfg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mhvenvox.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ugsrstbn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2meqvqpxb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dawxnaqh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oaoprmjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jevoacxs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhmqnga.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wazxasni.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zcaorpwh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zyoebjwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wtjgjlpd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ewqmvkuy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kcfviabw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oqwxlebj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wpfoutgo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bkgtqjwr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yqdyrsmf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2igbjwcxs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nmjvcajh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2esmatdib.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2louvygpq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2stjdozvv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ievbqmbl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eqjtjgwv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gkfytaza.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sarfbstt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bcaffmos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clqxrper.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pxmstfba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwmvrbhi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2afzzajuo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wakpcnrg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2itiagvrs.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kiqqbkek.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ziejxwoc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uejvucjo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wsgeckve.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zhjounzk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gkmtqjig.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dprhzoho.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vwzauyjg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qqmdwrwf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aozueocw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vqmkldkp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gegnwvpr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eeqyawtu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lcincibp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ujggdzgx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ckajcyvn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ztaqnocd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rnonegjj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xamjbvsq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2monimqor.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkdoxw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xawhbyyi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wrqamyfk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2onjumdck.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mfllwuuz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2leuojbhx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2shgrhgyy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hptpcinn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozymsbez.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lowetpof.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ehzqerrn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uywpuzng.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cexjirwj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2amdppmpn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvuiwmbt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yfodddym.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ktdpevvg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkaktbib.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2moxlqjls.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqwtzwl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfzyvyli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2erdaemdr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2spzfxguu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2maxpqvcj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ygwevvdx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cfauqksb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2geyxjxtp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqxciln.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qggjugkh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2omknkqct.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sflppzbj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ylddyrub.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2doqyhcdg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hvswesxw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ppgitswx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pujwpkkt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2stkpiuwp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2osjunatd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2psjkqfjk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsmwuxu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wduprira.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tlbcdrfb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mzqqdxem.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wagrrxwc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xanqjdlu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2clgepfos.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2shprploq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ndwxfarf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2arajezrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exaexkzw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xgcdkilw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjfeumit.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ootkimuw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjnpklg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ifurddoz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sdglywts.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qbjzearo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcebbkbq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kuntyswd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ucaukugo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axfzlzuo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ywiwwqpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tepelbru.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ghfbdruk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jxpptrlm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2epwzuyhk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hqfsntde.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwncjtht.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nmxnvmah.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ixiqbahm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2siypxyie.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mgtpfwrh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xpevypes.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jnbdishh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ufrbkqle.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cckxchcx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2agdtxiqv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yyyxclem.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rbpukgps.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qmyvhojm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhejkgqh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpxgnctk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ppglxusw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hrwqlmik.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lxekyztj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2onjvtatk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvkuuml.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2snmqfrvx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2onzligjr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2scimxsda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiwefkze.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxhjxykr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejuykiuj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zsrefgja.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qgnjlney.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2phzmwrrb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wimgcwce.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2luerhubx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2trdhsmwr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2apuahuhc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awopmqfq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2keujurtk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fsievbqo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypfknqav.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2feqwxjhj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cjqxwkop.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yuwhespc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2okfwgrxu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2oalzpbxz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mianrohq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sjgrexiq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ccawjggf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zdgacrya.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tgcplzyk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hhfhtkoq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wnogotly.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iitpxole.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ufdalpoj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2onppgvoe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rcmtvinn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nqzzaggt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zslwtcvr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvdwhg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aicqncqk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsqwtqqg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfojptif.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkicmduk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fulruete.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cwozhqav.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iofwotxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2niroulyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2odyflmid.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vasgkrbt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zhibfrmx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pzruyjgu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlamawna.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kuudaugh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gcgwnrhu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xbdykogh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhyhnzz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bragolyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gwbmerdc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2okhwsxzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rgcnvyuv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tphtjlwp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vimafrod.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kyacmolq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oemyitnv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwnvad.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ggxvpdrr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tvlhhzsr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cwsxcxiq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zgxdwnbq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xpelxrfn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lusmwmmc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ibbmeifn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uheqzdxd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2azdrowoq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yboofhqb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2grnjkswa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkzvohaq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2igvkdhqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymvykdfk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gcagunwr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jiwzfsij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2spqdquaf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2huizydfp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bwidzvqx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtbkra.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nsatejac.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hykjcjaf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zdrpjjhk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iihgimoe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tkkwgysz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nmsivacf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ljrrrlku.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ifutkozf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjygmmg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zvygfgyj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xhijjfir.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wcralxcl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uxgykcxh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ebwesljd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ufyjtbav.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nqqtpdtw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rxkvhycg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqqzlfxs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2clwetxps.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2nwhjlxwe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxprizxq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jbvthvaa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zffyavbn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jlnvuoov.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lghqnhoz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzaxjmqz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2abufsymk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2gjhzsvic.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dfdeccgz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfkohsh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ecoitjki.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2erthxhsj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vncvkcgg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2niatthcn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pkosueuz.html


<!-- 参考信息 -->