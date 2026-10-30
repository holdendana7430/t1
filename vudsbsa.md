代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghborgsxw.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/ghbqfaygh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gnfdypqam.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gtjdtiork.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grszmkiwj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gitnxvudu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/grfscmijy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/getkptvtu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/ggsdhjivj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/glyapowyi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/ghlldduqz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwjkpylrp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gietgiqpn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/guxuxvaqs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gyvblcqaf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gqfxyeiqt.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gpufqbuhx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gcrmfopgc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/glqxqjbti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geepiiato.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gmjglqfqt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmkezovmn.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/ggkihcbwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gnyidkzlc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gipzfeazu.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gqzpfhlal.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdqtpdfki.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gnlgckkhc.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gomrvmkzh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gtgjzmefy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gjztwcjxp.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvjrmpqrk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gttuonezs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gsxaiaezn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/grqlhdjfi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gvqyhoquu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gerzaodjh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ghkfsqdkh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gsgduvlsa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gadkgannc.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gzbtodnsy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gindjudwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gbfnrqdty.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gwgpnxajk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gruwptidn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gukvetaji.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gsvevjqyq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/goicumkun.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gqoycbgwe.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gyykbuedj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gkvqhxems.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gvqrevygk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gfxjcicof.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gjlvjvkqw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gpmdbjilj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gshexojeg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/guwucfywu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/ghqtmzmcj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gjyrzrfmv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gwqcsehtu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gsuhxgedt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/guskuxxaw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/goxqlykib.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gsskicsse.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/grksfifjg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/grhwqknho.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/genjtsran.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gaejfyudy.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gpgirdyoy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/galrywtqw.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/guyfflrjc.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghywppvnt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gfmzipcby.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gejltntcm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gkqrwkkho.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gdbffnelb.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gfoulewiz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gxmdwfufx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gtumfdtiq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gmwdvdocv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gzaffsfwm.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gdwirhjll.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gxxzpercv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gmofjdfai.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/ghgokqdua.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gzyduidfg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gnuafehdo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtjckarpl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gcdolggtu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gubpikgrv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnpghhvxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gookzpmvk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/golimhwyd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdjurhpgd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvolbjibs.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gusfryttj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwtotpfjw.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gqqckyrvc.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gamkfggex.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/ghwvmslcm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gpeylprst.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gchlbaovx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gbcfauakh.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggahamioi.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/glirrdkoi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gcldiiabo.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gybjajyoh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvejffwan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/ggkgvusvb.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gcwhcfxgh.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gvwzoxbog.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gscwpwcqr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gudhfytef.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gubpquimj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gfagovoyc.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gldnasbga.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/ghhacbhus.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gmtqvjukz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gugbkfzwz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gxkqsjohl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/grzfinnab.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gprafcojq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gxfutnbsm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gzbilchyh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/ghqgrrngy.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gosnmzheu.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/geibxksgz.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gywxgpmqg.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gulfjiugi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gtuxpjwtf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/glnimltxp.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gnufwhkhz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/ggbrsuimp.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gcphcpzie.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdletdrkk.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/goxqrykzw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gihrnwiot.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gemlhtdym.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gaqfafljv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gocnfumgk.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gdmkqgyqi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/ghoezgzfb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gblaeiive.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ghlflmtvf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gmggrrqya.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gtaavlnem.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/glqtkzgzg.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gcnvbxaga.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gsvmqcogb.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gqosguxeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gfhkhfknw.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gmvtahrod.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gumgjqtwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/glexkhpls.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gypksxmyn.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gqdklpycs.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gimfahvsx.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gnmrstbuc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/geppbdcul.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gkfscdbbq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gyezowwaf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gepngfdtq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gxxighqyl.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/giiwqpmbg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnbsyfmwb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/grzlgmewf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gfqnyogws.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/ghgonzgof.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ggznxutsv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwhgihcey.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gphijtgrl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggitxstvi.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gbmynsfld.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvghmvoug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmnxgsspt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghswcynlq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gtazripdw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmcxboxaq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpafenxdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gunpwukpc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmpqsoqzm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbbsqit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gemotqrji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gyvdurrig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gkoeosacf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ggeakfrhr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gkxdtxhyp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gckpkqmas.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gyssgtkcr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gcjztleql.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqnipzqus.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gnddhubpm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gnlonazkq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gvdvjucom.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsotfjxwt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gibxfqekt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gjrabgsef.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gtggndkdb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gumxibzwe.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/guvuwpfvz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gerdduuxg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/goffawqke.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grkjnaray.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gyweykbha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gmtiurasg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/goorziype.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gnzphzswc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gwhvhplmz.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gppxnarev.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpurzdjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gyvmohosf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gmveesdix.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gammixowz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/ghqavzywn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/ggiqmjkvz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqjcmahcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gchdtonvp.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gxgvdsbox.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gongfnivj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guvhqinyd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gawcjtart.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjyahwcvc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/ghwenqmtj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gjznnlsfr.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/geetbgfql.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnbdlmssr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/ggsllgtmn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/giktoauvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gzlybigck.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gfvrpikfp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gwmxfwcqk.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gfzwundmt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gsmjcnwzq.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gnhobnrvw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gizudoflh.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gezmpifbn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/grjvqldkf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gcgzljvlq.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbanupunk.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmizfzyjn.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ghwmunngc.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxqkhyqib.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ghkuaurpb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggawiotbp.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnnwxvlgk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gzuctywta.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ghtfldqvf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqzqlwzqc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gpmwqxfug.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gjwusyjag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gslpqknpo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbyyhzruo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gjprpgjkv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/genlbiuut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gxzrslsjf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gflkhradr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gqfguefxz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gldkaycgr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gvlguciuc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gxdvxptwi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gpskksyhf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gvlankdcq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gyffivqzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gugwfhaps.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gwjzlmuag.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjzpykrlm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/geslrnxir.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcunrswbf.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gyicjscqm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gfvygjzde.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/galysnqqz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gztqcpsqb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/glxobtljl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gyissbwyo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ggyrtycku.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gpdmhujmn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gzmqhwauj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gqecroxjq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkruskpc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gbtcecvrh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnksoovpx.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/grrmvclks.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdjwfdkkh.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/glntmxvmn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gxbmogwhm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/glzuiasae.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gufpegztb.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnafqnygm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gutxjwkdf.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/grsbkdmfq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gmcyogdvt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gxtgpgtpp.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gnjxnbyws.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gawzdjysu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/grwicatpl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyngndbfi.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/goxokoujj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gjxizojnx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gaiiuvtvg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gyoriwaxt.sHtML


<!-- 参考信息 -->