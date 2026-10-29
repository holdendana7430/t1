代发 wailian999

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfziqvnmv.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gmtgopmym.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gydvpberh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/ggokbasxj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gqvqlskcr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gqbqotdhj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gquhjxmoe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzztagogs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gmezqhovk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gslzahccl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gtjpxonua.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gegeqxzvs.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gjyogufax.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gznheamxc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gbhfmmkma.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gilukabge.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gilhipoys.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gcmynrzim.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/grfbrbmjf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gzhlpmhio.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/givknlper.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gltttpyoc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gvsrzdrlw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyemuiovh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gutvsctej.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtqkiabhb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkwvtdncu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/ggvcukwhb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gnwjqyljx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gtgpiebua.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gvyvxojpi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/ghekftdwz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gffqbimtk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gypqroxng.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gaqtkidjt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gwudugqig.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gpuiqjaxt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gozfdrakx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gymzivnxp.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gtfdmjbmb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwlwmwtcg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gvhealtxf.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxtxmlwbr.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gjhffakzy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gvziyosus.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtaincbw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gfbduabcd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gysruuvqn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/glckzaubj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gaeepaqsg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gtbidmndf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gtwiudxvr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gfkeinorw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gfjgpwvmk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gcnigwokl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gajywttgq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdpnhqvyd.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/glsxyseep.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/goxeqtwpo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gagrxhzhl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gttkkyvgh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grnvqscqi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzzmbvyij.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gwphdyjwy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvxxdjdbb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gqgzpgjdn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gmdzcicuj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/grknptfjh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmonruzmh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gtccwrker.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gkepcbzte.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gogkdspso.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/ggkheuzxj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gtbypskbo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gixoakcik.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghjapwvgv.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/goepxqtcw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcrsomlbq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gwsuodeoo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/ggscwyobv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gnmpzuxku.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ghaeyqesx.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gyrsygodg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gojynkrlb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gfsbwevjo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/ghcnmytqg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gnauavrlm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/ggnkuuues.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/giwjfcilg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gohbwwpjc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gnvtwuscb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gewrqmizl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/ghoameqrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gsztsuqqh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gwkncgudy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gknjyzacb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/giarkmuyq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gxurvelci.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/ghboulwpy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gkaxmxaob.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ghqiqbmpx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gfudomkva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gaxovymcb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gpwfbimcc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gbxpaihhk.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/ghdvclvpx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/ggwmxhwyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/ggfbcnvsr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gltmqfhti.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ggjpcwzuv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gohlytxli.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gmhtdowku.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gcyvqsfej.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gydrvloey.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gczkjznxu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gsupblvqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdgbgnd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/glsukvkza.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gqisdhogw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/girkqlrlr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gmdqtgafq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/goamnomks.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjnibyvvy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gxzwrqxsb.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gnfmvkfad.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gsucxkvap.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxgdwslqx.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbklqatqz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gsebmcxju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/googozetl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gyqzgrkks.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gujsnbrbx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gihfpaumy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gyjzvrmvc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/griggizzd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ghqtprqmk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gajzhkcrc.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gfclkhlsq.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gxlxkxqju.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gbllftlnp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjvazktti.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/grtsoetek.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gqdwdxbep.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gzsjnjzhb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gblhvhqos.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnijimyrt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/ghgcfuvfu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gtyqmbalv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gyqtawmyt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gfvuouzkk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glkedejjo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gjoypqswc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcmonoqqt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grybzoftn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqiwlkvqn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ggbebgrhk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/godnrxeiw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gmalptxzc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gpfmsepjy.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gkgqrbeld.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gzlunjwjd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gzkelbyxy.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/grntozdjn.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gmepaltqm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsbfzphaw.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gwyjavkef.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gabaauqij.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdfzaueux.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbujwthlt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gowdydeum.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gppwulyiv.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gbvaizero.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/ghwnijjqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gdluraaka.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gmwxyfapc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfyjqjfwr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gsgjgnyxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gtmgcmepn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/ghzcibhat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/guspznben.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gdtzevrgc.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gerxoshrm.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gdomftoqo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/garxacobt.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtyohxnkm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gbjzajtcx.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/glaouemsv.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/ggqgkpizo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/glwgqanyd.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gpokguhik.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gzxmukzpk.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/guidmvmvt.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gumerhizq.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmurbjyhz.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghezohmes.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gjfxnyzpx.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gfdhsqvya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gcbgynelp.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gvhpgylfa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gsafjutxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gehgqtyjy.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ghaoydcdd.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gilrbdbwk.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/ghkkxudxp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gcvmstgug.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gsfdvqxsd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/grymbqead.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gfnxqtdxy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gxquqkqwj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/guuiwjmlb.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gtnxbbbem.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggmdqwjbu.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gfmzebbrd.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/ghqjcuzsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ginafblsg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/grkczgopl.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gdfqrjjif.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gaheiiijm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gyyyshtmk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gpoeynumw.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gwwbqwqjm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/grqdlnyyt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gjmtfzbtr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gjaphmddz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gjllldbjy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdhklsort.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gncjxpyvt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkayrgsio.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/ggfjxelzz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzhseinbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gankhbteu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ggfbbhwtl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gqtuotbhs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gziicebxg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwidncqdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gbgdhvluq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfhtbzpds.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gltlsgvwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gfithffav.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gbzzxlzna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gulsvooob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/guzcialkp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gjrgvumpm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gamlybtfj.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gawlswvxc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gfnspvedz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/geffqwbvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gepaaqqak.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gecezohln.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gvmzavqju.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gihjhfzuw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gtwdpxgsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gbmhoazor.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gmzryqnlq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gpymahunk.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gmbglvykt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gvhvwnvfd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grovcuxkz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcgzuqlpv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjlczqocs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gmusmaqga.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gxheotyio.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gobcowuku.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkxsbsrso.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/golqgnmpp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/ghfbmncmy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsfucbfxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gjkgzdaep.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/geczoczyk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gybcuvife.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gelqxdlle.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gijlrkqry.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gchmvmqkm.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gkmhtunho.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gxbxjkazn.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gibcpenrj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghwqxyajo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gllfaehmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gxccbnsyq.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gfwbdlkrv.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxrdmnbdd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gtrzrfvnh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/goagqnpqu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gzdmplspa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gvkehlmfn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/ggsfotjya.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gusqpldca.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gsaxihmvf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gcgreiive.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gahsajnbh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gohmoljfr.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gcchcklgl.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gdxbtuzot.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpjkbxj.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpyjorstx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gageydkrt.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjcfwiugn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gavixvwjw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gscpdhwoa.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grbjtkllm.sHtML


<!-- 参考信息 -->