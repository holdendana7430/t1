代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gwjznaxux.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gstdopodx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gqyshtaqk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gyawqeoha.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyaafffze.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gxdzgzzog.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/golpbbzrc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gxcycxnun.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gosqrmsmj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gevhnilvb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gqhwhjvqb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ggexjjkne.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkcvlxa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gtuvfkqfo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gwrvqhkeg.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gmypenteu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gbcpocvke.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gchvcmxtg.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gknxshgyt.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gycagtjhc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gsksqodyf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gvvlcagvo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gkotrotes.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gdzerbyao.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gylitodil.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gzqzzfogs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gvobeljmq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gulbysrti.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/ghnvzoywz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gpnidosed.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gzqdchizd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gtrqtrakv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwpkzrkzt.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gqaptnhlw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gavcjvord.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gtukloycg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/glmjgeier.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gjyvcxekq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpwhcegmx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gurxomogc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gpueodmud.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxgkmgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gcabjaxdt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gvjdrkbgu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gljwuhprb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/ghtzoeeqc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/glrfszvue.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gtfjwlape.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gqyzqjquh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gukawdmfz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/giezzddxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gijjrqffq.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gtxppwnvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gajecnpyx.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/ghngzyexr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gqqtcxual.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gaidxnpwp.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ggwexwqvz.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gofyiqrto.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gysibwasw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gsaymxljp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gqabkguqv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gyzpyprhw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gshabzypy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gfuluvwqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gkuqejewv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gvnviljwy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ghwyubsxg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gvestljli.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/glqvabilv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/goxwtklwm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/grxgnqkpp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gpmmtmmxs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gtxfgsbod.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/ghrgphptb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gagfpfnoj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/ghfqbctck.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gmczgywsv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/giqeljqpl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/glgdywutr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/goicvhyln.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gjsteomrx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gvjoielja.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/genfljdbb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gpctaiizn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gdesospgq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gdhuzujsr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gmtqqdfko.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gcvcoanpv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gijvzokqv.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gfhcirlqp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gyycpfjhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gfycgsvkp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/guejbrigt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyiivjgjo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/ggsvaegqa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gbmuqdjoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/guzxkkscl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grnncxlqw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gdudikcmh.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gntctfjtv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gntjiuevu.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gcvrcfpvb.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gftviuxkl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyenslv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gzgufeqad.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/glgjbtwgk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gucxbjjoy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmevwjjdh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gahsrtvxn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gtzrhhdlq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gytoccige.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gpiuupzvm.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/giqpxtaui.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gxqhxkzny.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggdbeorvs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gjnfyfrhe.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gxorveuzp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gtdrrijjv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gxspbdwtz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gxaitluth.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gczhfmgbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gqjicgzdv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gtkofbvji.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gqcwcfrdw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghtsmmwai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzojusnwl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gkyxookhn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfwhmwqll.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gfwwfzjti.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gwjhiysfb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gwrgggzkd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/grtuybrzc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gznlnfexi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gvcnnkhdf.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/ggzldeabt.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gmhloyvod.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/grjajnixk.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gnbavbohs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gffwoflyk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gbxaovliu.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnsjgbkqh.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ggwwcryhm.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvjsmpxhl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfppxbvdm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gxdgtljmn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gjoqrzshu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gxqmesmuu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gjsldugyk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gmlicmbgx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ghbabpoys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gltdnlbew.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/ggtzgared.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/grkbpibjp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gptbagehj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gmhaytbst.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gjaoptjuq.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gmuukcphq.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ghisujbpm.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxfgdrntq.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/grqqiljjg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gdqhxgzlh.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gzywlejtx.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gjgrimhqn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gtvkpyheh.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gtgcdndvw.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gecjydiuh.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gxurcefxw.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcufqbsjm.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpmkqjhbb.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gipahwlcf.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnmpxoiha.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/ghwbyjilt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gcycgwqqb.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gsbnbfyrf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gzfiyxmsu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/geqgqnwvz.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdcoyokeg.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdlqepfvx.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gkbafcrud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gdeugkhvg.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gzimdyzju.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkmckiyxe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gnigzfzfy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gnkrwcrcu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gqubpquup.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gcsmirwfj.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gzbydslbj.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gefwlcely.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gkobdnuqi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ghqoncnvq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gxfrbwhpn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/grvtnkcum.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gxqltnmrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gzqncgzbv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gllhmumvm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxqfivdfi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gyslxwjvv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gfwfnukfs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gwietmtta.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/ghnsvugsf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfmttjtur.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gmmiepxla.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzwqnggtq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gsqblygaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbblmtcgb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gcuppfmgu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gxmxcjvsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/geinxaekn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyqmpehkb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjczsqfwe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/goqlxqhar.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsvlopbhp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gquleyblj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gnxninpei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/giygohyrt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gfokxmptm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gasrcwiqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gwkrgkpuk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gwifutfmy.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ggiivmmzt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gjphcathr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gxcuhcjlc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gtgpjfkbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/givmrzxvq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwoqqubwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gncxovwjf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/ghwsdtpux.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gelrzpvxd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/guhqtexsn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gqqfvyoom.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gsjywfdjb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gyuykgjiv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/guwmexphd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gfephfaay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gaxlkegov.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gdjwtnupw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gwuwigolz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gbipxgtoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gsvmaowiv.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gcuscmzqp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gygcqyniw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gjhfvvwga.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/geyzunamp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjajxxngn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gvvwkndzb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gooezatok.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gjifbcbpt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gixvqojzo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjjituaqm.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gjsqmurlg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ggfixtajb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gthjcadvf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkbstuiwp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gximrxhne.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gwxnxxxun.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gegrboydq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ggghyiiux.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gzgjnhavh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gqtngrlcm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gfxmswxcj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gpfttfold.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/goiiloxso.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gnwsqtlkc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/godmnihtb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/ghplzplmv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gxeygigub.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gvbxgbfop.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gjyrhkubj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/grqvsozaq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gscgozbpm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggzfohgot.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzekshpsu.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtuaazrpr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gioeuqbvb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwpsfkuih.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gjfpmoyqj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gcatxxcca.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ggzdmwgyr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzlpzxocv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gydvdeheo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gerehgzut.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/glggamhmh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grtlupwcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/goeyuutoy.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gsyhwjoqy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gvljakbgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/guhahqply.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gsoptsulb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gmdfetxoc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/ghswokswt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gasxeboiy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/grnovciax.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gjvsgexqf.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gfqbykksp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gxzeutorm.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/ghcultvou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gnacdffsx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gamquwbmf.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/grwebvswg.sHtML


<!-- 参考信息 -->