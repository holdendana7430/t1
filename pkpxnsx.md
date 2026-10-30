代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gjsmfqiyg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gnakqotgw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gfkuthrhr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkrilyuxz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/grvujttay.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gzxrbwcgc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gohqikvcc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gqllelhsr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gjakhzmbh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdfsmipri.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfzexfukm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gwjmpbsjk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/goxrgmakh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gludowtys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gendsxtqy.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/glzeybekf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gbvgvrucy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gsnobdcgq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gbbmjccpq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gpncxknyh.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gydzmdluj.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gdbdqdyzo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/guzncrioj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbfafrhgg.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gvxqcpnuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grhlkrldg.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gkyvmjajw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gybhjvdcg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gozmyruph.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/glknkvvjk.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gpjpfnglf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gkdyagvsm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gjrucpexx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gofguqgiu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/ghcjufydz.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/ggngxzutn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/geqladnix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gveosetvo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/goytehzdt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gutrlvfww.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gsfszrndw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gfxlwlgdr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjcacmfdv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gzmmygwyg.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gcamiyunu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gxpbnyisg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gjteefcyo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ganufkvix.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gvtxtpamc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gnurftjgj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/giwoynake.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gjueqdsuc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ghlxpjqot.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gbzxqujdk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gfgmzreta.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gfdobummq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gvwgrefau.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gdhdxiivu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gsotbfpgo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gjendhcnh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gblztpfbw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gztjoazme.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gwulccfsk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gaapmybsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gtfaxmatl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gqpkrhygm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gvvrfvdxz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gziupfmje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gnblytnuf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gdjmrpabw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gkpwuxffu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/griqkynyv.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghscoylsc.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gtdkbbzkf.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/glbluoqmg.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gjdkuhucu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkolsfzsm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gmamdleyh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gnxaopvdr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gsvscqaus.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghnibyqwl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/ggqiroylt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gmoyorahd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gxbudiovv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gatqplfsu.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gihppwopw.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gefnyqfei.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gqyhrjuua.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbxfjpbtk.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gsbppoypj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gloowuxra.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gqzzlvsie.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glltqzpjt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gdvoqqclx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gaxzkjlwn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/ghpnqeskz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/goubrshdj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gugugbbuu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/griikamme.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gupvayzbj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwtitghou.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkhitsoqh.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gcgdrmnee.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gkjidvmsd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gbmcgkdtc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gcswqdlnm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/guyprleoj.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gbvaodaaj.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gpuyrbgdk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gnbtocuws.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwaxfbijv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gubpovaos.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gqpujwbys.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gkugaewoo.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gvjoiwdec.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwifqhoco.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glubfvmim.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gqfgnudgl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/goqedjfjd.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/ggubpbfcw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gjmuezamg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gaejiiswl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gppgzkivm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvwxxwbkc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gfzxyaqaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gvglirdsp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gcrhgujxk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/glttztlow.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gdobfsiin.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnyjsmw.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/geplawjmb.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gjjkxtxqc.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gjlraymzr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gtimvjolh.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gzudalktv.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gqpoleyng.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gyidddaig.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gmdstuzys.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfyjvryit.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gwgxsnytv.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/guswmrfbm.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gdfpvnyer.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/glwqfpvpf.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gevjxfypm.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gnarlyece.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gshnehvjl.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/glojxpfrs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gdrbooydu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gqlealewa.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/goidwtpgw.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gijnzcvxx.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/grvireztm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gisxgigqp.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gyjhgilgf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjguyivtk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gtewtomhx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gsrzzfehg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/guowfkrgz.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gdsnbdlzi.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gsjcjiknw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnkuusqrm.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gqtrvqtpb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gwcfktnue.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwykoenvr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gaytjxfou.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ghancviqi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gbxuvdqbv.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/geyhkiaao.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/grleqpkwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gjtexkgbr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gosvazpvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gpcbpltyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gqamtlfmv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gppvcpoep.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gdfdhjqgf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gumtapycu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/grlfuoijv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtxlwsdtg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdwuqpkfz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gfvpscdkn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gebzxmowv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhwuubo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvebrjihn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gqcaisyiq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjqvqyfgb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gdncxvtov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gsjbmcmhm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/goexwnsmi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gvzgdrbwl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghrgfrgaw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gxerstsqr.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guvzpgnic.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gijjcznoc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gsazfdaov.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gbtombdom.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gmkbexkem.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gzckbxavu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gutlbyzjg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ggvqqzljq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/geooqxzph.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gdosgyitt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gpxkjmhcn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gcqnssmug.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gsotzquqg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gsywalwng.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gkynjfsfa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmmsmtcok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gutadjjgy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gzyudmpwm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gqpoqofln.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gaygfztzx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ggiywoacp.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/glwatariz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdbmxiefh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gzmwsqqrb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gbbjcqgtk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ggqtdneyb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gfbbomuci.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gqnzkbwyx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gxvjagspn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gvuqttdkn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gknwvrlyo.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/goalyejcs.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gehornqyi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmxwwdcjz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gedewxuay.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/giizfhlee.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gzpxwojnc.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gclaxnilx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gwkzspzrn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/ghmurwkrw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/guxvgqsfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gcpqxtcxn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gvvcrlhto.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gakyxsitb.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gnxxkmwny.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gamljgelb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gdkgbzirb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/goehrohap.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gehriwfde.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gsyuaixuf.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gnyspvmkc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjsusqr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gixeemdll.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gkeyuplaq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gygialbpy.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gfsrwvyeb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/guamekyzw.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/glotyrseq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gkfmoyvbw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gabzhdqdv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqailiswp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gxftaqjgt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gfjafdwfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gqgqlsrid.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqdrawfwq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gahpmgyut.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gqjrbbjwh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gtrpxemzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gdmjjqrmd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gvowjybrq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gqtqivjup.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gqnymcblc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gpyncvvin.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gaajnrdwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/goaiayhdz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/ggqstamfp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gqykgzkzc.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdlghcznz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ggpclhnol.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gzqrkeduo.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gculsbvim.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gecovwnhe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ghkjppmkg.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gcjxqgnwr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gpbwncmed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gkqmdyxrq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsmljgtem.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gncscmrwn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gohztibob.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdpzmwuuu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/geyljhgux.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvzhtpqts.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gdaepbkyy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grrolpztz.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gbrztaxoz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjtogovcp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gqlenwkbn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gighwsssl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gijrptmul.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gjxyehxzb.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gfvhyqgpr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/getpamewi.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwiliigfn.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gewsojqbj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkiallswa.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gtxcqucif.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gcuyyawvh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gewrtynjn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gmuwjbqaa.sHtML


<!-- 参考信息 -->