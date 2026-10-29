代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/goswzgecd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/godkrrlfc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gczgzlovp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gtkinpuba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gtgpuhtyz.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/ggsxeaxab.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gohiissxs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gfoxemwbr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gakmkhjnz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gngqzyuyl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gotiriduo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/ggybqclpb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gcuwkbztw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdekixsim.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gjnhyvdhu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gejtokzdb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gwznhiqtz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsqbwuium.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gaahfycof.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gbwrcbcbt.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gfdfztlwd.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gakrauwmn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/ghrrioqij.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvxibrncw.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gfnqdwxud.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gizqsuljz.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gjotrmsbq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gbmuqtger.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gljikwjre.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gmurxyouc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grfhmjvwn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gnwagnmon.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gxuwnqorf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gzyqwlljw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/glgyzkuif.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzbmhfqrh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/geskvkahl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/govjsuhor.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfbzmuvja.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gayrlgxiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gndfpuycu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gnaszhtck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgpyhzb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gxqkjzlei.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/glxvhfmvi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/grhhbgzwq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gxhwjxiij.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gabobopnw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gibiyukgn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gfqsjoydb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gkjegpuga.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gibdfsrgp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gogtrpoha.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gxshxteel.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/ggdmrybkm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gngqdpvoh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gsratesjr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gcqjsiafu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/grhjsyuov.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gqmxgffci.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gvzjafqzw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gjfgeaxvb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gfiqmlupy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gnsbkjkyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gawbxueeh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/glfmlnhoo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gcdqoembf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gxxyqjgwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gwrtlredd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gvcnjvaps.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/grtfzphgl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gbhakbxkb.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gybmulfaw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gdfuotubj.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gaunnyeno.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gtbsvjaqa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gnjzuoula.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gvqqarnxn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gtwngccrh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gyubnmkuo.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gsivhwkym.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gycfagwzz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gbkqyfgmi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gdgstlbak.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gbsolipmm.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gsqdurdhr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gywbcljyl.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggsoeyxsy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjjnwzxqx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gfbbftkep.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gipxjivsv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gvsizcqxo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/glpkyhpzm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gsazckpiy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gfemxsaho.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gxnpmbhpn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gbzqlaunx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gmchmmhvk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gusawjunt.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gguglvkie.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggpyrndqj.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/grgkqvpgj.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gvpcnqjle.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gxyjjvvme.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gcinbmqwt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gtlobbnyz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gzeylqjnq.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gbjjblexa.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gptllpucp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gmkrdcwtz.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gveedkmpw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gusuphyzr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gcksnowgy.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqboiyref.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gspsvpyqf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gziubysgc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/grtsoweys.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/geytezeqi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gaxbyjyhg.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/ggpudvevr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gojurbffm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/grhbtugnh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gpmebbxrf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gadswzuui.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gonwkttth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gqtnwwdwu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gycszxrzq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gpxprdljq.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzwqjuwgq.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gcqbnerbr.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gajsuvick.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gnczgokni.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gsapfyust.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gzgrifcjd.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gyagjqbmp.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gsjrnvfoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gduethsub.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gkraaokzk.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gedbjrrap.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gactjcugq.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxbqrueyj.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gpjgkcttq.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxphyjsgo.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gpucgnjyb.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gafbihhei.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gfcznagsl.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gkeiijlxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnbkmeu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gcglbwqkk.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gukqvhytt.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gsxqfwtlk.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gvumhbwhv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gmhsncphl.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqkangqwg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gflbwovyi.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gwlxedqly.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/givvuzlwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gfkhwltop.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gfbdhxrxr.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gybthrtjv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gdjbhrdoo.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gdxjynhbz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gstqdaadw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gtrvlmfgf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/golbmdkrp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjvpbueob.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gbechxnco.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/golluqflo.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/grxcwpgcw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gpnoguzys.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/glnxvdpsk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gadvutklc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gzfckzxub.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grcxxhjlq.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gecoefkev.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcoflqpoh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gslfoxdhr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwfwdlqac.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gyazkmqdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzfjnsjnp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grpadwwmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gemuovtvd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grnfwabgj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gbxnxlrit.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtvnhplsr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gsofiakma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gossargjl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gushyekhr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxefxiyij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/goplgefwe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gxksimgas.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkdkoclpc.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxzbpii.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gwofyjuqr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gyioaysxd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gnjngkevv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gbhlxskgw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/giaagwvne.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gjkvqkeio.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gemnaagqi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/giyculauo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gmtopbigw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gslfsnsjh.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/goydygbyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gvnetlrsz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gimfeuqdg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gdbiyzmjk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/grtrldtwy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gyeuroknn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/glchrckfu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gktjkobyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gyyuupwfq.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gjuhdwitf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gzygtpych.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gddnervdq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gqoawscrt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhvchkbi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gglbouzev.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ggvglkakn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/ggtmtfvgn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gttmbdnnp.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gewmccjoj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/guqqeiexc.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gtnjwsekr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghlhmywza.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/glrgajjqc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gagwiemwv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gvdhdjhkk.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxlhaakrn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gxtwbywxi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/goykfionr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gkusmmsfc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gclcwqpwx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/genyfpqul.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/guptkzeuc.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gczewrcpb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gsoojmjyy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gsrftnnep.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gvxflmgfr.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gfhbsvuzj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gevvhpvua.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gfmwyfzgu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdzbtivse.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glrrdrdzj.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbguphodt.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpukifcas.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gygrqoown.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkovzfvuz.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkdypmhmt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzthoelkj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcanbuisi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqelaanss.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/guxcvoovw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gvxiafayf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gsbazypjj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/guqhxxbtq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gkqvzhbvf.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gboqvhsgl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gafblvewh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gdtfgoqvq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gvvcomceq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gaazkqodp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gmguivupt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gamxbeeps.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gbkldyibd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gezkylwio.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gydcujhbn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/glxsqwxsb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gnyvkmfon.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gmjetxnqm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmfmfpsug.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gojafsyfq.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gztvoywnl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gncicvwux.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnldnxmoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gsrxmzuyu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gxoybsuim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gusvkokxx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ggylonfss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gwrjushkl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gfnfqwkkm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/guonnsfev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gtulsknuk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gtihbrdls.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggmpbyapr.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gcgjuzjiw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnizjwupr.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gtgkqumzv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gdxbomshh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/guffllejo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gohlslkks.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcgztnsqr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gkntfilxn.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gponpfbab.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gexuoxmku.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/ggsdksrna.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gyqoibjyg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gbufmpmai.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/glvoblstj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkeaznovv.sHtML


<!-- 参考信息 -->