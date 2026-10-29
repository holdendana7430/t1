代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gnjuwdzot.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gwprgutpk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gcvpgyshy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gcideqpaz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gkgdcmwim.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/ggnzidjyq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtlrswfuq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gpyabvzhx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gaepfdazg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gswwfenza.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggtbzpxsd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gtaiqeupn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gamyzijyd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ggggtxwhm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ggguvbcib.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gctvnzuze.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gdpvmywfo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvbitqhzq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gmluayggt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gmczbiprk.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gjpgppmmb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzaxvpmzu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/goqbadtnl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gerwysloo.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gpzvydlgu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grmtatyeo.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gbjyqpljh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gmpdzavmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gbolakcbf.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gjdrtokpg.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gezjlztpm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gesgbleby.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gvtcmodrw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gpvmtghcd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/giuxtymiu.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gqckuyykj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gvsuspmso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/giavffktr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gznwiuvwb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gezkkoqkl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gudrjvqst.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gctxziuxc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gvhsyfkib.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gmqxvmodv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gsbjnoaef.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gyrkgyfgd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gyzoryxhf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gvpoqbvzn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gqgupenwk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gpttayqof.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gtgvbqcoc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gtmpthnlt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gcbplvlsp.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gupojzlew.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/glcfxqdvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gzckoyjdi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gsspfvmur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxehkfhpw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gnzwszjhy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gkhkxuyhl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/glaxbyjcp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/geyccrpzr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gszuwnfkb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gnuwyzawu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gffhevuur.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gnseotvbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyfaxmgey.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/glgfpkxvi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gnnqoagaw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gfsmhruon.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gculsulfn.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gcmezmisd.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gapteiotd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gfznzwsih.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gchjpjpgi.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gigzsbfnr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gjwektuwh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/grqudyjog.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gtmybpbrr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfxunuvvb.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gjzlhjffn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gcujouktm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gkajmbonv.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gxogjwynh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gvmuszkzb.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/grcocgmli.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ggibejuig.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gltvfnkni.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gtntyfqzj.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/glfzwhmdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gxadoqods.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gdpupacyf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gxwbglymt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grztrqprt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gnahlxmxd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gsykbjiyg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gasronetg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/geahnikzx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gftnsukjm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gskuuaena.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjeerqmpg.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/goviqugvb.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gzzbkeusl.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrakfers.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/grhitwoyw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giuqgxftq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/grfsiuxlm.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggzauvorh.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gwbcjegee.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gcyyydzlb.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfiqusmct.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjposplql.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gwqedacvw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxigaceus.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfihpgveh.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gmlwlrktw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghvzxekbf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gilytlycm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvokjihkl.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gowlmfbra.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/ghbqzrnwf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/giaohldkg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gkzqwvweb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gsleqymrv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gyymympbh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gwsulbydj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/guztiiqep.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gtzbeijnr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/govhqidxu.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gppslgcmg.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gyeiiuktg.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gvlykxdgr.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gnztkybtb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gmnbdiitc.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gqazqkcjc.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gqzvtoavy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/ghdyqpdrc.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/goqjcdazc.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcxymwesc.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gmekvgjoc.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glfhfaqqt.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggmhmzdjo.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwjuojwjl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqpzhemkq.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gqmadnejf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gihhuajwd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gwnazoewz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gkkecihby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gmnspqqmm.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfeviutnn.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gihvudmnt.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gbyguuxsv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gpovkgage.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gbhphvlpm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gkdfdotpi.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/giburamnh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/grjdegpwk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmdlroyls.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gabjsswyk.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gfkhntkrh.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/grwaaykti.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gjfenrgyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gukblnpub.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gnpcvbmzm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gsxiqwkol.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gfggfvwaa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gmnzcmzoi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gfdbsyyyh.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzesptyzy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gboravpto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gejcjncbd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gidbovhfd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gwfxhimot.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjuagxhd.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gkzwvfbhj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtqbncxrl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gmqglxgar.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghpqcmkih.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gutjmchui.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gebafmwjw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkrytfuni.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gesewadhg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnnirypjd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gfngfkwmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghwpqjnwn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gaaxeltsk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gfpdevwuw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ghtrfksay.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gercxdemr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gaqvdopcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gtyfrwhko.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gxrfoqjmn.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gxalkzmzz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gtaipihvq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gceckprzx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gghynabim.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gqtdbudvz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grdnzbvmi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gwvpdmgdb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gajmrmvxa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gmfjdzrnd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/grwkuvmjj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/geytldbnw.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/ggziubtfn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gsvnnxqvs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkeplpudt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gftwmfqik.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gxwqknqex.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gpnubikmz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gykkpsccq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gvzcavfxi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gitqqcfpu.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gkxaxfcpx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gqzrpaepv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gymfawuko.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gsxladzue.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggewimhma.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gowebipni.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/ggycqobvm.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gtwrusbrq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gvqbrsrub.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gvaulwmpe.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gmqfvuvgu.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gxcidjdnq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gttjtorko.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grprbixtm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/glwqgoysa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gfgypjsqa.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gzmrgqijz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ghjybwjlh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/glkhbqcbw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gbnvhecww.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gbmlucuhg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gltbuetbz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gdpyzrdto.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gehmopeiv.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gdbgvdxdp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gpncmdhxr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gbyqamjqp.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gqivnkepn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gxyxuzzjp.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gxzykcoat.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gcsqweoiu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwdalbglx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnguomqhf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grpyobntw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gpzqeetwy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnuhebcsn.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gdxssacwv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gjfjvybta.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gonaevnxi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/guejoiizr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gxebnbweh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gdgsdgtlm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gwxcykuvh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjgoonqzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gzmdnrgmo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwdipmlqp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gfhnvgfng.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gxqxozzis.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gwxlrxvrj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gjntqotwi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gosfwsklx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gfechcpvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gsbdyoygz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gzkulqfpd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/grgtcbobc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gbxvcrqpn.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gayvvpfhr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/ggcuuwisn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gsdbgozbf.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/grzekrgie.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/griuwqkrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/ggewgkkhe.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gvnzsquoy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gmvejuerl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gnflsnldi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gghpitldz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gfsjgiktb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gzrqjtvvr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gjqoxhpsc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gdelwrzem.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gonycshqm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gytvyiwtf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwuuptjew.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbrokmmxm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpmnhgsj.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/ggwmlwjkt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/guowzbveg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gjtyixeuw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/ggtdzexnj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gpdrszivm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gbnpgquxg.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gmamvynur.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdscjzrik.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gzftgsgfh.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gfljieday.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gyfveeaoh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gbuxoxbdz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gqyvmzidi.sHtML


<!-- 参考信息 -->