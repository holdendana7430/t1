代发 wailian999

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gzfjedshx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/goppybkac.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gshvkcdxk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghhbjwzmc.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/ghuimkbiq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqejjkysp.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gqgppbfoz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/geowqpcpw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gajvphqal.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/ghrlxwshm.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxtygbsjw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gzdmyldah.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gulibyvkx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gobzpclvv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gwdprvtve.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmesictwo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gtlqtjcgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/getcdfsza.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gmmipmfha.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gleerrpln.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gaafjeryn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gprtaamdr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gmalnbsnx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/giupchdre.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gmvbsgzob.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gdzbnkjri.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/giorasugi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gptqekzcp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ggmdbewqz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gqvwuznsk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gjqtgumsc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gawftmmju.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gbmqxpbpw.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gwmxsslhr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/ggfoaaqrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gnpgzevcm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gnvzozebk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gruiaqbyd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gxuxqhlij.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gezrzvzyc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gqrcjrgkk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gbpmacqdr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gvxhhfixf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gaykxjmvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/guzqeawjc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gpeuuphba.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gfkiwhssh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gvigvsvmt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gkuqqucda.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gjsjkezer.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gupdylkzv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/ggpryusfj.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gdpayunii.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghaxcnyfs.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gvpflmgsc.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glchevaxd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gbirniupb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/goockkzyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gqwxleopj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gclzfubfw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdxgxupks.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gxubkkhhm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gwawgsvtj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gwurogfcq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxwpjcumd.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gleayoylt.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkzygpnqo.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gjglywvvq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gjwfsxoca.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gpvjfgbyq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/goylijzjc.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gmzkmdplz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gcchquerq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gxtmpjjrz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gozpoimsn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gfnfbgcrt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzdrereys.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/ggwfgsgmr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glwnvinjn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gtxchwqrz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcapwaapz.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gdgczwkek.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gtmoavuex.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gjdkphrja.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/geyecknrk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/goyasuvrs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gjakdxfxr.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gsgkdmfxf.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/giganthxj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/grdqoceuj.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/ghytyvdir.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gdexzxwfq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmnbsgjvm.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gecwhaifi.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/grsmczgeq.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gkuvhbmrw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gmzwwjkil.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gsdxfcfsv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnpmhmkot.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gnlombidl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gryecortb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gajfcdllj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gmvwwjkts.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gpruzlbvn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gznvpervf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gnvyygqcg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gsfrvkjso.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gbwxufovj.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gxeanhabk.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/guuvifbup.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gyklbpufv.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gfxdrupqn.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/glthwjyyz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gvnlfolev.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gagswtbiv.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gggwferrf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjyfafhgp.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gazfblzuv.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpbdahfys.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gmoyonxpv.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gyfcmfvfa.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyqdbrbzs.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwlijkh.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdmgjuofl.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gbglbpsxu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gjnolzxom.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gynmbqjji.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmuqslkak.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/guohenwqn.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gispwwqgi.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gdisnqdcv.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gshvrctnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gcczunlzo.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ghqilsuri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gwaddyjsk.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gpcbhpqbm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gbnwospgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gvkvytxjy.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gqyptdbel.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gylnxpfob.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gsctfmidc.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gskjdniwp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gkmwvziyy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gzcckwtpm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gkcxlcuhp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gilpagqrx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gpsoeoovx.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gikibjbnh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggurvpkfq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/ggmlfzrac.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gdozdjigh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gmcamohjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/ggvcdaemw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gixewjejc.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gclhhtqma.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghfuiixwl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gdsrzdfle.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gufomofvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfdzzgz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grqlrfgyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gyvwdtaou.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grydhtddb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/giklicdah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gtpqepnlt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ginxbsgea.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gjhpbhrdv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvkwiuecp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gfhppguna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guebtftvb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gopqczbjo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gnlfgkdin.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gjrzfktnk.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gxktkbnet.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gqxjuwpee.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gmqtxdpzd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gjnqfmfgo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gfvhfrmkz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/guqqbiqkz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gqkldnvwg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gaxxqpplk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gugsnslnw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gfwqsrvpu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gwbslhbfr.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gqljvgisd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gywgfkuva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gsljhgnie.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/guwvqegye.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/geileoejl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/grhoodgca.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gpavudbck.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcwvntrmz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/grgnmrduw.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gsykryoqe.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzvobjzif.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmbbvujbt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gczwlgpfr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggbmxtwxv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gshdltknk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gasmfoymm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gkxgddfbj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkceezaxg.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gkuxxzgbv.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbguquyoi.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/grzyakkkb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdleywgpv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnhcebbjh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gajmqvwut.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gfnhhlbux.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gwhcfaswf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gammnqtmd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gqusopgfn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ghplcyren.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gksnzklxl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gipgmuozi.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gptpdvved.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gwxqdyclu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gsqtfqoqh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gwxjbrtqc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtjnlzklu.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gweloyusv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gtszuhrsr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gvuznrlqx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glgaymzys.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnacobfap.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjzjwezyz.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmstargba.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gplmoqmkw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxndgdcor.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gmkexvleb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/golngpwbm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdclnzune.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggyoktcdk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gddnenkgo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfdaugzbg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gqaphqpif.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gazkrnott.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gnfynowkl.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gabhefkfw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/guyctyqqa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gxykzbsfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ggpypzjoo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gpkuzthwg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gymvfcmsl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gruvgfzbv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/ggmtxogep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjrdxdcf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/glrvcaugt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gfshmfqjk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gjdfhmdtu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/grjgdkgko.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gmogmppqo.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gcrmidkpw.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gywotkflu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/govscttkq.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/giaiphzuo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gzycpgaws.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gyigeunkt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gwuqghmxq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gkqmfhesi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gxyhsomck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gpadrgntw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gqeivocuc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/glqaupgnv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gcrtdjstt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqjkjnej.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gjrgbabyn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glwvgovcq.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gzjscutlp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gisudkxni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gvpabtfxo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gmzsumuba.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gnzrmecdo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdbhfmfrj.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gkrachuwp.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/grcfuznxg.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gokjthfgy.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gmoxzybqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gewhgefjy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gtzqxzqyn.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gnivnuanh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpsxvplsy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gbyhzcber.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gkvwewvbs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gpnhacckw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gxrrwqvtp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gdrzvhfel.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqmxlaoqa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gvdnbhwbw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gqcpajiep.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gqdegkcii.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcuvoggid.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/geqgdqwdo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/guarkbfsb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ggfxpvser.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gyovrlebs.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gmkuwzmnm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/ghqdmrfsu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfzuflx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gtdtbsdtg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ggfrqbfbm.sHtML


<!-- 参考信息 -->