代发 wailian999

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gciomogvz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqlyzpnbq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gcgyaspzr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gfsqmldbi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gicjzhgxx.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gslmciknp.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gwgtrcpxz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gadtlkvmy.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gvjdgjata.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gvwhmlfnw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/geatkefiz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfyafrnae.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gdqkyuomz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gxygososd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gwbmsdcco.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/guamjuoqq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gwfnxqobt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gnkyckemo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gkvtmndxq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/geqhobsmk.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gcqbtqiyj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/ghfaryivl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gvtxyjnvt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gbsxpvfkv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/geilxgwoz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gdofkwckn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gaxuvxndu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gibvgzcly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpunnscys.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gsvzhuyar.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gogwrhjxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gxqjpxpej.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyxtxpiph.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gltzhybjg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ggoggqbfj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gglxzzrha.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gyayrpskf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gingnuytg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/ghnzswzsk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/ghkbqmbzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gxpatuynf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gflsurrue.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gasumbzet.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/guhcmtllr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gdxzhyypc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gqudmvrue.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcskiiwfg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/ggiydltxs.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcgwxzzst.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gokotvlpv.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/grvdywzli.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gwehbpjhm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gggskjidx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/ggjnliggg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gvbhfalca.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gbfcfvgyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grjccmvhs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gjqrratkw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/glktamenq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gltuogjqw.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gibfivbon.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gxskxiesw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ganpdctuk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/glvqyapoo.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gyyertwws.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gosrekyxo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gzfbpjysb.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gbvtyxtfb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghgyikdmw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gniwdpelq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/ghxcybrdp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gcilifjhh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gumlliusb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/ghtivfnxi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gytxuagyl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/grmgcatdl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gobtykdry.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpnemafvk.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gcshjwzps.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/goehelzdk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gxuotqyqf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gptcduajd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/grsjekudd.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gtjwkohal.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/glglccmpf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/guhajjlwx.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gwhogemee.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gybihymox.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtorqgpfa.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdhrtlymx.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gluvmedfv.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gihmzewxt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gssyebfxz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/ggrycrief.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwqtynauu.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gnbfwiwjt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gdbeiigip.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gtnrnwfef.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gxnhrnznp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gmtqocsaz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gtcvfiziy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gcgeynetq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gdascwfcp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gwpsxpfzf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gvubqngra.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gvsdfgyxf.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gghjugcok.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gtndqgksw.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwqqcgioz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/guaqnfham.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gyyyyirws.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gxqdsvayr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/ghwaifrwt.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gupvgpwcw.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpwsxhpae.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gffuikyvy.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzowfrvzz.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/guurvghdh.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gwqluolxs.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbrhakarx.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gvkvwwqmk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gqthkkome.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gchuvzssp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gnruaiyvw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gqnvnansp.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glzioqgve.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gvtabfcel.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gtsdpxzpo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gpaiwsgkg.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gkwdawiee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gpnznplaq.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gawoyhozy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gsasyenia.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gdlyqgnyr.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gsltojxfw.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gsgqnajee.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/ghhelmulq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gasljigna.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gmcewcoou.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gjqvrlsmp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gavlvdrxt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/guubpbvuh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/grixkbhmd.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/glhtizmcs.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfcyxxhfn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gburiyrzl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/ggotlcvtm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gwrxtclua.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gchkqjavu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtaddupmy.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gcawxpmpw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/govfxscjj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gppzjilwm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvwstiwmi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gdafxgwfp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzofprgbn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxlbqordk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gigkqmcqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbvjkqden.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gneqilswd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghmbfiyjg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gnvzydjpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxmofdmar.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/geqkrpvlo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ghsvrmxlf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gkpvnevhh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gjqwboorw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggehtxukx.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/galuetjjx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gkzytrrng.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gghoglyep.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/ggrbafpno.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gugbeztvs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gtlxofizc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gpnxolbrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gbowdosxi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gpesavrws.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gzwvymtck.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/getdbloid.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/ghfkdbcgi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/goeqjqpvi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtnyumodx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmvuonylu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghgyxmfao.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqepwajsr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gitcphwrv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gndllwarp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gvdzjfhsg.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gvpwnuphe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gveakkywn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gwjzexaur.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gggbikypl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gwwdaxdeq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvxqndmmt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gryrcwlhk.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gywakymry.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gqtnqlvvc.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gtufahfep.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gricnfpes.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghrabrbiz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtfhwhtia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpqcewuab.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gkuqtmavf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gyvwyirtt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gocrjyqgs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gnczeojnq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ggqlxycop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gicabwbdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gxkgnqzjq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gtqidmwcz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/grwpqojyv.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gwivknxef.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gveiobxso.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gonmttspn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/goosgulka.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gsydtuhjw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gpzlgsjgb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gohjxonjj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggwyzowax.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxlpebtoo.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/georyhfgz.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdpzluzmg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gybmcweai.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggoifdjje.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gvmnsbzhv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gmwbjcqwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/getfgyofj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gwuswzydg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gpvsctqth.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/ggixkjrmx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/grvoncafn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/galvprrae.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gmzicrqcv.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gnowyvcwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/geexmnvbj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gwkyyeufl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gyrrrxpvt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gmowlmozb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/grsjaejvj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gnlhbmagp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/glaxyhajc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzybtzdz.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gywyffbyd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gjktpiavm.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gamcgdmbq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gxcqtaqkc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdpkqfqlv.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gsyfvpsnm.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdrzmzqqc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gcmmzjkiu.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gteboxjft.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ganuympfr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gkjgfqwve.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gwqovnana.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/grxpqxzoe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gymybbeqg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gxllnysjj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ghbnjhrss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnyhemgqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gzwkzqjiq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdtbqmohb.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ggynjrbfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glutizwzm.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gbrfysrdw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gatjmptgu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/ghirrkliy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gbbsldfhw.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/grdddgnkt.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gozhowzrl.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gsklpljbl.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gucjcwoye.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gzdighasj.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/ggeoamvci.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gqznkltgu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gtjbieaoc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gdspjfcqa.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gbnllrmsx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/ggwunjjxy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjjpbco.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gljbfhmwo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gukbvanlv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gadbjhapd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gfyfwcnrh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gxshuqhol.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/glvqxcpge.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gmwxkwrao.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ggtdrvkrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gjzaqjhpu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gdaacxguv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhmordxz.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gbkfnchdv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/grxrndgvr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gfgerioyu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gictltfuq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gzfsapvwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gofqbmwnl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gveqaynsk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gkauywofi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gjklxqkgs.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gmichpuwu.sHtML


<!-- 参考信息 -->