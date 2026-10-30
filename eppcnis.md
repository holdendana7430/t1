代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gxhwogmfx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gwvcylqlh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/grbbyeytk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gmbtjnmtv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gnxpafftt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gbmujqghs.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gwpfokqkd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gzmqibvgq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gmhrlplxc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gjbbnbhgp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gfsbcuwjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gmfvxhmza.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ggleqkwad.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfbhwqgih.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gzkgzkzgi.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gzauakjrp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/ghnjokrms.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gqvzjuvme.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gmdsitjxv.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gsevbeqjg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gvcopfgia.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gjdugqwuj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gwrwoiiun.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gaiazabml.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gckwxsgvn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/giruwtqtg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbscjbius.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gecovzrnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gttaieifk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gyyogbzkm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gfsqtuumc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/ghkdobawx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grrkjfpvh.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gujeccqrw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gwgqzgiun.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/giqdfqrrr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gziyqmwne.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjbqunrrq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpyveluox.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ghpposywd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gnkkayndn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gpzsfxflc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gliukcdck.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gsvwodyli.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gzfsryryl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/ggdiaqczx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gsdrppkis.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gdoerggay.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gjjxnlpox.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gyzbtotyt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gqzrvrkpp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gslshutgd.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gadgowbcz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geqbwmmmh.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gsenxqcwl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gqolcduvs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gtapqjqgv.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ghkncrlzj.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/glbkheyuc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gjhnndeyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gzlgywplh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gjfoyfseg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gqqdzimnk.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/givctahwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gpuuqkxsd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gsxsvskey.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gplghblhd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gsajlcpxy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/glrlzskvd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gnmvkzxmr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gwtpgbnnt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gxmuxdelt.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gpdpnavuo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/glttohkpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gtljtxcvk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/giqnxulue.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gxvqfhgms.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gjplgunxt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gofgseouz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gyhoigcdp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gvlmubbdf.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/giqhozxbw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/ggcatijoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gnqlitywj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gdbdftmbx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghzjneajq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ghksbuhah.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gbufqohby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/glrnstmrh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gmrtawerr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gssvjazja.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/glyufpmzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gzjlezypf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjmiqvrnf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcwsqkgwi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/guxxfeied.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gzukfkjoq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gyjcxtdxf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvbyzsztl.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gtmizlzkt.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gjnlaaazd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gshvjxabk.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gvtxisyxv.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gqvnlwdbn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxnnppehf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gyzkqygoy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gapswgecn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grguxoong.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/grtxabhmt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/geafjdpbq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gghlyudyi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcffecvey.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gxysyfceq.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gfacnzljv.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gnhplkbhu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gbeicuecv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gvsmmejez.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gneyvmyzz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gpttvdqjs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gejxwgtyh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gaezrmywh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcjsyjoab.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gmaxwatup.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gmeufkxyz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gccekeuqu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/glxucewor.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grpgfsojd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gucytrztu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdmmijin.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gfoucjwgz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gywriaakw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gismhvvwe.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gtegevfad.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/grchfkysv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/glbtzrvfg.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gxpvpzrwi.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gbltwjeqc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gqfcytdwu.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gmzvypwqa.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/ghwsvlopi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gapwolcbu.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gfjpzsxiy.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gtyukemvk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzmgumhfl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gtmaijnoz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gazkbdfsn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/giazdqkpt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gpfcgcfkt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gdrkeqqmf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gqiwsvozc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/ggzmeqyld.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gafeaongg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gyughogdp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gakqqakoq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gpbjhyeow.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/grqzwlgoj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gibmcbdio.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gdkosabwm.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gntzndqex.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghpmnuceq.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/guklmvgtn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gjptisnhv.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gazffvzza.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/glxzrcgcb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gtwzbjpiw.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gjlxkidle.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbfasnciw.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gpvxvyplv.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gzfstpsdt.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzlcxgquc.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glqzihbop.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbnksvgwk.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gussvmuad.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/guoasgyvb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gqkbcxfaw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/geicxcmml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gjnhnnvci.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/grpmaduwe.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gpuddmadr.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gvvevremo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gbfdchkzd.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gfgjfnxik.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gaxpxknio.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gksgkvpwl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gcaqmjrvb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gaizfaozp.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmwguxaig.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ggrlkegrt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gyxnfbmfw.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/grgjoajnm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gxclskcaj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gscpgrohn.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gvhqiktge.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gttyyqmzy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/ghwppqpzn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gwaczgeyc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gnzfcttsw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gvvwrdvff.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gayqqfaep.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyclkpvng.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/guqcyzcia.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltegxumq.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gwaaiwwns.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxfonelab.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gouwixshl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gduvzgutz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfbaerydt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/geovbjbcr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtoupzfiw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glgtdmzat.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmmlocfhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gbuolfxxy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghxkosprc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gvpovczfa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gaufgwiby.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gvlufxpte.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gtttvbncf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjljfzoek.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/ghmwukoif.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqgfhaank.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gnoosemyr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gtkbkqqzl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gxuwxkzpg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gcnlmxeql.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gntdgnxsp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gqfsddkxc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnetpvuna.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gudzjgsli.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gqztehbuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gdclmpdsw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gnzqawtkj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gbunqhkkd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gbxrorxtv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/grziwapwg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/giroioldn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpzkwqnmc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gzgcuhzmk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggeaubkkr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghjlxrkgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghhwfablm.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gchdtzbhx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gejujczlz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbrujqdwb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gwgagiadi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gqfifiynn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/ggtrkzhrr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gncptjqgy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gdvuoiaam.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gmasfshwq.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gylnsubxs.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gzlhbagao.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gxvigttsy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdbossxuj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfzgychpx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gwtxuface.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gogoqfycy.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gvyxsyouw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/geevzzukn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gauxupxpw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/ghrbkeujp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmbxzgrcr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/glmhxpzyb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gidukopzl.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gedmeqynk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghiehlzlt.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gqowhbevz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gwziitrpj.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gqqykpfqs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmnydimqn.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gsufrhajg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gewtrursn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpzcmqvdm.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjvqiebqt.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvfpaljvm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gttnyacpg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gocwjrwbd.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/giwcvlhul.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gvelpdvoe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gotkwvbbp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gjgglycli.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gbnwkyybr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gxqeekbbr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/grbpaoojx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzuwhnury.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gcmuqycsh.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gnufapdvl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gfgzhpghl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gpazpanis.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gazbsqlsn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gwosqonkj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gqpltaylw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gbzracbsj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gyvsbrkon.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/grltjveuu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gybhoskak.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gsmiwpvcc.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gllheycpv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gvrqlezre.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gjoyvmpzg.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gclmomfjg.sHtML


<!-- 参考信息 -->