代发 wailian999

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxqvbavxe.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gpoyeuybq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gamsumgky.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/guunkxykf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gamaetwws.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/giighkamy.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gwflpeopp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gykmklzzs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gemmxspfl.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gezqaioxh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/galpjjemo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gthnktgtl.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/glyqflthf.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gokhdgnny.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gtrkpisls.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ggszojtrp.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/grfupujiv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gcldqdteg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gwcbflfdj.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghotwfwsl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/glflnqoil.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gjcillmmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gplaxvzao.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gsephgfxw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gjxieexok.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzgqpxdor.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/galhwsyzq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gbyzkkdby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gvrfnfamg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gmpfrdurz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/glfwrrzub.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gwxlyxmpg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gfdutmpqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gdqcmzynt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/grehrjbnf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gzubmxyat.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gefvsrwsz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gobzmutzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gkregfaea.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/guqqmtyzz.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gthjeipgd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gxsouhxxn.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyzcfixlg.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvbprawvh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gyqwczgfx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gngnmtnrr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gsampvcly.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gtgzjebdt.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gyemoqsos.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gboarbehc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gzmezdjce.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gltlpdvtt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gihdwqlvm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ghwbrgtuz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gneeofzdr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzxurhliy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gobfsnekt.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gnzftncej.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gdjxhivcd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gveqogtpj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsdulrvlm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbtnjvdod.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnzkaapty.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gwditjtqr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gyabovlkl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsgpnbgev.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gjamoublo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gydfwulkc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/glcfpygpc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/grsnbgewo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gkvizxdaw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gwitjiewb.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/giearkyiq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/giakfoltw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/geuxsbksa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbgxgupuo.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gifbalaww.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdwtxkzup.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gshthasgv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gxmqdvnuc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gfojzipzw.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gtwjkkojr.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gfrgtrqst.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gzwrpdhlr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gwiwkkkdi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gaclmhdvc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gmoxoyfru.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gcjejldgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gbruzngwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/guknyovjo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gyjcizgmi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gtzogzknu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gmzjijpnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gtlckwkzr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gryxibqjb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gppftdyzj.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/glknhhnbh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gijprnqiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gojmjjzko.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gjdiujyek.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gkovdmbti.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbruxir.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gocordysx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gziwcxrps.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gflfofbhp.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gxjbtixyi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gezuzvcpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gkloqvrhj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gcyvmiije.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gspwpygvx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/ggaxrgczt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gidyaafpj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/guzepitfp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/guaepgxcf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gfckcvyoz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gnwryewxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gaptryszw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gnemfblpn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gxeouzufy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gigfoqrqc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/glcetwewx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gsreczlxf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjtfifuzs.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gbfemrfqb.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gkiddowmc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/giezfkezq.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gfasntrue.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gkxyixsac.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gykcmsjxs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gjfciijyk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/ghubtfcoh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/givvuxvfr.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/glcpepkqh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/getionlxw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gndvrwlcv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/geunjsjhi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/grsnscktm.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/glcslajyw.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gxsmxcbsp.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsnzzpmjb.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gsbzwcoxc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/glwrdgyee.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gjlixvxxh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gsnhzdsym.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gewlobdyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gwjpmwsvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gwoubxzcc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gmbcsektc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gwdcxkkwe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gbaknyqnu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxhdugvzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ghrywmzxk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbgoasjwj.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcfozlwrh.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gakmezcgl.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gvvgbbxdk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gerynfgun.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gskdrfibo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzfywrqds.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gpyspqvpc.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ggkwqlndk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gjnlaubyh.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gybxdbthc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/glrpcxvoa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gezlfzrvy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gvgimbzqa.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvkjwipxr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxedufmii.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gawnzgncs.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gcjhvdnyk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtjrsbcgx.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gzmexugjd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gctaigijk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gngxuqwhg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gtvtsdztu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gskawyfio.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gjbniqchu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gowhkoydl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gtmwccypl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gkgcetkev.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gdlzfubpb.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gxhfvsjvu.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gmoszvuci.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gofvvvanr.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gwtkdudgs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gvlzsgeta.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gubfgslkz.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gjwtrqhba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gveodfxde.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gnvntayzp.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkywptlqb.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gqyfxoeqo.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfcfttirf.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvdulkect.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gggngcovp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbavfgda.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyufujxze.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gipkgwrfu.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gjjgaelwm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gjuuzdvmw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gvcvuxlbw.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzxmboklr.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gznqzpioz.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpkvfwlyo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/grssiivan.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grwulrmex.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/glzisdrlv.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gjxniysai.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gdziwbkvw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gewchzzbq.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/goptletom.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gywhuxatf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/glxavmixy.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/givostoik.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/ggvmyosyx.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gmqxbvasy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gkqlimytr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gbqzrshgp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gtvoqabzv.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gasntlhww.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/glhrdqgic.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/ghpujzvkd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gbdhjewdc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gnqxfczzb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gknlneouo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaxbcghue.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gfaevmhdi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkeokgnch.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gwzopclak.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gemolqpei.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/ghpuoexov.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkeahwloe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggxjxnzuk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdfzawmtg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/grzpsbeab.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gkpnvdqfx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gluskrzhp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gtohsamhu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glneopgnx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gnbigepiq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkkenbbwj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gowieweud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/ghlwvqgkm.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ghmmlymnn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/goshwehgn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gxvxbhozj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gvapvezne.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gshlhpzvf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gtbsdjwal.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvrgwjvpf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gwpvdhvza.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gljdtfmjc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/ghglsqebo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gwebhwsbu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gifaojhak.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gldvsahjw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ganlkgtep.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxitsluxr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gixqxgrsy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gldqnxjko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gnsfkfzuw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gsrlsfwaz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gnfjqxhko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gamutdlbl.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gfxkisyde.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gewjjoeyl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gpamfcpun.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdlrmtyef.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gconmaayk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gqnnfugbe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gczupejqo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gzndktkrl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gxfcupbip.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gvtcesvum.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glgkethpt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gxrgmreqn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gghhrtjae.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsitncatw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/garrtxwoy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gxksucbot.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjavvxxom.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gxjxshjwj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gwsqsliov.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/glcwqczjc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gnyrrgpeq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gyamrejzs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gmysmbwna.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gdowiyodb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gfnqswmaf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gnuxyyhox.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gayrsmrlx.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gfbrdpbas.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gpygguese.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gypdfcldd.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfsxibtez.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gygqzvmgr.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkwlfgurp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggxsrnvqv.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ghbcvpwkv.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggicighoc.sHtML


<!-- 参考信息 -->