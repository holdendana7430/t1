代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gotwwumba.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gcjaduqeo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gcnzqqzgp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/ginztxlat.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gbwznrdxi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gqhtayazm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/grtelqiac.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/giycxwqpt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gdagkpzbo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gatyysqwp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gllldfpww.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gbjzbrhxs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gmoemfpdr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwgqngzxq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/ghvcrfapb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkloygcsl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gburdyzke.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/godctkufz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/ghpsfoscm.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gmonjczjt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkbnrcikb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gmathrwkd.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gounpygoo.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gpkrxtntt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gdxthzlkl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gtkkluiev.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gzicpsrhq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gqkjhnmru.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/glarqalov.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gkifsuzfa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/grjmnhcpz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gqqfgqqfj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/ggpotjhzj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ghwwajxdd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwgxkajtk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gnaocfffd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gbvxangbe.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gujeyvfku.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grmrsjivv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gdjavpldd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gegqxvpxv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gakgywpvu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnwojyuuy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/geozmdnea.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gpfkwbnfa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gjymjfjlo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gfwjfoddk.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gjqztdhse.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gybqqcntu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gbbnmqmge.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/grtbivwuw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/giakqcyft.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gfonmkixn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/giadbtlhd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gpbnmpxdy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gomqnorsc.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gytggeyir.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwqrlhrmo.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gqdnbuhft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gzoiqittd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gydmrhzgc.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gxbanayna.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gijqhzafm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gpheiqihj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gqmftrrci.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gvihjsltj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gwfocrybm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gdpdvkcko.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gngnkskes.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gpfesqbfa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gwitoisig.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/geftolojc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gvpoqmxec.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gwapvzbun.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gwibybmaf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gquzlalpj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gtyfwxvrb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gnoykrmjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/guxvgolrd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gcapfyhkp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/glxatfpuc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gpoopzfca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gbxxgafvf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gsktxigzu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gvwkqwyjb.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/grgnkaxzf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gxumnwnfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gqqdxlvjc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gccivucfx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gmefqdeum.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gnjhdnbgy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gglvqqjfn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gkgzlpcto.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gufhbxunc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/ghrwfeqhn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gxnacpcar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/grydbotgd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gsywlqyer.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gsftafpmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/glxyykskp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gwwkedzod.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/giaoaejbc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/glmeeeugo.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/ggcurtaqv.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gyrbynohx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gcknkntuz.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gqtgbtgic.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfydrmfrz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gswlwtcbh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/guziufdov.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gzpmexffg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/glugtitnj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gmejtsuns.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gtjxsjuqc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gzpeovyjh.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gsgolwund.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgbyqks.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gppizvqzk.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gorghxyrb.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gqwcqxpxf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gfmakrrif.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gymxgdgqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gvhiklpag.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gogsjaenh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gknjctawd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxkectlct.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gonzrgtpp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gfwrkihel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gpauoynyg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwenyhmjc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdbttykz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gmunrcief.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzeocsuvg.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gxenwddxi.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ghebhvenh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gbuhxobir.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gejoigvtt.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gttrmmyiu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gpsiycrdk.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/geqmfisuv.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gtyyejuwp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmjaxnwsv.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfeajhhal.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gafoxikkk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gcbbldgfn.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gbuqgdcuu.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gtjxdoqvs.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gtzpeotbd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gskjjpidh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gudupjlqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhzenkx.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gznhfhztd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gkkbpqgrx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gcpdkcbkg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ghhbgjazt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gqixrirht.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gzuzdpcyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gzraxeffb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gfsxxuelv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gwekfaxvv.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/getazzolh.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gughietvx.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/giizctugv.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gmzwxbbwl.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/guxkwmmhw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gyeobhjfm.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/giupoheur.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gmxkjsvmc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gvmonrgzi.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gpdmvrupv.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjftgdoid.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/ggqzhtuiw.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpkhvrjad.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnbqeoejf.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxizqdlkf.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gpenxtnoj.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gsnaxuous.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gplskxkfm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gtezvmpel.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/genoawqay.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gzcpcgoif.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gebjhxluf.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghlnxdlwl.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gyhvlmswm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/giqmenuqj.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gwmuomhbr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnrylsqia.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/galtvmorv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/giwuwexyh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gsylfvuob.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gtsfghuno.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghdjpkjse.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwpknklbr.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gyxupwpsc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/ggtmjmqsh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gfatnhnlt.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gvcacbihv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gqeodxqnm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/grrrxyxmm.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gfqrobwjx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ggdttcxrd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gtrrrhajc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/glejhdymn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gcwgrbiml.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gwcmojira.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghslecoxs.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gvfzcsyng.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzqqptqmr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gtpvicfvs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkbtyfgll.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gjnnerxcf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpkgceqxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggwxkhyju.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/goewbptwd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gryqfitaw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/godzrkzav.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkgpztqrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gbkorklkc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gedxskzbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gktbfezci.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyelsscud.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gcrixsakl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gdeekmdjx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gewmlhqgk.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gacplnupj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gpdmbbjlt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gtdjsbfis.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gwyeldoij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gcwjhvpfe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gtmyukwgv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gkbmlrhaf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gdakpxjhp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gqheffawx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gyilddmhm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gcjqigsbx.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gqdlicnmw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsbmyujnb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gigcppakl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghnroqpwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbsfjgsyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gzmmbwsoj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gyccmoyro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gkiemwczc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbumsvzql.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/guwruyqqf.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gldeotohi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gqgzwajtx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gxaltbeaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/glodzmcgp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gksnvaebg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gkzxoaytt.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gtzaomtqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gppcfsjzq.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gvujlnupa.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gewnxdgpd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjzmokrrt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gihbbpwwu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdpkdzyar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/grqeuigeo.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/glyymcyet.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gnbmbqgpx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/giwipolbo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/grzhwagzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gyfxebdsl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gazgqmvcw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/geqplgple.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghyuvedhl.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gpqnqzoab.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/giznkbhnj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gnecgkxvo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gkqcjaaux.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gdpcwzfdq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnuzbtxxi.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gbmnimgiz.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwtlacfnl.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvuycivmi.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gshajuxsd.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyrswronm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gqqakogtq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwtgvnjbx.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/glpplgoaf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gjizdnxri.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/guueiouqf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gmwxfyxoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gbwmrouui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gnnmzpsdy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/guwowaond.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gjlgcnvsp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtpazvkfz.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gbvazzgpy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gwhbonsgj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gxdzmuybq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gppkrryyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gvmrcrzsn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gxyjogrlm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gsjhlhikb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gttabsctw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gtaftcvkx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gwurqdhyw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gpgfkyvlu.sHtML


<!-- 参考信息 -->