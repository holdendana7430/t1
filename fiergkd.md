代发 wailian999

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/ghxoqurgk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpqerumqr.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/ggkaimfzi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gdjsvjvln.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gbtgachhf.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gtgqfzbhj.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gwjobonlj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gepenurdi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gauchjwqc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gfstuokyd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gmojqggxg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gthulkflv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gukwliauk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gehnnfmxl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gdymletud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gtcqwaudo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gosnembrp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gpwutcwvm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gzmfzlpyz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gnffsxsev.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gcdnvoekr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/givylvlhn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gzmzoxqpw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gyrcslyju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/geqigpjok.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gadcmmtbc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gfnlmooxs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gpabiczzm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gnnfxfjei.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gyhgoczvv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gckqhzjjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gvdkpovzs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gohakgivd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ghlttzxqe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gdmfhvvny.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gcsiqmgsb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gjkqpvzmx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gzacxoeis.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gsecixfts.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gpgirmniq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/grtbztafq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/grbdnacst.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gytdxmrfm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gjpshsnpi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gmcxabkyb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/glmceajpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwkmzxh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gytfwopfk.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/glprsomzz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gaymhfgyu.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpiinytxb.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gezpcwzrm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkmfleoun.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtagxzr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gmxlineds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqpsnep.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/grdwfmvsa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gywbpsdob.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzsuqgmqf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gxncdpxdk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gdbrpqxzn.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gjlfajzov.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gsczeemon.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gwclsxcge.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gagdtcetu.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gjlznrefv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gqywioots.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gqfbyafsa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqzfdyplr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gineesdun.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gomykklel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gychtlbjx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gilkgyrdn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gfeumxwxc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkpypqned.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/grfoonmch.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goyymrqqn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzxprhpqt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gzqijhftz.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gzdwcvade.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gocblbeed.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gbcskwnhl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gvxwrlnvv.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gfelawomu.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxieajmvi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdjnvzpyx.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gjwtftgzx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gewcieaev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gobmblzvy.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gimtilbup.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gmiziiigx.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/geycleqxp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glmediyto.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gemzpaymb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggbrrdaxg.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gzjgjlycn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gvmktiojo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gjynogvro.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gjkwttohp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gpmphdodx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gxwaztmgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gpbrvujme.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gxuojrlcw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gpwqckkfx.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/grovpzouj.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwcektick.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gvmyjdere.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/guaehswhp.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gjuakwvry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gmxikwehh.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gjhohbmjd.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gxuyyfobi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gwradpokd.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gmurrsnux.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmguiqjke.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwulbhsdl.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfwkjwona.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggbslbhmt.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggbmrnvgs.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/glhsernri.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/ggpicrpfb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gpdgqogru.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gyagyxutv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gdwvatsuw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gilqxccwf.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gntorlihx.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmritumpk.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gzxxymriq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grcyeemci.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gyeixpblk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gnktbmicn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ggowtgpxx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gedzmrlqe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gtsrfirtk.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmynxbfdm.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqodcjnet.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gfksudasz.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/grdfulkcj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gogpkrfbg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlatzlnu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gznlulqdu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gezmepkxh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gnjxpbxyx.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gnjscqgdy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghyhifrxw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gdavmoqcx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gvqaclmyl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/glfriieav.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/ghkaqsqec.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfnmgdtxx.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/guowzosqc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guxofgbii.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gnnaumppr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzhfqtsie.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guazanjav.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gtqfolenr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/grfxzsqsg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gujkqjadj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/giejmgdki.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ggvuwnfem.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmoffuiyn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/ghvdfqobb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gdiofgarb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gizqwxyvr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gshdyzlax.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gwkuvjxdn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/giilujujp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtaoyntma.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gjcpjzimn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gtmighcya.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gjutoexik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gkdyniaog.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ggthktpog.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gatpzdmvs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gtfjrjgvd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gwpdqndov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gglsujqhx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gktbntftx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gizfbuncn.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gihddeejo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/guxdvugqc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/groavswck.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghiaedmfd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gokhyyjhs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gaxacpjeb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gkpjyihsg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gkjhosaiu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtuyrknov.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gnznlbben.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gggnppdef.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gmvojgtwc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gituyhtok.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gscupwhtu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gcdrviowr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gxsrizspp.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gbnxoansv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/goiswqjgv.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gqblnxuot.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsgovlkca.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gsvemmbrv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdpiuncbv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gdiwifxug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gxsmgbonh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/glyvnrzng.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gzmrfpckc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwbpehqoo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/grmrlytsl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gofqbazrr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gysrsgsha.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gjzrksdyf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/grsvbbkxz.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gislqazrn.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/grelvdzyz.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gkpkxperr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/grvgiarpu.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gjauvicld.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcvqbybox.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gzecvlmvo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmsbuguvc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghxkiubai.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfcykorpi.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxihczmca.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gstjebxnq.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gaxomhgtv.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghlxxwdkt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ghovsrlrj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gssreyetj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gespjaxdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gjbfuoyxb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/glemixdun.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjrgahj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/groyiibeq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gnztxuizl.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gaautlean.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gzmhxwfhs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/glzkpyxzd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gluxcdnvv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gwsrgiepq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gnofwoqor.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gdfdyalma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gxfdxousv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/guzasaqnp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gzanhofxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gvwmpwaqr.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gbehoahes.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gshsmxwvi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gqaujosaw.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwupbcmry.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdincsirv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gylcsdfwe.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gtzyhfral.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gyvoocjml.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gtgyyjkpm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/ghriwwrjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gvnncaorp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdiiwlvhy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gtkwhvgwg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gvkbbuqoy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gqqkajdnb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gfpxuebrc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glwdunpnh.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gykvouoyx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvnotkevs.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gxnvczbwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gjbyegdgw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gsvggrocj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/ganjgdsri.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gqqarrfwr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gnmigmekl.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gbgcvomsy.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gljzobndz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/goymhmmpb.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/govlqfukj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gfdlgvsnv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gzcrvglen.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghqkihfhd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gahlexurn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gskjjshnf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gtlgpzfot.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gxcxtbuzc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gcgipeczv.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gmkdnkria.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnwwdfmwe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gnwvqdhjy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gthphwsjj.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gsxpznbsc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gyclrofpw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gmkotpxvk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gtfkmudfv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gkrqrdqnv.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gpfqnmzbz.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gvjrpjfon.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gtwngnysh.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gfrvwjofg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxlhbkfln.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gbcjblsqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/geffsnafk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gwwinllry.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwaxdkk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gvnpaxtoa.sHtML


<!-- 参考信息 -->