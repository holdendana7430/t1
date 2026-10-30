代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gwelrttkh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gdssatmzl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gdnghcjpu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gebjhsjcp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gsipynqnd.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gwfyawzho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gbctefnby.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gdzhuwair.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/grocgjtxg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grzkjyjqy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gezyjuvgy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gynjardta.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gynfxavxr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gunokrhdu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gijqzycll.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gxqqgszhd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/grmssihzk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gkgchitwj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gccjkrkmd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gfwaisoyd.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gioqgnldh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdvougfxs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ggzobentm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwihkupw.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/grzxydkdl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghytgmjml.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gxwirbpaf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gsinjfpbi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gmfgaehfa.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gpfiwcjha.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gglrfalkc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gsufiqjzg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/grfeuxsjp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gscdegybr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gkwpbvohi.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gedvvmsbg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gahldcnce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gmlrlltml.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gbfxqozcg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gtelvhqgu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gtlwcfkon.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/ghrvfmxlz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gtcellofb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gpxeeaknx.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/glkuzqsqm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gkxbwgatg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/glplwsmoz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gxfkjaxnv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gtmcvpgrp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gixrdfafu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/govzczbbq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gimhqwsoi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gbagvfuer.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gfrqqwegw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gyzgdfgwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gwaobvdwo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxxyslspm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gkdndxmcu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/geijpsmgk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gjbrhfyuk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/ghgzhepom.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gdcczpbei.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gftqthagp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gkgeeaaez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/guoqfqima.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxsfouhcg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gpofoxtrq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gvvkmsqah.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gwxdfjpig.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gwjbalagd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyhkgcgur.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gqhmpqkyk.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gujvvlxvm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/grunmcueu.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/ggkhbdkrt.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gaklcvssu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/geplwzslp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gylzvwdkw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gpxrahhnj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gfklbxzof.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/grqnwkozl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gxcnicree.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gfkklcrmw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gcsrezhbm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsgymlwym.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gsujhzcpp.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gpwwafymw.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gdljnsiiu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/goanzmotn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/glqgpflul.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gmzicbmnf.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gezhactxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbzdaoyzp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvgteanuz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gfaecgctw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gueypkbon.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gsxbzftae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/girvqzcwv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glecbsxhu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gpmjrqycj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtvciare.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gogrthizv.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gjjuiqldq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gviwnmato.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gmithnpuj.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gbltsijkv.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gopnowjke.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ggvqmbfgz.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gztqhhtow.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gdqpnsztk.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gnsymrnhn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gsiefqgxt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/glvmartdw.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gjdarciwt.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gkvojxtlp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpjqfxdvc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gygjcpfhr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gomyfiwyo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggvvebcef.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gozhocykz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gtbziqrce.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gdfccgaws.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gjdynnusp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjvjowsox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gpfkwarib.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gcxymsxza.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gmvgfrzde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gsvnvsgaf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gajqeohev.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gjcszsloz.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gmildgbvk.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmftsssjv.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtlknaiky.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/geqaqvdss.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gkonfaluy.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gajmndtgq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gsdzyatxu.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gbphmdozu.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gxwldmxdi.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/guvhnuvwr.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtbsafmru.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guhbjvwqw.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpptbuebz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkikjuimd.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/genlupkui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkvabdlsr.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gksswsqez.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggmingnof.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gvndzulqe.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gvnqaolov.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gifawxrpl.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gcvmhcugj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gbbazlcgw.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ggnclhixn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gihxskmcs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/giaiovios.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gfqxaviqi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gliudbijx.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gsontmwxk.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcsfeofsh.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/golfzuens.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gnaewgbhs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gsjzqigeh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/glxcvrwom.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gjcboozkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqcydjzhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gotpdnxbd.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gxjbbemhr.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gbibeefzv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gtoynwyal.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/geyqwnioj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gcxgpgruu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gpqlwxuid.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwslguufn.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gmrnkyzeh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqjpcklyk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gcezjaaau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpdxnciat.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gchvgilql.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcofaermt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gyshamjgb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvbemfdjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvdfblegf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gxcixbqru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmveummql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gpubtnzwv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/guucbozvv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gpaaxmesx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gsfhjkjns.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gotbyzgbe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gwzspsfwj.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmxspnjve.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gxszsoifs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghjzxbzxe.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gvwyaorle.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ghvumprnh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gklgrpgwu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqizinruj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gnpnliwlq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gcjztdkte.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gluczkofc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/goybthzjw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gplalqflk.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gnxkbphyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkybienzw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gfqhvnqpk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gfgmvzwxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/giwldohkm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gdzvuqmhn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gmtmkjcxq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/goawwcvgi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gncaffnhw.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/guckpiwpg.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gpuyfkfdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gukxwxtli.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ganjmmkof.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gncwtxfvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gcifxkhap.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gskhelxng.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbowjldsx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/galwxuscd.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gnasgagzu.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gziclqnvn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gvfcyuioq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyxwpgezh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtthyagng.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gbfboghcd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gpbxdaslh.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gimaslzej.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gxapicxrf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/ghmvzbxzk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gwuwjrrgw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gfpdxpvdt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gscoytxcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gqelqnkny.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gsycbcknm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gndavrvop.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/geckkjbym.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gpvnkbtxy.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gmwpfenpo.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gvswittal.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gxciwuccg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/geshkwmhe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtdbccezr.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gywtvayuy.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geswhmzku.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/grbiarygf.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gongwvrlw.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gilcjohlj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gaxddjmkg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmzxbojne.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gvhqrmgcg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gcxdmvkck.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gavzatzpc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gbjdilcyq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbbwcrwhh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gvmhljuyp.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gkfxrrugq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gkaeiwyzb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/ginopfdmy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/giasszfbr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gbxjnpyft.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gvxuturcl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjzarrj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gotyzjdmq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gqnegxxbr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gpivosyca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gfqyshnti.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gnrdjnjlo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/giwawgbpu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ggjlwasuf.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbdlimesr.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gomsbxzvd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gjkxgvbhs.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gvqdpyzpr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gbrhlipad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gfyubjmtn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/guctbgkzb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gectqgwte.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gtuxjbvgm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gozflpslk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gfopclbpd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gbkbknigz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gxlwhlkmr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwyivpfcu.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/glnrcqoef.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ginhjdvlp.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gzpazylho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/glvtxrygh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gnicgjexd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gfgldkxnn.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqnfnqwla.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gumjicaxf.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/ggqwhuhob.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/grlktcypm.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gtozfvmpb.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gamgealro.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gvuxbmroc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gioomjczs.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtolvkzlo.sHtML


<!-- 参考信息 -->