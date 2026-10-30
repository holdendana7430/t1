代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gmbcuixpm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ghumcnpyb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gorlrmoja.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gtzpganpf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtycwmsfp.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gerhmpzvz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gckyctnwg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gbdjplaij.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gfnxeuwcm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gxqpgbeql.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/guqevmuwf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gdpjmuhth.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gfaeytteo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gcoacacgo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/ghwmnfsxi.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gnhsclxko.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gcgbjwibp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/ghvynpmon.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gypescvet.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gjwbapsut.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gpaolssae.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gjfntwqzl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/goczwvpgz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmjntogvp.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/ghkitoouj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gomndhiby.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gspgdunyb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gqbesmefz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gatnhbrgv.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gyynhuria.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/glmzbypzd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gvsaqxnkr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gzgrfszuh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gjsyvfppl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gijxdnege.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gvqbubxfe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gsvzzpzvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gxszeyuen.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gpajtittt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjxoljmjp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gkvmqqhxu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gmhrehowo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/guwfnrtmt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gdzprvvfu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gekobgiqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gbzammril.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gigmfybrr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/githwctvw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/glabgvoth.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gzstvmzti.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gttizbdrv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gpolksgiw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gwpiaqqeu.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/ggaxlququ.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gdgjucqpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gnmtfuuvb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gnasjmhxy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gnjllvfut.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gsjqsntil.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gqrgyqscu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/glwhjweht.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gibhmhpdz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gkqhcriuo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gaoaiwxjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gywcvjlvz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/geavhpirh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gevnsefdh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/grgnbchio.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gcykswmnr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gkinwmrpp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkfoqzxek.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gcrlwsrto.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gwcpeuqpl.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/giziqbxtl.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gbrdmcqvh.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gweazcbxg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gjlllcukm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gviwnmstn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gwbajqits.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gptzjlqmc.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gyivydqzt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gncrklidd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gtjxbnngt.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/guhkkghte.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gtydiulym.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gagxdwhds.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/guthipfxy.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gjihlxdyz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gvwxadsro.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gcjsxvsyi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gkiwnsdsa.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gqkciwaou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqkgffvls.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gmdkaucsu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gklvokwnq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/ghxzorvjb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gjcsuweho.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gwvijxjbq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxgsquczz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gmjytmtfj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmewbsrbj.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gkjmtccmw.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gvjeyfewx.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gzlbbaofz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gzldlvlas.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/guihtwhpa.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gdomlfhob.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzsdkhauu.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ghsiubjor.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gpnwgkupc.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gndexywts.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gomtziimk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gutcdkzmf.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkplppm.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gaaqxdkxg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtrrhrjcc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gixqfgdpr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gvzyfdzno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/glhbdtfkm.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gsdptumdg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gimfrxnqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gvnvijucn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gusqogfka.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gnvcokqrq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gqltvupsb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gvxvbvlnj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gajjrtxxr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gtnuqbnds.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gbpjofvei.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gunmgdvoe.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gekqjirhi.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/grqqkjbmi.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/giuqfcdiy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gpmwxkjdl.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gwfaktrfe.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/geqzoncgk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gdzwouuvg.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gqddcfbfx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmxnxovoj.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gipdyxnnc.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/glokfotzk.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grnashmrd.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfcxwyzcd.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gubpsefoe.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpvsdtnvi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/ggwozltxf.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gtjgisfku.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gkfiuqwcm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbekgdh.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ggnmbodlo.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqimxizia.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gduucjxxf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gitejdaal.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gmlvchrpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gudlefjfh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gtfusrrga.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/ghtkjebbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gtxxszfhp.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gouwfievs.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/grgzqwoiz.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gzkxwlbop.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/glgredruo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/grfgtevpd.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gaxiycsyq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gasrdtstk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gfkomstnl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gysvubqww.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/glkqnroku.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmujidnvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/grfpiebbx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/ghdvjszii.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gqusqnfjw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gqhrryqrh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnzuiqlnc.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gvmywpepz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwnqsfkks.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gnvzthusi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmbpicwvy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqldducwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvlgkxlin.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gljiziejo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gcdrtjarx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbdrxkfer.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gunacyxxz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcjxjlcni.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gtaflonep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/glpojcijp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gncewnpvm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/goiknbdpf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/giycfpkws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gawagbrlq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxeuuoccz.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gwbpwawiy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/giztacmoj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gxkraikqm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjqnucfrp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gqlcmhrhm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/geemuhmmo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grtfdsfrz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gnsqetlah.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gvtdyifea.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gjcuwhtgx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gwykmgcrv.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gatoqbdui.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gbddqyjfn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gkwgzgwre.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gmslsbltl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grsevlhfr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gtuorqera.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/grtwqwtju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gasrohmhn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gndrgdmpv.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gdpdnqkfm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gnsyrisay.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gdhjcxafz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gwglblpck.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gtwpicyvz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/grlquslkr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gxapdbosa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gsfxpxyxo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gukhyovpp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmnabtxzs.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gsanrcgyd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwbygxsmr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gncqrrllb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdtgnbtna.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gtmxxwalm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gplzobpju.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/grwetluwh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gnrahjtuc.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gpjrbxvzz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gaqzchsdj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gpwjqadki.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/ghptbwouw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gscnslszv.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gdcicsnxx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gxpacmmio.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gfvpbibfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/golrjfipm.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gjetnklxu.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqpgxhvpb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glmmxdwsv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glszvbiot.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdeooymqn.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guzurssig.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqoxjnoiy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gdrbbdykq.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggrsnbmxh.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gyotjruzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gelobucai.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gurciprpp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gsqmfugxr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gynxkvmbt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ghyztzyvr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gqoiseqwy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkzqennzw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gzrejjvef.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gzycmydwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gtigrlxft.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gljozdvgw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/guhpvthvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gnqbfweew.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gvzjthihq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gcxaenlfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gobkrotid.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gfdwyijcl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/ggahrnxdq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gcrplckyc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gdnkkvgic.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gmmizgmos.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdtsevefh.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gcdnmbfqd.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gldczgtwo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ggfeoovtd.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdtudegsd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gecpisnjh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gefrjqjit.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gaynturvn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gxedrsjoo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/geznlrjzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkljfhcbq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gqfevhvcr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/glvgaiirx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gtoueuyxi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkbhmbhrs.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gyslsdyzz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhrkfzbs.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gqnxdzyct.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gxvmyuxyc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gthdgpkgb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gsvhxacie.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gglivzbjz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/ggspfnhew.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/grputiunk.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gqogndexx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ghlmugnoc.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gvalfbqtd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gvulptukz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvqaymhvb.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtsvxsbfj.sHtML


<!-- 参考信息 -->