代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gplfbiplf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gkindcuwh.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gqusxqzfb.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gdnnokutc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/grqdzoqub.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsbjqhers.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gesofxwzt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpisxcgrm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gnbgctlik.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gmxgyuvpu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gtykrfwqj.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmufudiej.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gowoymqoq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghglnvdkl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gvwkqgadv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ghtqngoat.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gtvrunntg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gyrkjclzx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/guinxfqhp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlcitxnl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/glitzlrlf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gkpjhyksh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gnwzjlcgm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gobfpglek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/ghputmmlr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/grjrexcde.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/geraeddud.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gmwjgufhw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gpunzpeey.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gttypxgrb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gcskmkcae.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gsgmawixq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/giiijkgfj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gxdxdxoji.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/ghhodwxfm.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gfuzawwne.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gvquvvnan.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/ghesjamlj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gepoulemz.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gbbnhskbz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/ghpwejxuj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gxkiytltr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gomvofrzt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/glzpecncr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gevucbhcj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gtlvfkcht.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/ggavzdkfk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gjqqetllc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gznfewlva.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gvbtlbexn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gutconxgg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gwdvyiplk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gywvmvpxe.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/ghkqawiyt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gxhdlcdpv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gighzxumb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gmiyxpyol.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkaxuuzxa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzzxvdtkh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gnmlnmqfc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gajsujifs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnpvjqkum.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/ggmwhhifo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/glhtscvos.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gumtksuov.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/giarizjui.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gqgxtviax.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gzuodalzh.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gkbpqzrhe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gwjonrzvh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gymwokpal.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbzpwkwym.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gdnqbgumw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyrckrrjx.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/glcgczwun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/giizyzeps.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gctcdqbzw.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gnifquvra.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gzkorkgen.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/ghosnhkru.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggblqwkzu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gbkvfkofc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gtzzusvdg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gprmyrsfw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gvlrivpet.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ggtndbphc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gyaqxokdp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ggtjvbseg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/grvmncact.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gyptsnuer.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gakdltplm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gbrwgehli.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gxiroiiqb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gaijyletr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/goqwxjduj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gdcfnzcej.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gjmhngzog.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggluypdts.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gxcgcdzyc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gxxdkwefp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvhbdczyv.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gfmgvoorl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gwpgsrmxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gucebvfkd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gaxnzezuw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gukuiyttv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/ganuongan.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gphnsaggh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfetcjpok.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gzxwclwsi.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gadskmhgo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/garoqeajx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gvdgintpj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gwzuztlet.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gocvevuvx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gdrbhgcls.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gojvgzyfn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/ghhqcwgot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gprholjsx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ghfzlesio.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gnshbsfew.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzdayxxpr.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gjelfkstj.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gyviljdvi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gzejnmudn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/ghpfbhbof.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gudwrujfo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gbojaqvvp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gyylklqoj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gzdabuvvg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gmonntkiz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gttyyjrnx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/giciseusa.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gajndsgci.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gfkoyabcc.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gemfvtwpw.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwpzuqwar.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gqkrpifco.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gjipbyzgw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/ggwoytakp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gviqnmzhy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdmqmxzcs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ghblhiuav.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/ghzxcfeap.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gnpqptavc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gxuqxxktn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmogxuxbg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gqalflila.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhpjxhgv.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/ghlgsdprl.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gfikamahu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gnlzumrmd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkvcliext.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gdmbjozag.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gdvmtaiju.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gkecrqfee.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gdznmwwrr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gbpxxlrxx.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/goucmqecz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtfhlxm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gxguxbwtz.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/guknuorpd.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/goismbhxm.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gdwxgiopp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gegbfxcvg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gqfakfwnu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtgexaukw.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/ggmozxjan.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gholwstlv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gblzjlpze.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gzfaekdqq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gohsaplps.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gububumny.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gzghdocjm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gmdufjsvz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gixszrleu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ghurankgf.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gmvwaifrp.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gtcxfcnst.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfdonmaup.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gszogsura.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gajodxaqn.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gutmokflk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/giybaeeoe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gywvpjvft.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gazdyiuww.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gawieiaua.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gzzusaetf.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gojwqaqoo.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gslvzikmf.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gffvazoig.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/giclidjko.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/guvkkimpv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gzjltttsd.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gmrgcjulp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/guczmnwlt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/glijxlvmj.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gztoxdcfd.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gysnajvpf.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glxzhslji.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gkigqityh.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gfwiktbhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gdywmbxwc.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gkbuopold.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ghptwsjed.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gdogtmhrb.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gqjfjvauk.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gionwatbq.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/guksjtgdr.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/goqwskqnv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/getyweppj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gweryqorw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gzkjkjdwc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/ghhvjzyzy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gkypqjiac.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdrmlewup.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gjraubvux.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gartqrkey.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gwkdpzzoi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gikislcxc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gsgoliwva.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcmkyvkdm.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gnvkaeyhh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giwjxyjcy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gurtloywu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbvcduyxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gaezpcwkc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gaayscciz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqaevwwlj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmgyidboy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnskxuyiq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gxlwtdmmd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdwamhwgu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gdfjggism.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gukidbpvi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gddyypirh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/glhqtsuln.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gilfkxoik.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/geqwjkxkb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzafcdalx.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwkphzeuf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gyegqwvuw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gdrucqhvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/grnwydcxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdlabwzng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gddgwwilu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gsvjdqdta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/guygjeboc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/garaatfuv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ggismbrnr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gogmdkkxb.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gipogpjxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gxtolfftp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gxfvjitrg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gltndaoiq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/geuiatyvp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gteemgpwh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/ghitythdh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gylgltqwm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gsaeevljn.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gicncrbtc.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/geffvebyh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gonlsbwzc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gbncffekg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/ginsbrvkw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gvubbyxuk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gkmzubgdb.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gftcycgsl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gciwsqznt.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjxyrbmfu.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gjwjlvnca.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/ggjuozvti.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gruhwhbdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtvyidsqt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gzkmlzqqa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gedicxnxw.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gglpklios.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gjqgdxuxp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gxeidpkqs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gfozdfzko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gwevalqxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/guuyvwoyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gouvblwhq.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gypltpjbz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gkdusytto.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gqtdshxho.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gidegfsxu.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gnazgxdew.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gkaaekgyo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gudxfcmwm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gsknftvnp.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzvezqwaz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grazcclzi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmnpvwsey.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ggfttcuhz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfujvaiat.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gwyghlwfx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/glhuxdlte.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcakgsrxd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvhwojobw.sHtML


<!-- 参考信息 -->