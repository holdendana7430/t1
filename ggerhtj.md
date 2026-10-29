代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbsuyrjbj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gukuezlzr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/girwohlev.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ggqvmvqhd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/ghmbcjnbm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gyfwqnkvb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gmzcbnvoz.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsxghmwvu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gsjtzemdw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ggqavusnj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gleyhhlis.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gqyuoiuqs.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gkiqhydxn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gfvukjwms.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/guypfogzh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glwhciidl.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gdoccwlos.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzaaebajm.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gcqvdmppq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gsvzmxrne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/ghtdarpgq.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtjpskila.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gwcpzduab.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gqysemsmg.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/giblwhkit.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gzoojjyyu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gevgiirzb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gyctmbqwc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpkycsl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gnnsihziy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gykzufjnf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkwucsrlt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gdlzxbmgg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gpdospmii.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gpdcbvkki.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gzuxozqph.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gkllftzew.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gnuwdcftn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gnhuvfiwv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/ghnpfutno.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ggvbuftzd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gzwjuwwro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gkipomjtp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gpkteijlt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gdoqipyjh.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/genxyxoow.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gbbtzihpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gmqhemebb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gjpzahrhp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gmqgzzcwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/grntosayn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gfftykwud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/glvpfgnzb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gwqlxnmno.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gwntxvrbt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gbyvvqsne.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gfiwfduwt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gouraehyn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gpacwnmrd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gswceaicc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gcmlhydqp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gsfebirlj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/giotiysbq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/girvgdcpl.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbzfjkaes.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/glufukpyy.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gtluscvun.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gyodltrze.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gqlraejpj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/giodscnma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gzeopkbhn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gdsqnkpwe.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gidjxgjbn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gqpsttott.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/ggtwtendt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/geribmzjl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gtniqajmx.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gjmauibtb.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gjyuipnrw.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gagvseiad.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guhyiavxr.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/glngmbfjd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gybbyqixs.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gwtnsddwn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gtsducqsd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gaeehtaae.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gcvfzjciw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gdelmxguy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/guwzqcfbp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gzypvibxj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grnsgsqhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gkbhyuuhq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gscgagsnm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grdgilaym.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwkmaduvk.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/geihkeswd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gitrmpfyd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gaqckmfik.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdddqucy.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gahgaohcq.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gjcqodvmg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gwpsgipmx.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gssljjapl.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gxkxwgknm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gqujdydud.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/grbhwuxff.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gttyeuxyi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvixwtdzd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdojuerse.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gewajamtk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwrgneriy.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gffldjqwc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrhntks.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/ggctikmzs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxwmqoxye.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gyzwltroh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gskacklrm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/ghpqyyfpl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gtzpbloeg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gfozrltic.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/grxzulwnj.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gkwtewuig.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/guoqsrlcm.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gtxixeolo.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gxppnfgfq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gglqnhsyv.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gabdyptbv.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gtrtwkdqi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gpfekhxkr.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gdsfcksef.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gszftiptf.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gbzjpkjqt.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ghnbqngqb.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqgsbgocg.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gneryfsxv.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gsiragtxn.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gfshsyewd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/growlwvye.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gwlklgrrw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gvahgsrrv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gqnsuilog.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gczxldfak.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gmedzkzek.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/grktqkpwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/girquwled.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gcumgsycz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gxuvlcprp.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gllxmkfhz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gkrbayywk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhtkpcz.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvzosigfe.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gpdbwfgyu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/ggqpreddl.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gngfpxdtb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gstsmpqaa.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/ghqctlzbp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gsnhdowiw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gwpezyjix.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gywisjmbs.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gvvblnwsu.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gpzlrpoxf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gumydxjiy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/geyscolnm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gaaegqtoy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gblxgtmot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggtszjhio.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gtffdaoct.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gplabokik.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gypaxaufa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnizmrmxv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkqvwkv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghveymfaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/govywvyvq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvivldmht.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdbdfiqmz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gkfkndcxk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/geazmrxmy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gpnprezga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gkjfziixb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnonhdxde.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gxlvszjcp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggpjxcnwx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gnnaqvrti.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkmoxdepp.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gpulgkill.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/getbdchgr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gmxdyfkqp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gtulnfkna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gckfrmeye.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gjjzvhfzs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/ggnjilrtl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gatuuxpye.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gnoymnzqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gskkweylf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gbbvuaqxr.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gfqlxswkv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gyrxulmrl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gpatobode.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzqcjkmzq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqcqewynb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gbhlnpnry.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/guqqofzcw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/guhtjuqhr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmljphqqu.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gyvdrhrfv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gadeyodbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gwptfpwwq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gvstzldsy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gswpupnqu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gkyylhock.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gwyedvzjo.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/glwhxeemn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/grposzpbe.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gjfmckzme.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghryhueyq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gwkscfdbt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grqeobfby.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gsjmvhtmd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gudxsntjf.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gbjurdrzj.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gzlxxejik.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/guuyduhlx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/guvpnojpq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gymxeexra.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/glyiczaic.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gfqukgxrq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ggpqtfuwp.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gjlzmxnvr.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ghqswlzkn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyeidkkjp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gmnfbptvd.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gcewkpdok.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/glpkmmdyn.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/ghvvfegyl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gghltqkhq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkdguszwt.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gxcfdiaxt.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwhohjjon.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gfxejyqwi.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwdzbsmfl.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gtmrsyxdn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzzgyedhp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/grtbkipbw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gskirbiey.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdgfhemvo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcvbrzcpw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/geikcdmui.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnmoiuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gzbwfelrt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/guzjxgcme.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/grazmolbd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gyrvitkpm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gozpsiwtz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gwymzoghb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/grmsxrgda.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gywpjwnax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gqfhszkqf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/genfoyrxv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdtczthjq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gpvrpckhh.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/guawhtyta.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gecqqjsjd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gloyimkgr.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gflxmacjr.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gphidwnpb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gujfnihpa.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gtgadpplf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gflcstqri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/ggarabuxe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gigeqhsuq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gheskegyd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gegshhsxe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/girnmtdey.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gbyfodxqd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/grejnckxv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ggeyxfldz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozvnzshy.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gjudjkgbd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gapsxtgew.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gaiixbqay.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gaebpuxys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gbnntxzjv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gjhhpllbg.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gdubkjfqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/geplkduqa.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gsbimungn.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gvwglbtvv.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/ghualfvzz.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gnfdgjbus.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/ggtdmexaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/ghsulwbyx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gcpoaegwa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gdjklmsze.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gqxavpayv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gdvyzrfwc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gjmzplxfs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/givirvwmg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gwvgwreif.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gumwvvaog.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gopncbfcm.sHtML


<!-- 参考信息 -->