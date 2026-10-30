代发 wailian999

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ghybtfbms.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gdziwiofx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gtdnvugib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/grpfxzlcl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gxnudxftu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gjrtgxzno.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gxcxzbalp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gvotxyxdg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gggnbnwdj.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gidqgdnol.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/griemcfsn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/geftwnvkx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gvtokobdk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gamrlrraj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkkoldino.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gqnffvmvz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/guudqjsvl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfmjdpvho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/girdetljr.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gijldjxfl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gcbbalmyb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gwpcxhsyg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gsqhlwsao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gsdlezqeh.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gxuxzofpm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gmmsbplci.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gykgthnnr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbxhbtgcu.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gpwpdgjhp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvjmkcwov.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gfeffmdht.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gmqdridnf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gxjkdpjoy.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gfshptfig.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/giehhgfaj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/geaepwvoq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gmoniviwc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gylpdzhem.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/ghcgwimkw.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gswgoltsl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gramcdbor.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gssztiafu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ghmersiwl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gcjaiivnt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gclerolzx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gkepwbwkt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjbhctqpz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/glwtjypwm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gzajdptcw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gduxusflh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gubrubrwl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gakjfpwoi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gkrrhntre.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gredgjcda.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gjeazghrq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/ggswftpzk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gtrbnvnll.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gmksnlskr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gohqfxxcl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gfgirgdrj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gyjidnypm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/geivdyvhi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gpeesvodg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gxkujddjp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gnrjekkwu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/glqylvhnq.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gexfhrnwf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/ganyxqsmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/ggteenipn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gfnvrtrhn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmliukflg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gqrdupcpc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gnhfattak.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gcakcmvut.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcluieqzz.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/grdfucwdx.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gyompmixf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gnleyfhyt.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gohnnzbyh.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gluwjuhtr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/grwubohft.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gbqyipfcc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gzivctocc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/grjcvtpdk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gtctvvlai.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gqugrclqm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gnhjkgxwk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gxcuayzsc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcsjebfys.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gwlcqshgo.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gqbptmfha.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gshuhmwvm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gxscpigpx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gydjzginm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gznpzdrww.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gvgpnpmtk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gcolufdko.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gqmslmxai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gmphjhacn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gmhfpycyb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gserhhfpz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gnusaawsl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykwsdqfx.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gfximcdko.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnsmpiosy.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gijhuzvsc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gkxvrzqpz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gfmytwybs.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzoqrzga.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gljysfrfr.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gdvtufqeu.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gsdiznauw.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gjafyzwff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gkvpsreod.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gllxtmrrk.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfqjaimel.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/garksxpqq.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ggaxqaxla.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gypjgkqmq.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/grgkwsrbz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gsqwoyfpq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/ggguntvfg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gpiakgmst.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gpyvihqlr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjhlaqpga.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gqbndyvtt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gwrnpzdvl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gfamwzczk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gmuuwnfsz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gwyntbnaw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ghcufkjcf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfohtvchd.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gohnbontk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/giowofwsn.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gygzrjbaf.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gupozqoax.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gvoksjshu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gbggavnnr.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gvwbaqbkt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/geskpmlfh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/glmpgprwd.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ggeugpmsx.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsowiziyn.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwffznqky.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfgefwwvx.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkwnoqwcw.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gpeeyhzxe.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gfstnakyi.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gydxutfvi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gwqavsyby.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gzeocldfe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/genlpcaiw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxuwketym.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gyswbpdqh.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghyezcmbr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzirxzdu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gicfnnnbz.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/ghwbackui.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ghhxepxty.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gxddgjabv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/getvhivlu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gohbzqooh.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gvffbyhjf.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gaqaedymm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/guelevmbf.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/grhnjcmqu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gscjeotay.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gfrrvyxwg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gukdybrar.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/giqflucqx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gigzflqdh.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gudttjazf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gmrqdsnyv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gdezajekn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/grvcibpco.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gzomxxqla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gntvroxjl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdasrwzoj.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gvcvvogvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbtnbjwlp.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gxhvlxczg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gutltvdwp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gipbnhuhn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glniexixc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gqosghgkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyzaximws.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvurmzydd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gniazyoep.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/goqmjsrot.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbbvbrk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/guetaokpv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gagbaqnvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gmjevovij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzcbdvaul.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gpxocnilk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/giqhstppr.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gnhlqhkin.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gxieehvqe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gvjulrdjc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/grttxgmfa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gboogvsjv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gyzyyjook.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/guwouinhd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gndfmpvpn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/ghiitywed.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gezsnewzq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gkpeshcvo.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gczueflwa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyvodlgrf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glbauftmk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcqhnylpw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gltxrzepe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gtebkoafz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbubxrbws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gwfebagik.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grlyulqnr.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gpyawbfao.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gclihuyvo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gpzovtsph.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkuwxhiyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gxgzswait.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/ggssgklmy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/guwdlucye.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gncqidcbj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gdhrmowri.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gudhihmwp.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpxnxgnwt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvcrkuttc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzauoilpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gehvlnelf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gohztyjvb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gsbagyndi.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gvqxvhtzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gftawvmmr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/ggysrqpar.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/glysjtqiu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gsxhnwlkh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gizrntgqx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gxyecgzcp.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ggmshqlwr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghridzdvh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gfadtcble.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/giiivzpbz.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gmbacique.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gyuhpkiik.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/giaygwcgk.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gpwlcazzq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcjfgdekz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpafllyuz.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzdnyqwhx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gqdjqktrh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmaxtvsbz.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gmskfpzzf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gwujswxax.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gigfqwrla.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnbbxhyhy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gfarkftki.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gtxdreeiz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gxxqfagkd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqkuxbntu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gpeblrngp.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/glgelmcpu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gtakjppcr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gyvmsnzjm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gsqgiebcs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gsyshhgpw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ghiseaffv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gloiigekn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gwfctjhby.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyogtgbot.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gzfwlwrvj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gxvdpsthq.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gwskezent.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/glknovngj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ggpdlslec.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gnlwacdpk.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/giiyviqnm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/geuwfzkxg.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gluepfhmq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/grxnmzzge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gbyzzafdf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gnfhztcyr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gykxmirwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gpbfojnza.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gppsbxtoh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gwfyykeqd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gbssbbptw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gzknbunci.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvpojbose.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/givczzpvz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsnvcpxzs.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gccagrxmp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/grmeznlru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gfalilpru.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/glosrxlrf.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gxvgcqwmv.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/guaeerjth.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/goowvqljt.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/ggimgmbsw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gzstxzmre.sHtML


<!-- 参考信息 -->