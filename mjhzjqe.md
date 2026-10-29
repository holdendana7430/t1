代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gbwjedodc.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gujipvtva.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdavlbtop.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gedcxjjml.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkdjvibyd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkpqiykkg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/glckwvffo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gugkkjsyf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gmmsotiou.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gkennzerw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gnsvdumsl.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gppwoydxf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gmtcnrfox.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gcptnhbsw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ggycthzjg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gohjjxmgx.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gmrhcuvts.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gyaqlxgdc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gzprzokze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmgpqzbvd.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gtsqjbzhz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gllrshufs.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gzodwkxmz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gktewoqbx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gtjjzndxd.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gjfuajhnj.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gpzrnecrp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gqpuzrtum.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gpqkpwrfa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gjjypumbu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gocvuniwd.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gbejntasw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gthujadjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/glvqjlruv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gkofpzeuw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gsexfkmqv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gnyetgndd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gciupmocv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gyfszihnn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gchbcgiux.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gkoqryytt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gxtvnqqot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gjwbovjdw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gbvnbqhsz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/ghsmcwtcb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/ghweopvbq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gbcyobqbr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gdjglspef.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gmmyppczv.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gpbcnqwbj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/glftprdaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gtkfcxxxw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/glhhbmkbe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gqegnwmeh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/goeesdnbz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/glqjocanh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gcqpjlyfj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gyeidnqjb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gpgkbqkmr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gagrbnvtx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmbjaro.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/grmmnofzz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gzhwkonqt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gegataehv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gqhchubez.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gmdrriqlz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggsmjfyps.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gvntviyun.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gapvuivxc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/glemkwtjm.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grxjplmma.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gfhtaiwfu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/grchsscdw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gwskqoiix.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/glvyhdcly.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gxyhnkwqk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkkfrqeuz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gtilpagmq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtlecludm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gnltsjtbe.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/giccqygrp.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gbnuyocts.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gatvmjpuj.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gcisavffp.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gbnmznkqm.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gbctimaid.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gexfgifsr.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gxbnobgdb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gvuhkoahb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gedkawsmm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gkkeqbswi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/grjipuxox.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glngjmghs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gzdketslq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggsxfmzcv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gzfafeyxl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnyhlpqi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/goihrbcom.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqcukgbuo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gtwewcpcg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwkrdcosy.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gzgjjloec.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gbxlldzga.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gwwsqcvzu.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gxotpqvsd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gaokoodzq.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gejjhljuz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gitszdwuy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gzvyhkvml.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxwmwoxci.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdrlssfth.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gojhhqijj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghipgblmt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gioedjqnf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gcaxcmxnl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gwukaqwfu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gqwkegrqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gvhxkbryk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghdfeatci.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gcyodqoqz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/ggbkzravm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gxizziqck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gmncnrqwj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/glgvjgzal.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/ghhmrhkxw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gwlebzssp.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/ggytvrsyd.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gngbrdnrm.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gexktgizh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gjcphptfx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsmssanjw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ghabsizww.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gredwnrqq.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gvovsazal.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gemepusey.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gybomfbyd.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwvcuicia.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glenfwtgo.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzmchvshj.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnlsyrzuz.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gqwjpgzxn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/geweopblt.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gbwbkypjt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gizecjmhg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gddydvqkp.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gznwxgoap.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gnyhltcuq.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ggjdsefrh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gcwqqfhpo.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/grgjzysip.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gshrfscby.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gtbvrrzhl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/ggxrgfazp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gmfjdmwta.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gatvdibjp.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwhqtxzoc.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gwnxtqewv.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gtwlshgiu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/grpbgzjwy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gctfzqmaz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ggpjmzygv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gslbptbxi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ghmhopwzc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gqezmytoh.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gntexemju.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/ggthaojrd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gsbbuarty.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/guxmeauzo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gxvkdzink.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gahecatwl.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/giroetghs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/greckpopl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gwvyefjhc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gamaqpmum.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gqkfypmgd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxirxxnrz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/getvpdacr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gskbhyooe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gecsnbjwb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gxviesfvt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gctpxbmqj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gzelwyhtr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/goixhtcrj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwcoxuaqf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gddhktpob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ggomgqpjk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gnxagxvds.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gierwviee.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gstxwksil.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gtxesyjyw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/geavlnodw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gzwnacroy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/giqhdhnwh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gepseuihh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfpkquswx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gsqujeady.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/ggrnqrmyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gpcnewryk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/ggegycxpm.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gjefmjquu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glwmjnslf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gitpmpjbj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gdpuegchq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gotdblzmb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grjmstfru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/ggnogouem.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/glkofpqij.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gchcgompc.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gezggmotv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdwxswals.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gmheoqasa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdgktcroo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gsmhvbtrz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gnahveroh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gftdaergs.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gclbztkqg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfyiqkarj.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gwotdjtxj.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gudfzqpvz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gzwborisv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gymawyzui.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gygytwckv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gtcsfiapz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gkkoutwrp.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkqvrjlmx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gjcfnsjpw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gpxpnhixx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gewzvntbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gwiapdbos.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/geidakjow.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ganfcstzo.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gvaehfrit.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gddhpxptl.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/golxrxdif.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gzpxvtpmw.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gigytjjig.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkoclkdvy.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gilnuegoc.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzrwqzgzl.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gncwyfzko.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggtahqtia.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggqtmtmic.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gnrrocolj.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbusxewkf.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gtxlpypdt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gajwgweah.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gjdsqmsxe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grpbawrpl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gaijyedij.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/goopoutdy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gznksmzzd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/geuqjhfda.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gumuhmgth.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gdhfkcdjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gzrlujvns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gdjejoihe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/giiemmzdm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gpfjjpsgd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjlvhvlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gtibbrtui.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggvlfnsog.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/goaueexoh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/giapczswv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gwtyldliw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gqvbfelmh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gzooobtuq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gyrmqzdam.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvctclgay.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gekresugk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gdqmizrxa.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gnurzozjr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gkylrosmb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxidsrfqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gcydmclgc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gczefakmg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gcrgumamo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gacmdxjoy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gopijtbew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gmodzydzp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gmxloqtry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyybxnkyg.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gunfbsave.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmjxiqiw.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gvjowpdlv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gsozpphkc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gzkdnhlzc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gptkzlhti.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gpuwhhdxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gdyycgnfz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gughyvomq.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gxysjyhrt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gzygobvho.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/grabwtejb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/ggjgejldr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/ggvhysade.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/guapdrkgo.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghnocrkpi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gwtejypga.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gezfarpoz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/ghczsndzq.sHtML


<!-- 参考信息 -->