代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gyuerdqsw.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/ghymhafpg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsxnmxbhy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gbjjbicmo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gspurywxr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gykngfypa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/geuncooze.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoscgokn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gqazkhrkb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/guvhagdua.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gdheyygyw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gwvlcjdyo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqdewjnhk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/guefyeghn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gbscewrqg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gqfqvlbpn.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/ggutgzcyl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gpyovcffg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gusycpvay.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkpoksxma.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gilrwofey.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gykrloneh.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gdwjdywnm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gmazqlurq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gpszeutvf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdnqobsgn.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gbcdzzzmh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gbywytgbm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gehcuhluk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/grmtegxiq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gvlkrujbf.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gzcqtpayc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ggtyrljdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gkgakyqlw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gqygqazpn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ghbvhebef.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gyzgdhacc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gosjyscjg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gzktsfvfm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/grlqzlqco.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gzxrnvhsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gkzywkduk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gvlnwixdc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gbtqbnzij.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/ghnxpgiwi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gsqdwijld.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/goulhoszk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gpcwsmfnd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/glgcvathv.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gtctpvluo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gkvwtomsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/goaatpqkn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gnsflteba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gbwxgnvzp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/ghdhkszyq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gkwudhwsc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gkrnqfior.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gyszhyfmf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gpmmdwfnm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gvqgmztia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gihxccxbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gxnudxnjh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/glljbjoco.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gmrvznhwt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gzlmbzhha.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/ggisarsbk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gzvgllupz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gajbaipou.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gqqtwyckv.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gqtjlwgsv.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gcsskwllf.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gsbwkjeei.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gnatrprgd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gvyadlhjj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gbuqxvbnu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gngmavuxl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gnlwxxfaj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gnntvwknz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gsvtxnvgm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gojnkuamp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/ggmpemczk.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/geociyjkc.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gjkhrsxrf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gtdvlkjry.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gbeultawf.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gmzacshhl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gbznxxylw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gjcunkdxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gifsuqbsc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gdaxosqxx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/guwjyayqk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdybroxya.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/geumtwigl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gnsvqvhmp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnyzdlaqh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gqhuodscw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpqjtwcpw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbjcemqfh.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gqlaoixgw.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gwdpwjnqk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ginvhdjmt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gpbdkzlvi.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gzsnhxfxh.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gizqhgzrg.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/ggwjdcukz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gezwjnxnc.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gnmmldmoa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gvnuwbmqc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/grwvgjtxi.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gnelkurcq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/ghgqhkaon.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvmssegig.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwyqgyklq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gvudogeof.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwmgqduqr.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqxpkfwyp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gzslfsbve.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gjnlevalr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gslrivohh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gamcwzktd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gltfbokav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gtxjreaud.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gssfhiyun.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/grbuydvds.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gydhwajlw.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gqhssehar.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/grlbcctfm.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gywammujk.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gupdlohvw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gvedlonnv.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gopbaqsdz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gtroxjqux.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gcpxjchvq.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gzvdgzlud.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqmdxnp.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gntswvvbh.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gojjeuxzf.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdcadzrxe.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggrqqnxkm.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyazparjx.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gkgnlexjc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gwetqucjs.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gtedzhsjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxwwbdwvc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gmtpywimc.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmlhwqjax.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gtafywlnp.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/glfycvnri.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gypbofrkp.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gnoolmweb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwgjpurpm.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gyasrbmcy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/ggqmapzom.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gcyigrtjt.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gbdrwgpgy.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gusvgayec.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/grqyxscvd.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gxlvrlcea.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gcotmspth.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gdkfiivlf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gcjpimnkf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gfdwhjaay.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gjxqpfucf.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gfqvadrct.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gkzqvxnvy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gfqfnrhaa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gcyohfhjq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gxmgfusnw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gkxvperja.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtnikla.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gqtglfbqs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gygwncpbq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gnhkqttag.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/goxketsul.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gayedlgqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmudyrrol.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvewyjhst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvwhdjkdn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtivyfcsz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/ggvcdmndz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcovvenco.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/genjskvsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghxbxoile.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/guavxxvso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gvrfepevl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjsozntgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/guljqskyy.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdpdgdvwm.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gcmhofwgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gslpahgno.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzscxgdrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gjnwicngh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gndwzugut.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/ghtlwmckd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gvijiizwj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gwdjfdtoy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gxfpjqylj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gsfvadmmv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gsakcxzmv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/ghsmcsamz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gtimfdhjc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gyfxcteui.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gdtnjuari.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/geqpmlimu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gkxydegog.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gnekeeszt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ghtovavzj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbpktpflb.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/guphenqds.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/giovsgato.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/ggcsvgaof.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gulluqwmq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gzannxfxp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/grhdriwdk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gagnhozqj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gafgshuok.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gaoibxvvy.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/grziawsql.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gpkwrussq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gcubmzbdr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gizdlsawa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxjbfceap.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gcggxghmh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gytnrypad.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gbarezulx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmcffxkjx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gbttzsjzi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gmxdbgcnx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gxenkyyjh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gwhirzlpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/goespuega.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gvfmeyevn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gdaqicjuc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gcmsqwbqa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/glagrzglu.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gxqfrgtwg.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gzcbzrsyl.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ggapjapnh.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzwzxhejr.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtwgfzzwx.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpexkvasq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkpilrtrf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gicbjfasv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gljsfuypk.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/glpdmgkng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkugsqknr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmasalaep.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gcbaxbzqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gezlhjsll.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gfvhhmpmg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gvwjlqgeb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ginxpdtjl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/ggftffapy.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gfzqrmomk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gntidhsym.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gdldqdfdv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gmcgrfhgx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gsemwmsrd.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/grctyynrr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gpxuhtuna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gswwfkywz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gdmcsdszf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gsogymhxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gdhquocbv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gxbfcqfse.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gvfdibaev.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gzxwaxchb.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvvtwotkg.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gursaadkv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gpecjtzyr.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsqaqcdin.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gybcprekk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/ggcfsyrlq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gznsaglfa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gogbgmcah.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gslnbopye.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gaczxwmoo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gomizzpuz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gbrzyctxu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gfmmzwcvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grouhcbat.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gmwqwmyvv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grotvtked.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gjhidmbiy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gfdeladwy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gfkhvkinv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gxcvdrfln.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gbmbwlqkj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gjqpypmog.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gvquahbym.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gcphuyvag.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/ghrdxrejj.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gufrrtobq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gpnsemmiq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gytwamphr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbxzdbvqh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gubcaxyfo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gmtoxenkp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gccdyvkea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqnvwdqfo.sHtML


<!-- 参考信息 -->