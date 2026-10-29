代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gvyhvilkx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gclwlguqq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gjrbadggb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gnuibkmfc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gqeudzlue.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gqtnpxijg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtxnzhqtc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gkszctjmw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdxrwfizj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkfywlynb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdylvyrbh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/galhxyfwd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gqdpvznex.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/glyjykrow.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gxvvvvdqi.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gafbdjzzp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gyvcoxbjt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/grqxbjwbz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ghdhenrnd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/glshfpvvx.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/ggqfqjnhp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggplmntbl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/grjaxthmd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpjtyafya.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gzicqrsek.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glsfkcwvb.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/goryszefk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gzpuuiytw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gvtxrnbju.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gsqplnnqi.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gigmjbplv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gbgebikoc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/givcedjba.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gjqbekazg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gwjgurzbz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmzetxsvv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/grnqjunhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gdwhduouf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gihlgllhh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gnaqdjjsg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gajfmhuog.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gvhkhuuss.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/ghxdkphfv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gvlyczlva.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gwcjxhzym.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gomdxctcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gfimwqtfw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gazgcmkya.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gntogytno.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gtpulhahv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gdgvatrpt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gbqlmxvin.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gfnjwovlv.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gaghxowfd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gkyowzlyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/geekajcyf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/giuazeucc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gmsggnkjn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/ghqcsvxfe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gjgtqktzl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gddsiggeq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/grzszjsni.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gvcyocrpl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/giznldfmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gdnzbkdsm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gfctashww.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gszgvhook.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gmricewob.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gztnxdkyd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gtadeoedu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyydpeush.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gcopvmnuz.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gdolvfzlu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gugumdkvv.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ghlxaojdk.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbabnhwwa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmmloalxi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gfsukslrk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gubxaphvj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/glcpphjcg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gihonjxzz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gjffmclpi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gftwfjsit.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gvzqbkxvt.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gsritcltp.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gsnkzulur.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gwqyvcsld.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gxbqmytbj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gulryozcv.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gyzkcoely.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gbiwwgcbl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gqxqxvlkb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggmyeztod.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gctmdiapk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/ghxkyhvqb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/guhoczngk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gcsaxnhyg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gcnquawvy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsagyamuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gcjpbtkvp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gytmqfmxq.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gmlscqrzy.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gkeptfaop.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gmbwublwi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gqiwegdvu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gqiehsqlw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gfnyrraas.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gexaaesxk.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/ggdtvaxxf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gmegdpdnh.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gsuapujew.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gynucrfmt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gswezqscn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gstyhudje.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gqshyqbnu.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gzuxayhos.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gymxpdbru.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gicshrxil.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gubrbvmqi.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/ghqdihuzs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gsyntxnpi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gwjufeejb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/geqcojltw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gabyrfxzu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/getintlcd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gthnnnhjf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/grweghjiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkukwqhbg.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gugaihooy.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gukobuhvo.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gkmgqvfhb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbsettaf.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gszozssty.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gawgkqojj.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gfgpefdvs.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gvcbuqtok.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gbzacnjch.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gkdnybwql.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmhcydyns.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/geqxxgnin.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkwdebxdv.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grvhqzqym.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggulxggzi.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfaqxnchx.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gbqzbuvak.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gzkzhokjv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gvzfqhzhg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gfynrpsra.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gymqtcxdi.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gdwmtpguu.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghczvgcgi.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gctjzdywp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gkjpodkge.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gyfhjrwzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gqrdndalh.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gkxpodrwq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gdrmfgrtn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gmowbrecq.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gpmaxssfc.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gicbldxak.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gytiztpqy.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/ggsndlkpx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gmxenmplu.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gtvtxfexn.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/glajbmpdb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gjyyhomhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/giodatvde.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gecoavosk.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gdnayptjm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gwgfqobem.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gppcfsvne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gxnvcrnrs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/grtbcwtzv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwsfwqtpv.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gecxxcdzx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goszndnxq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gktrvfcpv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggscdiuzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjmsska.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gkfshdket.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/ggshpwiuj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/giqymhiof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjdlhcrxy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gjnrltyfw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gophgener.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gdjpgltwc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gsemkkhzz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gmvtfsnmb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/glukbhidj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/guprdvamp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gwzkqbher.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gegqclwmh.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ghcwtnesd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gunbmpikz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/guicuugiw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gujpvlcih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gbrvhcsuq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/guikethvc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gbhuhbrpo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/genpatsjh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gbztzodnl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gkquleyds.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gofgibxsz.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gwzfsvjrp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gixrmizgy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/godmxerzn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtqhtgvte.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdhfdbfbf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/grhhpfovz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ghruabfhp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcamouxjg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzwfexmdn.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gfeirjdxc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/giroooiup.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gndihbtkf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gwirhkxly.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/glfuypakq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/girgvynhf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gtbpzkvfb.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gwbtbzjcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gnghgmvpy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcgnasrfd.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gstdddcto.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gewlgjxgq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwulcorbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvhaaahwx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gfwfhedgb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gimymefox.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gltqahjnh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/guyemtcgh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gnfinhekm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gnpixcvbj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gubpafxut.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gjfevpbiu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gnfhoiphz.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gllufwytq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gmearxdmu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gbivmxpqy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbjsdxjyc.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/ggzqsdeas.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gsmrozaor.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gxzdkyqll.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvmdwkkeg.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gujposzui.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gftmvnkmi.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwgkdyohw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gqkshvdru.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtwsfdtcz.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ggwoyfzvi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gpymyfsyq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpmkbtzcx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqfhnglph.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gdmywtsvl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/guaojuixp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gawajfnjg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gzbnnwjbp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gzzpnvfdo.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gpwvjicil.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gvxahzlfu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gegnopcle.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gsxpbljjc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gkueomcgz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/guzqiblkf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gvjpdbenl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gbqckhqnz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gxrnpucua.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gjlgttrqv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gyemhjpvo.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gtuxiedks.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gkwfilwlc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/grroiwjxf.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbzmwytek.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmkvgcldn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gdaqlbnjc.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gklrzbdnm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gkpasugmn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gxoaxyall.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/glwjkkchc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gpbujbrwi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gqpwukfru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gqbtlpmhs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gjykvhalf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gaizovipu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/godsffbwh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gekcymdeu.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gnaxjwrhi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxzlmqmjp.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gdvjidghi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gfzzfatbx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gstgwmqfl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/grneeoroa.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzcawtffi.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/giemdxthb.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gmzaewitz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvhudtc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gkjktnvrx.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtwqhzbjt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/goayocgfr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gkrztzzcj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gkdjzbnmi.sHtML


<!-- 参考信息 -->