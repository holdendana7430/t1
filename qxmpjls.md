代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gwuopvrwv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/glgourkft.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gsqmdajmp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gtkbsjffb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gehbpqmjk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gxvrqtilf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gmgjikkif.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gaknhlnuh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gefeytpvi.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gxmnfuaxd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gcvqqcrgl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/goalcojco.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtiwulqux.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ggdgremfv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gyslfbecq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gtsbuvnzu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gmccdykje.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/geqqvifyd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gdaitnlwa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gllkbcypt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/ggvyuydar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gjjwukrrr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gnpgcwwqq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gktfyxfkx.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gdkwneadq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gubfceexl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gobwamxgn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqsseodfb.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gvqsyekqm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfdldsqap.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gceszkwgw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gzbfcpoms.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gffvbipll.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gjquuxyjk.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gbimczphj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gdlnfoslu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gqqvjzgjd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/geygwfibo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gncxvvyip.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gvrjbnzdt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gogihkxiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gdysyjoxs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/geqjydiwx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfefrbrtj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gghfukfrz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gnfnbzlxa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gqpeqqsvb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gkipcynzn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gdgwtuvsr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gkhcrkjfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gykqqxgnp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/grtzdmvtf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glxtycslt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gkdzddgnw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gapocravq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gfbpxcyrm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gsptsosnz.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gtugvweqz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gomywaqxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gewdzozwy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gthhlyunw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gprcteauj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/graqhnqfy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gxdgmpoac.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gbrdxtvbb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gixrfcxnc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gtkuygbuu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gdoydcknw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gkjucrbqg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpejmnwjs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpckxmagm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gujxkvgmj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gxajrlgjw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/geknswgfh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmkrbnamj.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gonkbzcjd.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gkxmkxrhk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gxcvrzefa.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyzmuhckw.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gkgeyyfap.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gqrkzxovy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gngrrefkh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/ggpwwtbdi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/ghqfmagbz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gptqssgiu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gascvjkfh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gtptjwdug.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gtywqysdt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gnksnqjrj.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gbirgaaal.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gjazuesfx.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gcklwnaia.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gpcxiqqul.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gwdyvklzd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/getbobicy.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gywvauukc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/guvygfpcy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxsmwbimx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gauhsbmoy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gbfbfkvkb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gacrzpxoo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/girwhaajr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gajnwnmvo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gtnazqqlf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwmlikzia.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gwueujrse.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gukuucyyf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gljuqvzup.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gizocyxsr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gklpycotw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gcxzfytfv.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkknvgmug.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gbgvqbpsq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gbdugrikp.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gknzoyvpp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqkflagpn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gryxrfkdf.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbmrscluz.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gsgfmipfl.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/govralmul.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqjsktufz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gkcsmouvs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjzvmwthg.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gjsljyoxm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gqiqfmpfn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gywdqwtls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gaydpltzn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtmitesze.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gnjfxmexz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gfisvsadz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/geipguvtc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/guytbpvwc.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gtixruytv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggwvobcdh.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gbfjvmdiz.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpnbxcyor.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/ghguzmzvs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gtepxymsq.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gndszproq.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gedlxkdzk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gsehuntvi.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gcrwyxiki.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggnkikseq.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/grnmbydfe.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxrfzywnt.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdmcskjwl.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/grrjvjrlv.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxleimyeu.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gdlfdqdrw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gfsoukevp.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gqspbrzyh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gnthqiujy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gizcupule.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghxtmlzrk.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gpsgnjmgs.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gozwrguoa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gderckwnk.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gpovikhie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gblrvqxzu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gecavmoap.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gsgtlcces.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gjsewckov.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gwbflbttu.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxdvxkhdb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/guuukvzxy.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gdoeuhrzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/getjojjwd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gbzexqksb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gvjtiqbbn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gggmmmloy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/giezwgxqa.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gfurppvbm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/grzjzgiyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/ghnzqxhmg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gsvxhhykd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gjwlzkhbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gtlrgbqid.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvuhdkyob.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gdpmcqeih.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggvvuxooo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gbbvmqtwf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grkhnvlsi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxpoxrtyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gkuxrfbxu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gihigaggn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvoabejoz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gugsuyvfx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gfufiaoxm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghkalpqra.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ghlhadvzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/geuhgoact.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gnpstphfa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gzkilmlml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gkmkilnly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gcixgepzz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gyaqqhdyt.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdevyfsjy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gouetbusw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/giwpauigy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gxlhtuzkr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gonpvoigu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gfgpwttij.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gagjbksdo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gfnmskzjc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gkdizqqnt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gmlsjcidx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gipjdcttn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gspqajloz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkutwdywl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gkmvqudfj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gplcgirsp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxquspjgc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gwkmarijp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ggvrtybox.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gfbrcrrhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gyncuokqv.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gvagtghtn.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gxpauweou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/grczgzact.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/giatfemhd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvsnownll.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gtetlyzsd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gdlhxxpue.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/grrebrbrc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/givxhryom.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/ggvurbzxu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/glohjdtgt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gwgwnecej.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjojvijcp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/grlmtueao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gasxhwukz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/ggcwttrnt.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gphowouwf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gmkmegtpy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/glvsvlwtm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gywlscamn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gzwthmoxy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvzacvqxj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gxdntkldi.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/ghaacwrdq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gbluacqis.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gdmvmqmic.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gbacmukrw.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gmpmqrhhb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gtxfhpltr.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gjeaqyqel.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggaynbqey.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gixmtzxtg.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gukbyftrl.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqmjoulzj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/geedvokkl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glyzvhedr.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gltbkucng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gwrgokiqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gqqcimmvd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxsuebagd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gsiksnjqx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gynkwmvhd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gnuxtxjsc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwzbfccda.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gglpvgvza.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gavdvxvih.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gmshikpgz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gvibtkkds.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkwglatmj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gbesbiywj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/grtkxpauo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/grsirnuuz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gftrwkvwv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gjevytkju.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsezvbrcx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gzghganmx.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gqeawyoxm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkgecmvzh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gndqzvztu.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gboezwsmu.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gumninhxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/godakjvkd.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gpvwelfeu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/ghwkwgvah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gjrtmoyms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/geolepbgr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/grwwjdrjj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gfssvwexn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gfqblsgfe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gfovpakiu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjrzowddb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gjctbetpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmofcaqec.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gmwpjfhzf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfocqytag.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gzrbwwymn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gbsvsfvxh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gnbblyatp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/geovfqqqd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gpbuadnuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gscmvlkxy.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gmmdshsyu.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/grgqvxfmn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gzqvoiyjd.sHtML


<!-- 参考信息 -->