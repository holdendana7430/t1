代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gthayosqz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gmcravxwl.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gsjibpuwi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gkjyupppd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gtwobbooq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gsedzslpv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gxbyputnd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnfphgqjb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gxwxufaes.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gvogezgly.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyhjeobew.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gclphjogd.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gtbfuoadx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gequdextj.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjvmxjipq.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfctomkny.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gbkftkkgr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gyhcmqgwy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gigqdrkid.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gwahckoua.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gyahaaqwh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ghyckfnhx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gsejdqfdn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gyuvlndcf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gbwhngadp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gdfxpmzeb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gvewrexjh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gjqeefvlt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggigqlgua.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gnnmzyeox.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/grpxoqgoz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gdbkulwsb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/geywkpmkd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjlswnqeh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gefctdcde.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gaalzbhtp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gziotjsfa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gbhlwapik.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/glhbpbntp.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gxlvwcjcb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gebvfqjgb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gedwyvqih.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gduoqrnfk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gpwqgbmus.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gacrplkpm.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gezdjraly.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gazgwwqkq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwmzbfipb.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gcujohvfz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkqykihbx.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gwhstzvzm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gfioyrcly.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gftbyymqx.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gislqhfir.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gegncykdy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gwzeitmms.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gvnqqhdyf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gyelfnofw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/grcttbmfa.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gsdizgxfp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gwmqhyncz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gdkehqtbu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/glqpgstcu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjzikqtnn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gugeeijor.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gfqmouhbq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gwuyqzzoz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gycahtiuf.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gbmofeete.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gzhlzrypc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/ggktvjbdr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gdyivdwns.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gxovmoeay.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/guqsygsdp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/ghqvgasco.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gptpywhty.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gbbukynbd.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gdtcjqvkn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gsqziuyes.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gkuwjgpyw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gjgwosfbg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gsdlomckv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gylsewuuk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gspoekmou.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gbxoqzftd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gbcszrsrj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/grxbczwxz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gmdshoilk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gvpujmrls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsfborkgy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ghjmjxqkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/giotrlcll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gbialplkw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmpakexlc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gmmgxjynp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gxsuvepap.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gpnedyloa.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gimhduijm.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gsemqqiuq.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqbzlhdkm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqixfdoho.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gznjyeokw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqdrzdt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gjbhlqdiy.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmfbadzun.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gckjqgpnn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gcjgvoxjj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ggrnrmyaa.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gpufxyeky.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gbxlxfphy.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gnpbgeemt.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gfionddqt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gbmqhrzev.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gieyegrla.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gtumklrsd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gqczukmrv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/guweofzwy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gegjemdfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/grekiyyxh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gvxizwzxj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gqoxtnfxp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbchxtact.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gljrwsypi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ghrwuxlmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grxnxxoro.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gvnkkmwfp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gvdmllkrg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gofkhrquc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnvhwmzcx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gysqzgyrr.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gyhopazqh.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gztcjlcyo.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gukvcnezj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gyrpwjlcv.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/grkkauisd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gysttgxhp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gmksglosv.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/ghkgtrbds.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/glgyhwdqm.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/glafoimxz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghpoajwcw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gfmujhpgi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxnyvxngt.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gocueyktl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gmphwpbun.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/ghrsjzheo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/ggxutpkyd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gctqyxiwg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gnlovhnsc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gnmekfsfj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gxwxkaazj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gngtaopdo.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gqmsiyvvl.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gwhgmznrg.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gphbaikex.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqnxpsfdm.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gwbdcwmps.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gdlaxfwsm.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gkoyanxgw.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/glixcffuu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gqxcubzzi.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gqjoxnpfv.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gajcvbebu.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gvitviwmh.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gioaxptbh.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzrgkpjri.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqfvkctza.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdpzpqsyy.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gtnvbtott.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/glsfcomhx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gzrhkqjpr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gnvgnqmea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gxukywfpf.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gpuydsmys.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/grljznshg.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxllouqsu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gpkqukwxd.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gnrchorbr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gyjshjeej.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gohorztav.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gflswtmka.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gswicuqwq.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ggvbynvaz.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gbzwkqhjb.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdomndnmf.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gvkzqshlu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/geghcjnfa.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/ggtkqltcm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gcoxvvcbt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gsjpepqin.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gvkndwtra.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gtasokdpw.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gdyzmgbks.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gicimwgoi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvqsyqjgd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gctujrbly.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gzjcnrbec.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfimhxvdc.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gqxhzqyzc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxpdwtoce.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gpziuaixk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvclcgxms.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnepnlvhs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gcounjcak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gpkmmnqho.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/glxihyhiw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbabximgr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gqkjdfprf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxkjuksze.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gvzbwzkpg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gkfrkozhh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/geqziayxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqckgayze.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gxpefbbbt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/glljfrxiv.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtfzfbfet.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/giccgtlwk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gpprnmgvy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gsnhqzikk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gxqdxhzkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/grxqpdpue.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/grxepvvme.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gxagpckts.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gyppfxfep.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/glhugoior.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gqallidtj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gwexfyodu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gmxbjqlhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glmpinndw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtfffbvcw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbrzdckpf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzvsnkwjp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gusntxrdj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gnrifpwqa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gdtdotycn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxoudncrt.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gzrvegcvh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxuzpawmd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gqgmsawyt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gygnzmhth.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gayckxmou.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/guvpcxwkt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gjlulgtni.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gzgiirnnp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/ghcuwbijl.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gbhyimsiy.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gvrtebvwk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkludhacd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcyzktuut.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtkljlfdz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gavsniohz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gvxockdem.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gfivucdzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gxtodyicc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gndjhfnrp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gzbgvlxpt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/grhffcsfn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gzravlrpi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gqojlqnze.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gwgwjhgxn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gvndtixgk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gzgfgnrwg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gbcgitlir.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gykbghasm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gbrsqwoqv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gjbtcohcj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gganbaiye.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjhthdpqs.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsblnbyuf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpyztfimj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gufbjppws.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsesdayih.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gbwmljogc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzsghsbog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gbhxmpkii.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gilumpmjm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gpgsifpnv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmqzxgytq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gfnjtfgpn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/guullqfbf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/glzstrhgi.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfwcjlu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gxjckmbcy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/ggqbbhxpp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gghoiiohu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gtglbikid.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gshafcoxt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gvaixxwjf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gexprjurp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gfqgydtmb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gdskqdusp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gjweecuuq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/ggfwjvpom.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghmmlnodp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gnzkqphkj.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gnfsjvbfx.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/grgpedmcx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gqwnyyhfg.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvcxaaens.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gokjvpfnc.sHtML


<!-- 参考信息 -->