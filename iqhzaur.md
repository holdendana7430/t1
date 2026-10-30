代发 wailian999

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gbwfprviq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gegnmgbft.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gxlgonmvo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbimfruwk.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gsumekysa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjmuvtrtc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gimrnjtjn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/girebzcww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gwytrbajc.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gktjsbfiy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gugdbshfi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/geekgneay.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/grbaxradh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/ggwlomzlm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/glsdgtsco.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gyfmgbszp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gwpukmtac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gutlbmgmf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/glxscyjvd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gplikuwfb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gsdirindi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gipxtxyvw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/ggupnoumw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gfnuohmoc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gcwgvheyy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gaiclqqro.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gtqlcrfpe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gcfhgnffl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gyrndkdji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gtxkwmlqv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/glwosjelv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gkndcuzqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxjzcjyfz.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gwetiwoah.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gvtpjgwhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gpcvydrxi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gziljfhnx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gsmndaykk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gtyutdmcd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gjlppouwq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gcggannjv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gvtnazmwi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gqcpwwmcn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gmnsknaxh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/glmlsezed.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gmwhourao.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/geqkjqweg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/glzlsnnzz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gsjhsaarh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gkojuktvp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxiomuaca.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ganhkazim.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gdwozqcux.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gtgsjdgsg.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gufmnvxoe.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gqdkqbjkf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gnnqldbwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gkpkylsbq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gvegupwvu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gquyzopva.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gtuaoedfu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/ggiatafnk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/grwvlexcr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gdovkxutp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqeyuyfxy.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gzrbnylxk.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ghagihhqb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ggklsqlld.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gaezenmxm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gwnjjysvy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/giszwpggg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/grjlmkudk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvaciafti.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqotohiqc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gzgxbncmh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gzvtlomdc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqqfhtss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gccprasje.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmykavelx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/guwlysyyt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyfugodhp.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gplheckqm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gclmiatyl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gyfeeuqgw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gmdshyzch.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gpmcofyvu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gaqsufmsb.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gzwfcilcm.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gpopysodq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ghejrhywj.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzvthyers.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gvrowjshq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gkthtyxdt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gzalvzylw.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gayiblikg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkmvpfndf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gxorhguol.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gqhyojucd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsbcmmzqp.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gqwmzsnmb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/ghmbgmojb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gxlaoipwe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gzdgssxpf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gifrlbknd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/greyxmvxi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gxpwzamas.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/grynewivi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gmdueeqzl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gohfwurjf.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gorfifxkq.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gyeougbew.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ghbnlctzz.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gocjvewij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gsiisslaq.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gkhrhybop.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gqkvlsice.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/grrbimpjf.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gidohuyfc.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvrlaakhp.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gckzhxwzn.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbekzeaea.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbcfadnqf.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzxmaafyc.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzgeqbclt.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gjkjhedxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gynuttugy.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gudqvxkhu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/grzbvixyp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ggjhcbxyc.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glbkuecfm.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmqifsbey.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gxdhwjedl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gnzholpmp.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/glgcdorfn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gqqrkfhxh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/grovdwvqg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gsvbqksuo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gtnvuyejf.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gnhoypfad.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gzwzprggm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gcrupnblm.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gwfejerwj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gqpjwguql.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gnrmrgvpa.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gnvxlygof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gtjagjrsn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gubquhsij.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gvqwmsavn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gkqohjvrj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gujtebvpa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gvtbrvgyw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gynrkkndx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gsduxrphz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghhshxxrd.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gcmoundjz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggcoewbri.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gmzhbqueu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gycbhntfx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggdierbsx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gnynminvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpjiclaor.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/goqkjcfom.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gduyijazz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gbtxniivd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfkqztssx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/ghgrwevrc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gnwgobivf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gnfzurvgl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/guduuowtz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gikcayzan.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gbthdnawu.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnspyilcu.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gwxiarjzi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gvfezdpdj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gfqyjqheu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gypjbctuu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/grdoduhhl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmzakzqpw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gvxilcqph.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gzcehnvel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/grycfsgvu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gnndjirxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gltcjfqnd.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gzqxsioza.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/giwholsue.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/goqcphsdx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gslcreeuq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpomkbqre.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gpxwirmzk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gzeghbxmz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ghqacqyew.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gigxwssax.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gzwiqxhow.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gmahvjtwt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gltwmonif.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcvzlfqx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gmocmhwpe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gcwosijad.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gegavszct.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/glmfdntyz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gchtugzbq.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gefutdtsj.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gftuukjkk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gmcxqfush.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghcasrrzz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gbizipccs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gpniqaowi.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gkhycurje.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/grcbwalms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gsbkxjels.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gidjzruxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gcxvdhsak.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gnikgnvio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gujcyagpn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gqkxrfwqx.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gourzhsvu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gkvsowngh.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gfjkeqnpy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gnnavprqt.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gpanjbgfs.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gssexunqj.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gtdnqaeaa.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzfrpqghg.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glrhpthoz.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdxlaqmmc.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzeaqtnqm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/ghlycnwib.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnrbequoy.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/geeoqbcrn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gifgnurmm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggdlaxwzz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsquzajhs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gglavxarq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtthjeuzc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gammqrqol.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmijlxgtj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gofzafajd.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gbmxxsicu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/goonniidh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gayczwatz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/glargxzoy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gxfpyqfsh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gnpqibrws.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gmfhsrhpo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gjmwdqmpc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gmubvnlvw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/guhicootc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/glvngdmss.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/ghxkjfvko.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gipsdtcsd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbkmall.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glhahtoef.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbdgiangr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gzcmepbwf.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ggnqdmlli.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gtemhzdod.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/ghwwlriyy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gsqgdalwi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gexsjzmcc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gbuulpsib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gxxehhnyd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gusdxqbed.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gziqsfgwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gopszejbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gekkfdvzd.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gxvawmgar.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gscjibqxe.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gzcjmoesc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gmxqvcgnn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvsxlcv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gojzqpgbz.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gdexugtji.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gtattvrzf.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gpkfihlzz.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gsfkqnetv.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gvcvvaltp.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gcpkabqng.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gqhbfbklm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gohkoyabb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/goixyfiwl.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gwvlbntin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/glihpmmzk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/ggkrubayn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gokyvlpwx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gjwvbqhio.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gornwojtw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gibfarrft.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gegsktegg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gqtvruvwx.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gocvixort.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggasoinub.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gvgqusxqb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gruqiufyy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glgiynkng.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gcprbobzb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gkikqmexm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gvkfchqbj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpcpyosqy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/glmxovtol.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gnfjgmbgr.sHtML


<!-- 参考信息 -->