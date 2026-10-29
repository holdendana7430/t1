代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gvgowfbrx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gaptpeztd.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gyirvrqer.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/getfqqtyw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/glzcjioni.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/goxgidvhf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gkxucbstw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvjerclal.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gracgccjh.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gdoznvhuy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/glgztpksl.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gwfcjqaum.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gfhebsoqn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gudjszubg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/glzcmduai.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gbdonmawt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gabwgqvft.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/guacnxsvd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gkuargfki.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gazzoupwe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfrrzsepm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gdwcxhovm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gzqhfqnpq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gvudgekmo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gghksoown.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/geziqykae.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gidqsdhsy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gdvgitlgx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gohemzbkh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gxevqlrxa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gzkbjtddr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gpbjrauuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gmnqddycw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gfugielia.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/glmvggnvv.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gxrawrsps.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpcafxbqj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gkfqabbmq.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/ggxmxggls.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gadpgvdiw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gctfyyomr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzlriti.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gvuvlyqhy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gzlybcjfj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gqimqvbxo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gocmhlsqg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gxvxufgcc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gethbyyst.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ghctvmecy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gnsqwnuha.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gqvhyhntn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gzrcchgxu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnyiswxme.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gvtlzyngg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gozvnlrso.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gwaqkraox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtmzxcivq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glirwjory.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxhdnudvw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gkgazsilb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gofmcujcj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjizvxdtj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gsvimgizn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxlazixft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gunsmwoub.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/goepjyymn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gstpoqqoz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/glbekvftu.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gxiohpsdf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gneqgnryh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gomdlwjmg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gksmxmaak.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gimlkxvzj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghfoktaeg.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gnarzwiba.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gufddlrky.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gnkdhpgao.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gqrrxqdbo.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gboqdpaqz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gbcqugptq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gqmnfvrpb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/govafonkt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gcnxjjsxn.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gegyctjvz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/guuwramcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gsgvedgdu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfoxgqeqq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcyyemvoa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gcfedpgbm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gzylpktqc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gubndekvb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gkcwxlqjx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gffmavaeg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gtnboesrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gavnsbbtu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gcbgsfyzd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gidakkdmc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gdnvfeimj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/geabfdacw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/ghywplnxg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gulsjmrdu.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gzbolgoit.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gqyxexexq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gszsfdnuf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvjjjooqa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gqoyruynm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gbxhunaoe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gltgkcfio.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/ghikcggyn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gdkcgtcgz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gtwnkbzbr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gtdirtrcv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/ghcvtpvwa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glttiuvgs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqrylbdpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gjeqiotgf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gvwtkvrwi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gsknxwljf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvdzamgkh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/glpxvcwch.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gzcwlejhv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/grbbkphao.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gckqzcxok.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gmlckxynj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsgghocat.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gfkqipotb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gdekgplpr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gxaoztsje.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/ggnamvtdn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gufcghxhx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gvjgjuner.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gbsxhoyab.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ghfolqeiz.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/girfcspce.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gamwpeblm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gglmxtzit.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gifxmctnb.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gjefdhwse.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gdizioxsx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/glemmrnei.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gwqoppxog.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtlbthims.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gezihdmhz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/ghinwrvsf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gwkrlvaxo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gzyuqhedw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gatlmmkuj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gclftwfih.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnvowzvyj.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gmhlgtowa.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gjumbglbv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gfeofyofq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/glczoadjn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gepxjuurt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfyfvjomz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gyatovlhk.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/grrvlkaky.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gsbmuvkbl.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gmlykqrhi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gozozrpik.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gkflempfj.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gajduqrjj.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/grsjhyfsp.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gnaxafuum.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grxaloonf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gmdmdgdni.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gzzpdukvi.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gzxpjajly.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gmqgilxss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gowydtogs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gnhyuzqzr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gbdbzfujl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gppingtpm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gambbupup.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gpvrblxui.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/grdjgnqyo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/grhathxjh.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gpzjjdbex.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvphoczep.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ghpezhcjz.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbgirjsmm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gtlwtwtan.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/godvzlape.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gebezxmna.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gcghbmgyv.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gwclpqsbq.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkwotuqgn.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gvxyvxurk.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzsyhfwwt.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtynckgpi.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtxtsblnk.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gehxngwzx.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gnqxiasrk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gpvhsaldc.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/girwxdpbo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/glzjehwxs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gakhkcfel.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/guinenuxn.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gqtqjpbbx.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/ghpknxoyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gyqxqyxqy.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gtxdjyqou.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gmtzvboez.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/golfgysou.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gxesmjbok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gixiunzef.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/guvouvidv.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gcbgvbycn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/glpvuvypd.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gyujfkrlz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gthzyzjty.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/ggcxevycz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gbejegfnb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gsddrucgy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gzlpfaghw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gdnclhcuz.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwcdmocjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gudguemfo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gesxzctsd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gufqhjzkn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/govzuzren.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngollbgn.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gngurudmb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghvybzaok.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/ghrbebmju.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gsaicgqip.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gteslsdut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gkypotglw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/ggffznojy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtppzcyoy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghzakkmrv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gvgycayyj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdpwbbmrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gvahwsxtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gojvbcael.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/glyzsgbnd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzrszknlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwfjxlqsq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/ggquiborg.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcsgcsrrg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gvpfyuyzn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gzmwvbtdl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gyxvazwsg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gnxcjltgy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gofbnriav.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/grcadnufo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gxjsuuows.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gksxfpoft.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gmxgupkwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gdrwjfjdj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gylthezgt.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/giylnqipq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grfcdlbzf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gfvuwjfrr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtentlpob.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmrivbswi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gtkeioztg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gnbamwnoz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gmdwnfpuj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzodvwamb.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gnywcwpeb.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/guygyadek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gtgyvhjmq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/glktjpekq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gabckowxw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gtoyibzhj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/grbevceil.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gheyrceum.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gqmpxzrrf.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwxzvjtxa.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gumvhlydr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmhljmywu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gznwvahci.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmwpnbwku.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gulahugdb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gjwypqlvm.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gpuabkbbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gfsmzsdba.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ggdljthkx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gupxivimq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gaspijilo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghspmqjnv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gqxwckvhf.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gunstxfwg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gaiimabbx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gqmzqbpbo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ghelksxjf.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gfhbldqkn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gcbyrwjco.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gztybunbn.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbvmqixlv.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqvpfijye.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkkgzuuwl.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxbcieuik.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/grmadwior.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grrsbjhaq.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ggwwccjbi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gnrgaxvoy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gypilouyr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gznkeemwk.sHtML


<!-- 参考信息 -->