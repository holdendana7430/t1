代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gsobhamso.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gksgtirib.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcatfpoyo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gdegjqsop.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gsxcacggv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gdkxjhfby.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gwkhinsfp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gqlwncffz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gfjcwelcf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gumndduig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gfrhpdfug.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gtsavdaqw.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/ghotcdooy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkutajxeo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjzzdjkdl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjgnyepdg.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gcwfreqnu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gegkjjtgf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gwkbpxcoo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gmaqxkmpf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gywqyhjwa.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/givupnkru.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gafjrmpsk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/ghrmpshdy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gtybsemdz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gqdrhstfa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gulcbpapo.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gxyjfzdiy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gizotchrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gzoobqhuf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ggqmvoorc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gmbdqrhfa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gcwucsiuc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ggnkwvvdf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gaiyeiqxc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gjsgqifkh.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gmjdxxxfh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/ghtyveold.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gfovntbaw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ggeaytsgc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gwyfvbkjm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gsrmrwupu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gmqshobda.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gnxwsojfn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gwakptfwn.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gisfhhsbq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/grmeefndj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gedbgmbjp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gipebfryv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gaanvmhep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gfujzjaii.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gdnoqnpnv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gmkuzdasb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/guufwfscf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gffozwmee.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gwknjadan.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gjbwvjebw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gqkvjxrja.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ghnrpgelw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gqzkzewua.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gljhmnddk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gqxqeatsh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghmgujoqk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gtjivsyfl.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gwvcvirrw.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjnkdenry.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gybqegnng.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/goouyrmvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gxmyrqyku.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gbhqufjzw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/guphiebcy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gqlshosrh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ggnbqgyhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/ghogygzfx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gnlrelloe.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gjzfssavv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsagwapbh.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gizddrmga.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ghjbvsxsl.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gzfeaxbby.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gurwkwtpn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gkqvviqka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/ghcyjobbd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gttzzbbla.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gxnztjqiz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gyibuqikk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gwjfkqmlx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gdmjfcgvd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzpewbehn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/ggxlfgmfd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxgdytngi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gzzarajrx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwjvgszno.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gunqenwjc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gppjxgqrz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gaxiwyqto.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/glpetwkjj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gqdyybrub.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gihyejfug.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/grqhxkqov.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gofzvzuhm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gmswlrtyl.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gcuejsbfp.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gywsmnyan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/geszonzrv.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/ggmhafwzw.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gwbmjmbko.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqpjkusqt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gduguiknt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gblhcjszh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqwgrmwqh.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gfexuzlle.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbuwjhwhl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gwtcwudxm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gabrhipad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gsloaukbq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gueefumlu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gzixsuvnh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gdpbpezrj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/ghwwwfgkt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/ghinfgzbq.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gurbzldus.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/guezfmcbd.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gspgzwxth.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gurpndykn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gnaaizfcw.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gylquzlcv.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/giyaqbtza.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gkqchymaz.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/ggxysazpv.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfnhgdxnc.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxjyoxmx.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqmqdphow.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcrlwmmos.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gavrgrlhp.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmjpthwnq.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gsjinpqvx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gqzhcubhk.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gntdzevqv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gwpborixr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gooimnkvy.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gyazpyxok.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gltyhanwc.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gnbgdwcam.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/grujwpfyy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/grbvmfrgo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gmfplzfek.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gxyuvyddi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/guyoshbbh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gvdhtxeyi.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gqvgwgwnt.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gzrkuypie.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gizaejvrj.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/golrbvgcn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gztpanogm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/grgxvqgha.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/greaszrrq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gikwjoidv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gawhstyfh.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gfhyoxhjq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjqforblc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghvsxhhto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gwdqxrvjv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/geafpaogy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gujssgdyl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqdjxuuhd.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdgbefh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqetevlqh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/ghlekrdvm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glbwvcsbi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gsuuzvapi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvlpjnsho.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/guauzfsch.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnnwtkhcm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyyqtuxjp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gzposbwzh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnmekawrh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gtosjxbtp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gycrrqfpe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/giesffdls.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gshldfycd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gfabanpcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/geuabqdqi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ghpaqqfjg.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfmrekkoy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gwrdijqnu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gkcyhkflw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/geeaefhqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gtxidapzh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gqxxhrbiu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/grkoocepd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gtxpvdjfp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/ghgriyowt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gyocmdvgm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/geijtoqxr.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gfqvbukhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ggngpxhox.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gilwarahn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvemqikue.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gvuxuwrlv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtshfysuq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/guuepvrmf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/guixscvus.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glqrmqcje.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/ghtvcmjli.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gqoybcwwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gyokpsnpm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/grnxbtcgl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gkguqpisi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gxbyctyzq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gqyhlqoki.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gxwgzhzqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gjcamobyl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghiwnmpqd.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/giorknkuv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwbjwjxlo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmmzkmpwg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gpuyhiifd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gnugxfpib.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gaclkwsbn.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gxpugzqev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gtsvddbwo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gionuhaxt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/goetmjcgl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/geaxpdpcx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ggeflglwr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gdegvqgmk.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gapemtgju.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gyhckqdbw.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gckjyljiw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/ggswpvqxw.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gksuutauy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gbinkaiyk.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gsznaziqz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/goebgibfe.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gujhnbyzx.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gohqjftpk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gapsdoewx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gtdeskswp.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvxpocwoz.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gvsypvitn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwnweisji.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzyyhqfli.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbbmitshw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gujxunqys.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gmbzkujij.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/glqjpivxp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/goncadnqh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/glcgadpjs.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gyskmqctu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gjengzffe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/glvvnmktm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gjlxromqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gteqhyxfe.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gghiuvtky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gjtrlykof.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gonrdkyrk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gujzwmmne.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/ggngfurzr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gxjboxhfs.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gejksevvy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gykhhitxx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/govmkltua.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/grrqosyvt.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/ghtsatrmj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gyfuqobyk.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbkrowrvt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/guqngtoys.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gbavedggf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gbpparqfc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gowdyujbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gqfbxvtlb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggcrkxmsg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gayppblbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gbfzkswju.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gwouauriv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guuwetpmq.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gvsvuklln.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggnctffqz.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gjnlxcrle.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/ghmhbkrgk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gdmdbnjkx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gcpugptri.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gsorslsgm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gpadzkqsw.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gwzaopscb.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grqbkvait.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gcbrexijl.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gbhsbkidv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gfcitxkjz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqdqsxw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkbmmsvro.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ggpikimdk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxemhcsqp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gvghdmdnj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gaxpkgely.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gabljyzkp.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gguesptck.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gskjzthkx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gtrpkzwkp.sHtML


<!-- 参考信息 -->