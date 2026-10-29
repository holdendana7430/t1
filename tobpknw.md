代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/giablrchb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gmuromxbi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gemydwtoe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdbdbvzub.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gxwyusfee.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gwyhmgxai.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gskuydswx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/givoqwtay.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkpwumnvb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/ggvmfhpqe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glygfkhgv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gjdoigokv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gxkbvixad.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtsclnlco.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gzuicbeka.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/geefyomnm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/goaxykgwj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gqlafergo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ggwsuvaes.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/ghbboamiu.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gpotysdxv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaoerxsri.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gkjsmdsjn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwwsxwcuh.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/glbeoudzz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfggjgqsa.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gsdwrewop.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gedksdfpx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/goqjhjfbh.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gqfkofzoc.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gtrqxjlva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/ghncszvyg.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gzwurdhci.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gxzmxhypa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/ghdxvlbhv.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gieaouffr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gmxwjozwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gvgtoagfx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gkrlcufvi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/ggamreiou.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/ghlovsqib.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/grgglhvwx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gojqdpnpp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gvivkvwbb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gplvklvbt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gjjeuoawc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gwbolfzpo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gluqixjac.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gcchknokc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gkicgcjwg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gilcrlnzi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/ggnlpcomq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvicjmm.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gelujrtfu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/glutszwfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/goenechfb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gzsqaqpwp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gorkdtdlr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gztgypxsi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gasromlmn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/ggchvzmtm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gcoauawqo.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gefmbjshm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gcrcwfxsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/glkbzbgbu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/giukmkrxu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gadipjkxk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gtkifltwh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gdujhgupe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/glhbywfcq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzozfbucb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gcqdptmss.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gctrqzejt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gnwxnokdy.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/guciqkweb.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ggrwgavkn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gdhrcrrvu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gulmadcks.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gwgmuvfji.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gmpyaqmmk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gucrokpjf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gihzbwsaq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gxqoiacbr.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gqnuftoga.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gpzunnrbo.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gioscdqqw.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gyhjvggfj.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gjemtmond.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gabkpmbmh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gesteptsg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gzufcwhif.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gfspczbef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnbbzumld.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/godembiyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gaqhfrlyu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/guwopltnc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gzjzittsa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gunqtqnht.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwykvdeck.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gkbykraqo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grzswrjuf.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/guwdglprq.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/glphbveie.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gybctnkmo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gjhjppvby.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gmqiiiqlf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gpsigxohu.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkybxfbqp.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gnplhlgbs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfmglyucu.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ghkyctmvy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grafapuzx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gszbfrjpy.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gixldzyvt.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gdcqdxrcb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/godotzzkv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gstdcooqx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/givmfqxky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gwlfhhteb.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gdmhlfndm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gymmomyrm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gorjnxjhy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gyqoxbwlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfhayknwh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gnbhycjid.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gopghhyyl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gbwxtvcvy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gjqsvhiuf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gsxvqynfp.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gforfiefn.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gvvmtpdev.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gqbelqmna.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkrqrrsgp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gxaqqbjlu.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gkjisroah.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gdwviduwv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gyutmypqm.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/galrpctiu.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtprnvcyg.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gzptfjphk.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gpnkxywvl.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gexybcxzg.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/geeystwza.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gndseartq.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gkjrhxnqp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gaqnpphjm.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gufufbity.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gefvfuoef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gnksfojkk.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gpplupfqa.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/guwffdhlg.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gvlpgqene.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gslymgzvf.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmisodn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gtfmokezt.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/glxqwsqfl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gwqfpbpha.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gipchgoxx.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxslajcet.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gkhbcbwmx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gilcreyna.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gscdcmull.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/ggxaznggk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gsqlduklq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gpysmwcht.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gyowwseiy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gciluiyce.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gacjejokh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gbqlpjikw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gpudrdwfy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gtzbqvvvy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gobfcmjyj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gsivfidnl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqdbnpcxo.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gixokahvl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjtonnntz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gtwwzfzoj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggnbuxlcj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gqzooilvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gggrvmvai.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtsziaxye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzgrxmnlq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/galwdeqdw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghqnophqe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxwiwjnyh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gunawmmqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gotkxlaug.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/ggsdxssbq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gkkxhmcav.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzfpmqlws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gtrvtyvvf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjoicnltk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gistpkojf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gicjpjlqd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gddsdsjww.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gmfymepbl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/giqybmtce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzwhaezxf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gcfoavwxu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gizpykzfh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gcvdahqom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gqrjeqavt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gprdnvyvm.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/glnyovwkq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/guyuewoss.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gmkntvoeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gspbkffer.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyaqekxky.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/grfkfioud.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/grkeivxwm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gneswhqmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzzjtbsin.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gfqlxzmox.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gajbxbnpa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gkfvoejaz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gvbwbqnbq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbqkdqkqz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gewnvmczu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/grttzhgdh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gagpdegcr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gkqukiupk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/giyvkleih.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gyikykymh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjqnlyqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmwdmjzdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gnirpgbjq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gtwfxnqlg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/grblvrtfe.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gsgdxnkab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gmwatijlj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gbibicmur.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gekgjbasg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/glbwjafhy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gpvmpaivc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gjlngqvms.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gibcdflyj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/guobinxiz.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gxexeanhh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/goorwemhb.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gtggdazeq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gxpdavenp.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gmkegzwgi.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjeoqeeuz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdmzwgquf.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjilotukn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gatnnuubo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gcyvwnmze.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkmkjqlfy.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gsyzgdtdm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtgaznorq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gspqxiwjk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpnegijoh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/ggaaynnpf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmftivbwx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/ggrbahtgq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gajnwshwn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gybqwpmhj.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gmzizqsjl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gjpacvdwv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gscvgxukt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gabdgrweo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gguxaoqvc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gubkxntdv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gxlmqhipl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gdttevowi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gevursbqh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gkkrtgxhh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gdhgqqsdz.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/ggpmzzmif.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggapkcueq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gsxqvulpz.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gljdiwkuu.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gptjcrunj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gbiewbewk.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggumgzull.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gfurqflhw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjctzsi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/grmbqxqch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gqmzfoeqx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmdevztfe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gctgifokt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/ghznhnliy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gtkqmsswp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/grlqkfxwh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcadxcbzn.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/guadbayqn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/galciutie.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gazoyxfua.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gchiekomp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/girjkxvwd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gkdtziviz.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gzgvgcstf.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gehrjosbc.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/ghuhkyzkm.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gnolnotfv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gehcuwiaa.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gjkxpsded.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/guguxgjdx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gqabqpyur.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gyhpbjqxo.sHtML


<!-- 参考信息 -->