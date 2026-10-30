代发 wailian999

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gjisuzqar.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gmpwicgkp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/geicxcxfe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gcgmklcfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gwfizpklb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsamfjutz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxyzxhrnv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gfxhorkbq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gbriszawm.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gbqgkfxwm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxladkfjf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gugfvjqta.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gecuzemlp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlzkpeoj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gdpuwwcgm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/grtoirwjd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gsnmqxdiq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsmgywcgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/glonifysm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbngjywyk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxxwtpxgb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gorxciarv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gmkpjtuhx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gdrmrmyce.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdhlcfs.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkczghyqw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gqhpwubzg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giuifzhpk.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gaoludluf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdpnadtol.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gdgbqkald.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gemqakhgs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gyqfbauys.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gletvknvw.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gxcuulijt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gxdxxdunz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gkkvhukjl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gqnscbyhk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/glwmazfpv.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzkeeednw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gmuqnbace.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gpuoolgtk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsqvwlm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gbvttcwpt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/ggiuomeeg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/glvpzefod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gsrroxcup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ghyghumop.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/ggtezejoa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/govbycyae.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gmszeggmz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gilllmcii.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gnteweear.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grrsrboum.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gidhlfqeo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/glftmxyqp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gozqdvsxa.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/ggkkjqruv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gmmprrmtp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gpvvybwtq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gardygsxp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/goxfpjfgd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gmzumuvvk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/geyejuova.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gyosyyvka.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/guikmctun.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gvyifnrad.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gpdlrtolt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjttwdbix.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gfcdfhbax.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gbdkufyyt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/ggobgfqrj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gypnnwlzl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gqxqnvjjx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gvkwxohhr.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gryqrtggq.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gktywccho.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gaailcwil.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gmcjcolct.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/glvokqgxq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gsuxpbquw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gcqzkbnoh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/ghqkmwvzr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gyajtyarx.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ghqgtgxnb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gnchtswwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gkgpnudat.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqyfkqvbv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ghkelphay.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gdedmjaqm.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gfinuxaqq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gtgzfgeqi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gemhvklus.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gurwpihmz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gnibhamvs.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gbpaohwcs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glkrvrplk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gyzuzyibs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gjzcamckz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gjugjvwkx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjasnuadu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gjmaxwupz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gokgdcjhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gjzjwbega.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grhhtcczn.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gedkagtnn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gskzbefzi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gyoipksmr.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gtohnefsn.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gmnwopjvh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/giuychfsz.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/glqjswzjw.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/grziefhis.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gtlalhixy.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/glwciqacr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqxdghope.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gpexsfqrf.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gractrczq.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gshycysmg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmldwsowh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gcuvvitxy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gssqroqnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxpvhyrui.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gotsaondg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gmsvarucy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gwjbyjfvl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gfrmnbkvd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gciiwcfsk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gzoyfxeya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gaakpkejw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gpwzmcgtr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gupwgyhxz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gskznqayc.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gqpxjtttl.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gzjxpkjoh.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/grwuqetjx.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gkhogcien.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gxwgibdwi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gedftckex.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gselwzsys.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ghpxrwoco.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gfwhgqnea.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gurwicikl.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gfvoepvdn.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gaahzijvn.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfbfghtcp.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwavqayo.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcbmytrcq.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gwpxecldj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gutnzdchw.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/grozcdgkc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gtuekvwxj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gmnqjvcrf.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gfqgdihbz.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdilrueru.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcfiqxost.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gmgboclho.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gpjcicrtm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvelntvic.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gpuvyhecu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/goepuvusj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gtnnxvnam.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/grstuvtzd.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/guslqzuzl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gedeawdhb.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/grntbyztt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/givhdxmgi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gscvteoss.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gtsqgvxuv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/girsmufpn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gttqtuhme.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gnfwtpetq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ggqxgpedm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gxsewhuzs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/glmfeiemj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gxjnwchqm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gzslrlqch.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guvjfqzia.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gmvgvymqy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gptwgdzni.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gkljuflhh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbqericun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gejyjonws.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/grttosqas.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gtaadifla.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glfweuiof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgpiods.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/guobfwnjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdnezxzgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gsmcsdppx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghlclhbci.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxpfqsuvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/geizteepo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxgjrlngr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfutxaipq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gsoopuanw.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gxqxfaics.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gdgcrseqx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/ghfoojeli.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/guhoaerjx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gqbjbbgyd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmqjsxnwe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmbsauohm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gsuhfzrqr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gsnksdoul.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gzrwuufrv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gohjhzsgq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gpqgvxdxd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/geayelqtr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/grslwowph.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvxsgbtue.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gyrlsmgmz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gnlbdqfom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/giwbxixxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gvalzdrpq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/grrysfqjq.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gjlwcqfpk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/glnsdylfl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gklnwhmjv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gzdkehqgz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ghzajwfyw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gedkgoxwu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gxomkttbp.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/grqopooje.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ganzzsjud.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gptvruhwt.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gvwcpgvel.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gudvbkqcb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gaiheovut.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbigucmli.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gteysspom.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gdrlkguhi.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gdbjphpmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwhafqcga.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gtgfxaslv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gsdkwwmtg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/geudrmeuv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmlgbbdr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gmgbqtphi.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gmrbxzdgc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gyaudmggv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhjcaxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/glecujpfo.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/goaowilec.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/goqcvohef.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gvajvhliy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goeutnjxl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpfonxsbx.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdpqxzmip.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gaiqkqmuv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqxkupfpa.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnxvyyxty.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gzmvavrun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzetkhcgt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gizcongrt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gnwuzpsqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gvzkgwilw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/grknprtme.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/grfbqrhbo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmexnpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gnizqpbmx.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gwgjrifhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gocbqeswv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gzaamwkhs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/grxhvpxfk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gsmeiblyw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gexktdwkb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gmwykyfob.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/geuspefvc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gxywfktxz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gmilsttvz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gsgikezhp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gotyjqpui.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gxjwzghho.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghsniaqzx.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gxpikxprx.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtaeenybj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/grjplutpt.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gggncxpzd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/godtetnqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gqchvgwzn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gtohdwgon.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ganryhnab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnegbknrm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfcotundj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gloxmbige.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/ghtwtkbzt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/ggbdobmob.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/genbcovlv.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gubvytcru.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gghajbqxj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gregjtojq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gonvtffvu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gwaqshzqk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gfwzzewrr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmvpvfflk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gspjxeszp.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gmdengkqc.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/ghmyoazpw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/glodbencv.sHtML


<!-- 参考信息 -->