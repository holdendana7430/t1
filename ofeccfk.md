代发 wailian999

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gtjckkwjb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gwzeonzdp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ggqgercco.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghvbmfkib.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/ggwkgiosq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gabyumomr.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gxhidisyd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gdmdeuchh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gsvbfplaq.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghwmoonaw.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gtznuoceo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gqnnkqeov.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggswpmnqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gsmddhwaf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gktbreqaw.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/glbamhjlw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqvhpebtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gtpzafexe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/giedquiqq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gudwjelep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gqndydwbo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gzlsfmmgg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gwiwsrwwe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gpbybmtzr.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/ghymedfaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gbfggiezd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gliicglwr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gylrfwhus.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gaipqyfii.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gspmsiyun.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gewvkiuad.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gbvvveqid.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gwpdarkob.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gcmprfrvb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/ghhbgmwmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gbzcvibac.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gduoqhdqa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfalsxowz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gqtoofycw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gvhjskfeq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gvmcsyhvd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gpiolojui.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gjvdydsrt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gksyvnous.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gbukeacac.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ggtqtnmcm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gyvsgqpaq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/glzhwmnga.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gioqtreqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gdqfrvcxb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghzayadgb.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gcaljkoig.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gyusvhtaz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/glhuvdmgw.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gkdirnxcj.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gynsubqkc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/goyjfskwt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gpdgvlzbs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gnuztyotu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gozwajpcu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gshaxqzra.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gxnovlskn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gbgwjkuog.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gzameputb.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gjanmtknn.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gkeefmhby.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gtdgrmkxq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gkmqxioqz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gyjyppmik.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gzwcrnpuu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gdwsrbhpc.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gmwhfdxzz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gehwkzavp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gudilrkhh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gqwdtlkxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gstaissyv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcrhbmnk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/ggnorrpwp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedhckahc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/glsbxfxzz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqadmsoyt.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gdlqrcdzs.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gyzypopam.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gzagllxqw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gjttqjrkn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmvsewezd.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gbefvuhgu.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/glyzxyhfw.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ghokjqeui.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtyntxzib.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/givsazahj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkymgkgak.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gttdezoln.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gqrxokxwq.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gpirjjcqs.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwytpqark.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/ggkcxpppy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gplpbnsgm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwdknulfj.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gokcvfvav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gtrzxadgb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/guwqaoqxz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gawyeektx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gzabggssl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gidzytdqn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/ghvqblfmf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gomaeiiee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gclwzkplt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmoihuzmc.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gabcubzff.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gebnmnicr.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gbbufmyhd.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gjtjhhtii.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gvkebcnqa.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/giydhmxdq.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/geelpelze.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gdldfckwo.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gbiskkcav.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gupbamxts.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/ghqvwowka.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpdyxnvky.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghgdmbncu.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gktozbaxe.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gvygbwduu.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gqzcjjjzp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/ghrolelyr.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/ghvuymshu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gtgphhtki.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/ggmxvbmeu.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gkmdsuqnr.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gsompoqaz.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gsldvvmek.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gznsyxqpy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gmyhhnarh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/grtgwqkzv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/goibykgah.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtlflbt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gddwisvmy.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gyiauzaqi.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gadzetwhr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gyeqifref.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gxcadbkkw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gybcsrfer.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gevnvsiyc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gzkxupntq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gdjwfttns.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbbfhjlnx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ggigfdwmc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gnmybnwbe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gnokmzkcz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glbdtpsmx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gwrgtlrae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxislzv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdjgnohqw.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gylrertlj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gslrgptzi.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gsgfuecbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxesxfjem.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxgrlhzec.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmprbfjaj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/glisfoten.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gatyoumxx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdphohlyp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gtoqkuvxc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtiwyusgg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gxzdferiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gylwhbmip.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gljvsnxpn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/giaeswqdy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gxxxhvpap.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gtitsivdt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ghgcwxlle.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gdprwmzus.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gvoyaukng.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gyghcdtwe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gputaoufx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gvcjyqjrv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gvmvzwlln.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gufzopfro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gvpehcmzc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gnahsbrin.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/grfgoskpu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/geuczjhel.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/guafgtjpa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gmjuqrdij.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gsruokeqa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gazrfgzos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnvwodjmn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/garhxcwsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gjbrtvvte.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjblpyvsf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gcxlzlnjl.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gcbkpomch.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gropztdem.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gdagwwwsc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gwwbkgule.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gyddrioas.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gbillzhae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gtzvuoxpw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gnvkkwrdn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gxgztuien.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gyxamwqdn.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/goouuhfpk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtfpazrai.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmualzaou.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjhwetpdg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/garcumnvp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/geiawjkin.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gmrvzmkqo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gqggxaesz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gfbwbmyos.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gaoxzjznc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gjqauousg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gcrtvkwzw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gxoitenuq.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gizajeuar.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gswkpnbzg.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gbjfggqlt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gkvgvqyfq.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gejxhcmok.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gssjxunnu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ghbzjblaq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzmdkugjv.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwzaeiufz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gukkvvqku.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyioqffvn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gwnpnletw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkaezcwog.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gwchqxwdy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gmxdcbtem.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gamgluvdl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gadazodkk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gzfxosaiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gdyhbxhty.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gtiizcpji.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbfekjaev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gdxhhrxtp.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwutoaeiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ggwwzwpul.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gorwteuxg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/guggmlfnc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gwofqgyeo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/givlcxuvt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/ggvnpilbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gbcmepwqd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gkwlcbwub.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/govbljxdm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gludwkclo.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gfmtgcufr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gacyiodfi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gugufxuul.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqfxfuagy.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/giotyivve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gfhfppfby.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/goicocqwa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gzrnkozdy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gxzedgveg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/glsylylmm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gpukysczp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/ggfebskla.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gwqkilivx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gdytufevt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gcaikuydp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gqjshpcyh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwdhvaer.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/grnfgalqm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giiuqknsb.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gpiizigej.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gsirtnlnp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gbpazldxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gegizbemj.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gyhydoxhd.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gpwvkkmyg.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gtdspfjuz.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjajvvwlu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gqdhumnvm.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/garaibfvi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gjlukjmit.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gwfxjpzhk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvcorimjz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpxwbqrvq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gqzwzpjxx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/ggckvzhdn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gqdkytiry.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gblhsohla.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gjazntcvs.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gzpgqjiuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gzhdfkhmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gofptzape.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gtzrzpbcp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gjwuraiuc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gyvtywchi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gqhybatti.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gpfzybruj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gejhjptwd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gxcpcnqsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gyfjghgyw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gidaogink.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gnvdjztgt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/grivusqyw.sHtML


<!-- 参考信息 -->