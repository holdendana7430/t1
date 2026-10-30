代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gjxalmmam.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gjnejnwva.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ghuidbtlu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gvvhodutz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gwnotfwbv.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gvinfmggf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqlzebusf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gsyelexis.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gjoigunfw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gmvfipsin.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ghvcrkhbv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gflnkafmt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gsezazxgz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gdwbzyvpt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/grdzhalsk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyjchghzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gouaicnnk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/grdyytbly.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/glgfygvfk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gkquuhmrh.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gfzybmzlq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/ggpxxobgb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/glccksamu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqqgfojdl.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gfbkrwryx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gekuspxeu.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gchxflyjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gaakpoxcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gadedyqry.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gquayxfsv.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gddbyrmmn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/grlnwmzhq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gmjxfzlgs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gozefqcwj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gjtgnntdo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/giiutxqpv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gabsmbwdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gamyjhtix.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gwxygqmbt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gnelodvdl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gavauroeo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gjddtxyhv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gtbkdtsmw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/ggjbsqgft.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gaphkvfvp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gifqqoljq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gkfycrllf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gogneytcd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gzmngliwf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gqdbqcbyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gcdfjrvgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gqrlqrjpl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gxncezquy.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gtpjffpgs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/guhgzyldc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gjldxulqw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gbrcjzjsj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gmgdiuekf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gpqxedmpb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gnsbcbqgg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/ghecayfwt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gfsdsswhl.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gudvclifa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpadurygt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gynrsjaow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gfgbmmrhv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gisjrrteu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gjzvndqhe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gvlfqkurr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gmxvehvkj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gkvtstedy.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/ghvvfkanx.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gvadffqlv.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gskfhgdgx.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ggdnmmasv.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gwjrkfakm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gjiiwblpt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gfktikazy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gbnjpcnra.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gnemrdtez.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gzuiulezg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gebuddbmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gkydfnebl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gcccigewj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gnalqigqv.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/giblfngne.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gdwidpntn.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/giuvlemxf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gmjcntgna.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gpxzmalzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/guaonmbxg.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/ghpryhpxv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdjufthvw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/glgsywaph.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvxaptjwk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/grygwivrz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gpuuzrsla.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gfbmcvduf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwkxhhxzp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gbixeuxhe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnvqoosxr.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/goegoqgzy.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gjtadeocm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/geontkxdw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbwufdgtz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gjxcraxrm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gerizrrzg.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gxddkmelw.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/ghlvtgmrt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gwcqokflt.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtbpvkhzj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gxderywlk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gsotscmls.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gmspwvqnw.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/getdltwir.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdjlaaytd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gcjpzshgv.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gvsoqtuyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzktdqbga.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gpotkyyjj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gxwrghurr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/ghhycyhbn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gyvqttymq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gktrgisdf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gdocskgme.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gocfxqnik.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gxsbtjezs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gvfmoksag.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gdpctujol.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/guztjmxjl.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gugisxotd.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gysnohveb.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gspghlqhv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gkypxaqma.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpwnjscvr.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/ggmiknqqd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gqrwcfyib.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/ggacdviot.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcmfwkxub.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gymtuzhgm.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvlxqigwg.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdkpbmzap.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfjgkypem.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzzzfozzn.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gakjqmzwx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gljasrnoe.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gdbestdzf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gzxxvtozh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gaiaxldzx.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbqallcel.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gvbjxexmq.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gxleuttfs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gphaddhhh.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gxznayfbb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gfejtyjpt.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gmzlcvyix.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gfpqxwjea.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gqnhlwxjm.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gthgrtnui.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gokfqjgsi.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggzohhsqd.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gpssuapto.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/guqakvxfg.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gycconbzm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gecadawzz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gexdqohhg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/glyosexcf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gmkevyfrg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gndhddsqw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/goqoukqhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gsgoenyap.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/glqdrcprg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gvjjpwced.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghhypoxcy.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ghsjqpzzm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcvjfysud.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/grogmaciz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzxvzmpgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gkmkmqmwg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkeptsuie.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gidehomaj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmxeghbwi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmjjeodml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gqagiznnx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcaaaxsbp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gojygkrkp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gvxsjkbub.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gewcddpzg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbyqydryq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gqqfzsebv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gegpznfhy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gvazwuadg.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/goshtfeiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gaacgncrl.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gpbxqvtsg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/grnxmagbq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/ggaluhvpi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gxizmgigj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gtbyunqtv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/giojivnmo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/glgxzlzgh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gwtkoivwh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ghgnajkns.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gshcmwhvp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gnoehmsyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdfdiukil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvldxpvid.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gxkjlrdcs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gznyiittk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gqtcqxwes.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gcldhvsat.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gafqlrlrf.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gxraumkjp.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gmesxcxgs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gotzqrtsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxjzoypz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gaafilgsk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/glmdurayq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gkrskzgju.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gcoqxkjag.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gjcvtfysm.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gginzfwyw.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghvjbqsoq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grbwkvmuu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxnxxanaf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkydzoh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gulgijhvo.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/galvzsqhd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/glcedtgaq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/guslfqfss.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/grgzlmelm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gqmditgdp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gwzoaynpj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gagzegytz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gqowznftq.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gznfcznic.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gyhjcwxmi.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gctnihuuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ggqubrull.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gpfnfbajd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ghvvovidm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggnucpwzr.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcfdzbddz.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxkngxoii.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpimrqbro.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grrwtfeub.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gbmmpvhot.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/giebjplqb.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gknzecurq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gszjhexwh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/giuuhmeoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/goxjvvmbv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gktylynwt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gfhpfuxap.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gksmizsnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfbvohehh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gagxsgsir.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gkshuovqn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gqrkzlypf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gefoumttq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gfbrsdwri.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gqftvqmwu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gkoejjoec.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/grbhoaefm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gurcbfyyr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gfoqpvcln.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/ggifljbsn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gjtxmbckr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvqmdhnqg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/grnyudumj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gxkephjxv.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gliogxygb.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gwgxmhnrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/ggnzyxnic.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbrepgzad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gfkzlulch.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gdwarlwye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gaqbrfzyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/glojdsgre.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzapnncko.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gtxbrwtua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gqacrncuj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/guvavauvi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gygevncpm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtpvgazjh.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/ghtjruspv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggzkuhdzv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gtmorgoto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/glabykdpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gabjuawfz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gnsrhfvtk.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gttxxejbj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gduworpmg.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gruuwmwvb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gxwttnygk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gzadklyjd.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gmwjterux.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/geibamgwu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gsrzckcjp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gxgorlayp.sHtML


<!-- 参考信息 -->