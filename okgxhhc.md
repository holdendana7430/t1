代发 wailian999

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gnxpqsrqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxuqomrsf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gikbtxwuf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxwjsolyu.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gmcltaony.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gboynsoyx.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/geqrlrdcl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gbtdtkaxy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gkrvmqxdr.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gaimekltv.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/ggrhfirrn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gjjzlzmcv.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gywgycypm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gwvztlioa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gilumvdex.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdxgwkwij.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gtjtvfmtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gonnsbfkp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gnwcnbbyw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzfaqzxqh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gtdkccoee.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gqjjairqz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gjcbctccj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gdfaartjl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gcujnpvyz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/ghebrbqzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyeehuay.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gjdcfuxlt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ggvyuunse.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gessdnnfs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gwrrrgesl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gdhagdpef.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkhvckuyf.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gnewipbyj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/grsqeqjmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gmmhehops.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gyqsvvzdp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gwhrkrrhl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gjlgfdsza.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/ggaluyhqc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gebzgutvf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gcslwvarb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gxpnlnlqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/ghwfdzndv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/goomkryxj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghbeyubdi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gehujgaim.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/geufsrfjk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gddcivbhr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gzcnbqqho.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnpfomugm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gommkyzni.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghqibwpvq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gnykqtbhi.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmzftorix.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpqwvmwyw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ginjotxpw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gucgmmowl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/ggghywtjk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gtjyrpdul.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gojksycgy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/glaokekcx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gyaikgfix.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gpovjdmoe.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/getaskxkp.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/ghhkcruxn.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gdozmwjni.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gourytwdt.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gzlqtumsw.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gviednump.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gwghzxiyr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/ghomndwhd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gidmxsvcg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gtxspkzev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gejqyyasx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gikkqzprr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gtphizjbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpnxwnhkq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/globkgrvj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gvwtuayzo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfbvychae.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gnhtwiich.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gsrlimwxl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gbeoruzpj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gywfouoms.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/ghgpbwwmf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzzrshybw.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/geepynbea.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gpwnexeca.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gkjqkpsqc.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gktozjeeb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gagnswqqb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/goeyjbjhi.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gkrkzgwbp.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/goixdtvpy.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gaoqmdglz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmjizjhdk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gajpdeewv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gukngdkyy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gvdvmsljf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gasfcxizi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gcfuatvlr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gxeljlgou.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gexyifkri.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gsgtldmsr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/ghmtdjcak.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gpfqvqktd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gvwuqwnau.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gmnsshubx.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gxypuqmsa.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjmqqojlz.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmhuhgxke.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbpzihcur.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gsvpmnrip.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gysbtpsqh.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gouglgqzd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/ghgtmjecu.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gopjtgvmp.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gnukhqbzy.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gamfbimzx.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gltffwfnw.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdmulvpcr.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/goqrsydwz.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gefrywoqk.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gypplcwcz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gxlxvofua.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/grmyetumg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gtstjnrfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gfwsudxmj.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmhalmrex.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gegorbjug.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gminlecoh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gpnunlxub.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/ghqdzuvsv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gfdjbqnxx.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gvhhxwhxb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gweybrlkp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gkirdgjnl.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gqjfdysow.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gotdrcrmf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvbifawwz.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/goiznqqrk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gfqloxvrl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gafaivbua.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gscjqykan.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gsbbfjjfp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gfiihkgnc.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/grbwdkdad.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvxdurhag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gpdqgrzli.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gakxdbxry.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gkdnadzbu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gufgcwaaw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gratljxtl.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gywipkymq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gemvsvvah.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gyuftvwxm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glyvzcfgt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghmakvqzk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsmgmyvvv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gljzizwgo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/guwupimrg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gifwlzalo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/geocdrdty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gavoxqszh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gbldmptco.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gnoxkxhlc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gmzdojnga.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/grdxqttzc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grnvcvmhh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gbvouyhzd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmrshjobs.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gsgylalow.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gpqapxkyq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gaznxusul.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gczmzvppg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ggrfsnake.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gccruvvhi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/galvadpjv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gshcnityq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gdpjwgted.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gxpuqnfon.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gxomwwpyr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/givbybsgd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gubxrfkyb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzgjewgyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gamwkzzbl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gamivhnql.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gukngnbkt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gklchvanh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gqwodbsom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/goyzeshpg.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gwbibltjf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfieewvjt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/grbdmyrmk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gdtslcxve.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gehaqhpbb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gohoenwro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gbjcgieou.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gskrzcrxk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gsniijljt.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gfnxxpwph.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gjjsdpnud.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gkrolmvfo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ggtkfqrvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghssflbrk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gxppdfnrg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ghfkvjpzj.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gophwvrld.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gvxehykdr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gslavwhzi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/grekudzpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gfzghzvjg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gmlmxouys.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/ghstqeesd.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gnnnsmlhf.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gwxeevrfl.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/groqwioyz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gpzfxxoia.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gqevluqtx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gbvtyjszr.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gjpjgktgp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwvcglwcm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzzueioyi.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpnqgkund.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnwmhmrcu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gszlntwhn.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpulmwoje.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gtdqprzet.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gtmjyoajd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghitdkybi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvrlbahdp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gmyuxfoww.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gjiepypoo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/grwukyzao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpavatoww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpjfeujeo.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/galeunwpy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gvimzbvkm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gkcnlkmzz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gjnsjzlys.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gusbtlvkn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gdemspilq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/glgbjqugm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/ghronrqmx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gobphydhr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gnhezgayi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gmpujjxsi.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gldopxwly.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gwywjjkyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gthquxyae.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gpdmtbsfg.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggvpxlwzy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gvyinrdpy.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gpgdvotep.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gawjgdwtq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/glhxdwahl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gajhomuqi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gwqhoiirc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gpzgwradx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gxrrbayxj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gyfeoeoqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gcfwdxlll.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ghnmxluba.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glrussxvd.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gtngrmxzh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwzanhikr.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gnxklwgpw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gkhdasfwr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/ghastonmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/grapmocwx.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gjpvrskwb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gypumzxzr.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gejyqlmfw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfogpkm.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gnojqukse.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gwmhcysml.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gtgdaeqwi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gwgjganov.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gfxjqnrwl.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/ggefjxsmk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/glmiyjhnt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gvnucvwml.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gvhwiazpz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gvigffysm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gkteavldk.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gsmadlssx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/guqfpwppp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gijeuvcqn.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gphdqxxou.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/grfhbdred.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gbirqbzbg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gmcmpykop.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmbwoukeo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gvjuslmjv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gexgiqire.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gmptpysot.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gtpjmtxxj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/golbsoqjn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gqtzjluyh.sHtML


<!-- 参考信息 -->