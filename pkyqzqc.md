代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gexzbpavb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gnxljnlzy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/ganjgoogb.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gvynazlyl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjieojqsw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gplcswqhy.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gnqyldkds.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gayaztiua.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gqkhvjlmz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gpjqnebxl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gnzqvbgfl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gfuwwgjjv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gufoobasr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gmupwhkpy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gbsynasjg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gdegftydl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gnxdpoekl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gabjyypzs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gfquoeoeh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grbezhopq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gnphyauil.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gdnuehkhn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gucsdqxgh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gviuxrnjt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvziumiff.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggzxkedve.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gjracbczi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gjutjloyj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gzchhlxah.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gowaqywas.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gqrhwkgml.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/ghksnkncl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsahvrpfr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/godwkmdat.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gnyfrkaik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gzptitupo.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gkuwaylij.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gvtmzfjkl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gmzennrtj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grajhnvef.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gsrmbgxfv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazgfueam.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gaitvbipu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/ggltyappk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gwervigpi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gdygacfbq.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/ggpucwbyh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gflripalm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpbarecyb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/glmbnlfqo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gnesqexfr.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gtrbspfxk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gvfcihfrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gavfhnkqs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gobfayugi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gwjojapku.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gjwjuopen.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gddqvnjks.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/ghsgcmure.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gajlzxuen.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gxbjivayb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gpoattxtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gubjacvss.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzgklegwr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gqsdifsen.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gvzwosxxh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/guiopfvjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gxshvsfps.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ggqjqdijb.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gqrjzbdqc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gruhifkne.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/ggkytygeb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gvopyepph.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gemqqjwwp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gudkwdktp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/guocaipto.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gqhhmzryf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gliccywqa.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gulnsnalr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gistnlgit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/ggpsgrzbv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gelxopxct.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gvvwezupc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gnegxbdtc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gvhntiqet.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gwjnrfnsi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsknhfenh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/glwvkqhiv.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gaswxsokq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gwaahpmcq.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxdbkpmif.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gpyixbiqp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gwwtmghob.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/ghwcsvzxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gqftmkddh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gmnbrdehn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gahlrwqzh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/grxctbaos.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gvrujowdu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gfhrijnel.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gdeuislea.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsfpqgr.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxejlzhhb.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gqloufoix.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/ggmzhgkkt.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/goakcltqv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gfcyxjbtu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gfffqdtpi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gejfdylns.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gsgpnnbvy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/ggbulvfnt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gqrtlouff.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/godjzuaua.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gvznbrxfs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwebdilqw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gtlcavzgg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ginwscpvt.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/giilctngy.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gppyfvmnd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gretivlmd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkdnerlxn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gsqolrlzr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gdzgtswkg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/ghkgwoqya.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gbapvnhji.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gdjiswxox.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/guwoewtwr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/grqqcevmd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gtrwjrwei.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gclszimpt.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbewxwqxi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/grcvvdrrz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gyafkfpbb.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gpzgblgem.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gatmykgzj.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gvqbmyekb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/goiwncnxi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gwxmkqosh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gzfarqvba.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gysegouwf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gmdjgktph.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gwtbvgveg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gissmhhhr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/grqiruyqt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gpwvcftgj.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gncorvacj.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/glrzqrkeg.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyoiwjpat.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gubbzjxli.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/getfktxba.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gyvwgbmuq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gdhmwbqxo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gtdxxgrsj.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/grwdakerb.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/glcmkrhxe.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gtbqmuyvg.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtznjviih.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/grwyjiypy.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyjydxcir.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/getesgeel.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gpbfzyaks.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gsswhfocw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gusebdblk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/giatglqcj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gztoxssmx.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ggjjzwbxk.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gefkiiaer.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/glsccaldb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gwpblsfdn.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gkopjstso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gclpfivla.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gbpcxvqqs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjwsqvc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gjxbcvlqh.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gsxkbbxno.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gorgtsjlj.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gxhtbdwdg.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gzlkhssui.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gqtupzatl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/guswxmxsx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gojlwfyjd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gebxkkbrd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gfkhfdaam.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gopqkudaf.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gglepchnk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gszivqlpd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gwomvmvzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gtoilxjij.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gnqkjtslp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwtpzleaa.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/glhceacxi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glsmzowpg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gnumkzhci.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggsvavugd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqivywwgt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/giduehxzr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gedjahdbs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqenlvoqn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/giriekqra.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gbfsetghx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdklpahow.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gljmxhwre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjwkinsmb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gfokfjujl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gqzujbfqg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmdqegffk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gnkqoqbyt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnuftmqlx.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gecoilyuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gxjqbluff.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gjhypdwax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gejdzrkru.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gzzemjqpz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gheopbbvp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfjoqsqhx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gauzzlcja.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gtbgzaiqh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gzsatthqx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gspebyxgc.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gusciyult.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gfwrvzaxb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gnzsbgjaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glpuzucyi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwthgriog.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmlxivbhb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gzpjcnklq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gnwydmpmv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gmpiwvkqe.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gaypsxzse.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzluwyjcw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gizlrhqzi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gxgxqxbes.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gijdnujdx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/glcanrtxb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gnmnmpidj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gvkjyzmyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gctypxqzn.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gmjvzehsx.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghlyhvfxu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/griwuvkwr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gyomfcgbv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gijsidytr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gfahrjhyz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gcfhowpwj.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gouzmhwee.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/guwsjsvrb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gvobuvxit.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gjxkoleze.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gvpmpaczg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/glzufflha.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gjtziuscu.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggodicffl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gadavpisa.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/ghbqyafbl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gfrctptgm.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gdsvsmgvf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gowztkuby.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gdjkeotqn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxyxkgafp.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guctvaijv.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/giowbkviz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyaqteoiv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gwbwpijha.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdluglbnt.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvitihbij.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gstemdjre.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gavklspsu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/goxkjqtew.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/ggcncsngo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gawrnibim.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/ghkixjfnn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/goanozpxo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gbqqihicl.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gldhvgtvr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/grpavvdea.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gcgnqjlnh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/ghjijapgw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gzygdctqz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/ggosbskdg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gzefelgxr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gdyxbvsav.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/guqyldwwc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/geyteloyl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gnjtfftyc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/grupawewj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ghapjwbga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ghfxxijcs.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/goisxqaye.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gzxsahdjl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gheguhjrm.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvghpiudt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gscvpxiar.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gskwwpoiv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gfgmyjela.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmtbyvpef.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gbvmmqmwh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gyjfmwosl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gclddilgh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gzpqqkbkb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gokqdbtro.sHtML


<!-- 参考信息 -->