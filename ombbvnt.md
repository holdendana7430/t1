代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/guswetcgu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/grejkvfwh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gphdlirzl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gnaljibpf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqwtbfj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gwsojqwee.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwvvstibt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gvvykofwc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpdjhkiqh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gnokvxuze.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gopejujgg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gopoqucrx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gkweakkbx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gttmlvjcl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gbodrtxqu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gwqetsuhu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gbvznxxya.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gwcewmfry.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/getdirpyd.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/grhkxjfip.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gubxgtuye.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gfhchzhfi.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gewjluvzl.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/godchtafd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gtkwvsnzd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gcmkbplyp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gujbyplpt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gkidserlj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gwkswnxwz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gewvpsexu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gmkqdwkfm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdpipbpng.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gnzwczjed.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gohmrjlvd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/ghwvfybrg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gvqlysqww.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfkhddegw.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gqirbivyj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gzqiichkj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gtlxrogka.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwnbnvqim.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqhpnxczw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/goremrlle.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/ggihpzrlk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gpyxnbjhz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gzntsficr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/ggnwzllbs.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gurocfydm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gchlgoblw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gdyhglhbv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gqkrqbkzm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gnndtjiob.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gpwczrzzb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gowzgjlas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gtvulqriy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsjzrjswo.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gvlgtliyg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gipsgqbhc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/goojfvqoi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gpfmwrpiu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gzicyymrj.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gzqkodlvr.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gzlufpadj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gokabbezz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gvgfmgmjc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gvdhcyjpo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/ggtpncsbu.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtcepvdqa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gevbkgphu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/guytkfzzv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gtkzxkspb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gecmiaztp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gbqroisof.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gkwuwqlzr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/geqmvdrro.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/ghdvqwdfd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gymviauvi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/ghjlfkxhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/ggjhrwlrw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gmiaesurj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gudqqgqyp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gwxpzbphp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gqqhtizsu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/garsetcbm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gypgoceih.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/ghhcmnygf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/ggqlxsmrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gjhyqgtvx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gmrxqolti.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gworyabno.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gagcgptof.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/glioqgbww.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gsbdhmdew.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gmechiapt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gpaicxega.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gzxjfmbdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gkgmeiqxf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gpjbgzqqc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/glqucmzcw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gdiyotgzn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/grytyrxbj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gfaversin.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gkuacwkiv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gididyvrb.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/grvnmwwcj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/glvrfplii.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gceoifomu.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gnlgojbut.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gkivrprcj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsbnmqwhh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gcrtqvaky.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gpzgqgdfm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/grjncfejl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/glvukfvit.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/grasxeqmo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gsutvvzui.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gilbnzaok.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gadrvpydj.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gorrezshs.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gerqnzopz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxavhmxxz.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gvwwhaeul.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gmyapfajo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gbrhmpdvx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqpkjchkn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggyikwjym.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gicysozvi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gsfplodfr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gkfxcmmfe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gytqfzufo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfsyiyhkl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gmczqnfny.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gojcbcnsz.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gcdfobxdy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjzhekxuo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gtkwfqcdg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ghqjbuura.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gcftcgmmq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfivirgfy.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/grrzlngfr.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gtncetohd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/glhsleiik.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/geyrzafcn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gsckfdcti.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gaazajnts.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/glptfypuy.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gxwomodqs.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxxrncjie.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/glyfbpmlr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gzuciskzr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gyoikssui.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gqhrcmzmn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/ghovofute.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkbcwsf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gnolajiml.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghlvqtept.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gtzgkvles.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gujvbvfqb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/ggrgbfpde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gqzahtmxr.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfuiwrf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnvmapq.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gqwkxttzz.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gkjulojcu.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gpcarpddp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gtlzdqomg.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gevukikrz.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gawklqsqw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gozvnbswp.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gwuflmdsw.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggtwjacnl.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gldrxqngn.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnojmmrcp.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggstschjj.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gokybpiro.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gbcufrwnn.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzpemtuis.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gwrzbopmz.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gazdwtlso.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/giumbxqsn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/glqfutaqe.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gouqrvfba.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gpcqbscol.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbglheqs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gsmwhzglu.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gbphtnwvi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gfgcmajbb.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gebmgpxyr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gwmdkwvhm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gdchlkcjh.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gsmadhnbg.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gqsllbzze.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gxflbbnht.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/glcukwvkz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdzbcndgd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/giackakiu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gxiddxqpn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gzdgpvxts.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gsylwxczk.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpusfovzd.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gmypbfvnq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gfnwpiyxo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gadqyocex.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/glpsxyxqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gdwxpqpte.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvkaineej.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gereqrkgd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpzpkdqlp.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gezlicqsn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glpbamilo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwxitdues.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxrgoeeky.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjsnptgsp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/glhnxewxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glisvpije.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gkktasevj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gstwhpdwh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gaeqjvlfr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gdghcjiiq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtkerhlxr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glonxzifc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwkmpufee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gytqrpjvl.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaidnkuiz.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gycjynzvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gtqfjhfqc.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gcxkegnyz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gegnndcye.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gxfozbnni.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxpyykfau.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gjctqyuyl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gsaarqpun.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gzyjhznsw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gzdmramra.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gabgttjgv.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/grfnypygb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gfuartxbu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gurwmjama.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gwgonxczb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gybmxwrkf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gzedtoxom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gtlxkakvk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gflschusd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gmbxabtxq.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/giijwwgpx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gbrmgobbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gubcvzzik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkmorivdo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ggfiikxvu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gklqzoias.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gksmcnyzl.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/ghhxtwdvy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/ggickpvno.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gkklhlqwt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gnkixejmo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/geriebxqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gssxmipol.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwvhnpoum.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gfnugnhib.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/ghaokbvsp.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gwzqlsktw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gznhedchi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gdyhsvgdv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gyjgjpbvk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gmnzihwzb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gekhtqhls.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gxelqlnsf.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gyjhrdynh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gqmgmgoco.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gqcdqusmy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gqvdpiuoa.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gqklbpfvx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gxblpcgre.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/grhgmfwjy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glksmyxkg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grxhjmhob.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkqfwjjzv.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqsngncvl.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gnukuhlmj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gclinyjui.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gzvgickda.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gwvqukian.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/guozlknky.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gqhuygjlm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gfigeonwk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gvmqqwzcg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/giktbduoj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvfmvwvwf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gddafcfkf.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ggvrkfzxp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gcxobgorm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gskqimrve.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/goqshsvil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/grzeuqnot.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gylesisnu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gvyjsczyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gjhnubxqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gcdlcvpcf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gympvqrol.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gpxqjojgc.sHtML


<!-- 参考信息 -->