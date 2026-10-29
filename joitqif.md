代发 wailian999

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gytpbtcwp.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gbkbuwtpd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyvtfeqkm.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gutqagqzt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/geaogffts.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gwapctpob.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmoxradtv.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gkdlnmtzs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gayovchxg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gximlmqwj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gguuurkek.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/goxtqkejc.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gubmflepn.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/ghpcwadck.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gxcvlralv.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gbkbklvpm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gjktazylr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gtjdqqwid.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gwheiecjp.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gaqcgqxau.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gioouijer.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gowbalnbx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtlgtlqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gargbkaxy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyirwlrxd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/ghqlfvenm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/glfjngdsj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gkaswsmfw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gcloztuxt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gngnubvwm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gafzgpohx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/glsykgnge.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/ggzhggxhm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gydmtyyrz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gcojfflha.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gynruqkti.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gzjvdlqjg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/ghtdjmivy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gmebsjpdz.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/ggwgzyule.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbegmoydv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gdvuhhwzp.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/glnipdops.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gcnbktoqs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gmwqivtht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gthejniif.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/glnfzocrm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gtkxmrozd.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gdtiwmbqm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdbbmnowu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gmsnvgdfu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gqwigzrkd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gfbrauhai.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gdomwqjah.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/grbttajal.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/guoyzbdbc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/guvwkevhb.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/guotcpugd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdbtipxjz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gvxdmoois.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggezfydeg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzwzcbsim.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqhngugxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gmcxbigkz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gycabwsxq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjavluhoo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gjtmcuott.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gitugdqbv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gxttiiiwv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwsyvxbxl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/geaekstzp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gmlzprfci.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gnjstrczl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnpqgjsde.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gzgresoja.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtxkxkjur.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/ghqoaezzl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwjodfjgo.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gzgypynyu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gvmzqmkyb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gpeyuwbge.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/grfykbwyd.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gcrpawcxm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/goudlvowh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gveudopgw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gqlujzfwb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gvazfwglq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gkmlmzyrs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gjnbxrybv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gtbckczgy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gdemeravp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gsqetaufp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gzijwarhf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gqqzwhtcm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/ggkgocyik.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/galbtseoh.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gxmidszpz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/giclgfify.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gblewlgxm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gcxeaeqmx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gkwtigkhw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gstyhyuit.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gndzwapdv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggyfxedzf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gfvzmjefz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gpseyqnjq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gxkktpxrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/goygriuhu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ggidycrgn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gkbalcvik.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gmvwknsva.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gjzvafeoq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gcqzzqihh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gldnbokfy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/glmjvzdlp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gfbcqfsaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gmpkcqxbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gpkjllvwo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gfbqpquzf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gcytlumjd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaxceteft.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/ghbjrhxaq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gropkfwkd.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gitwtjwky.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gwvbshrag.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gkvuwnpzw.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggqoujbzt.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/grorjtsay.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gosrizokr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gypdxzmgv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gtpftttqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gkgwbknby.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gejgwotwi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/grndhiawu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gwvyzncpj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/getcuczof.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gdpwctrvk.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/groajcwno.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdxolepnb.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gebqponsr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gzvpeclms.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gvrvlfepk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gecfckkxn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gpkvhauay.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gipnjsiqn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gkualkjeh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gkmmruhem.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gsozkvttr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gsidknwnt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gcososrol.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gylxvtjmh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gavrmlqkr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcroaizm.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gcixeijea.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gyvzuqxah.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gcvectjmn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gumnvurwr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gneihiqoi.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/giihxvkjr.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gkubcwxno.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gvpmzyxsp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gknrmdhog.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/glakcyfhn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqrcjkwnk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gzvdtqops.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbplugeok.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gvjrwanod.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwbwbbhir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gltglwxur.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/ggntfrypb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/goiyylexa.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gmykroeqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gyoweumgy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gyqxmendg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gszfpcfbq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzkaissid.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gcrhovjzp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gyoqkxjun.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gxygngkiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gxxlnicly.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gxoqoswva.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gwqwbtnyc.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gcxqzaowh.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gofxiikdu.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqwdebrat.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gdrxfycxp.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gggehukht.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gjmrbdygq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/ggyxieboq.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gpartqnwb.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gcxxwlcbb.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gwierltpx.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfbzjgxxq.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbkargea.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpjbsvgqc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnjezqpwu.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gntijutum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gbgqotvyj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gketdyrbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/grsskggzc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gjjkqhhvn.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghogjynas.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gsbnhvhrk.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/grygcrdyb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gwqblhxtj.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gamxhadrx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/glmxsmxyd.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gquubwcpm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gytvqgwfm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gibphxpkq.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gzcqheecy.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gxxnxhgxm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gueimxqpj.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gvlssjxga.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gmnqsyavj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyeqjvkg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gycftggal.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gunddepuf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gmibpaxvi.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gpfesrvjh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdvbedznw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gkzlgzxnn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/ghlohwqnf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gfolqbdqz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtneplmdc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjgwrnhtu.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gzeazeiym.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsuwpvhql.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfqdzriht.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvynhjkyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdbhnifwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggixobogh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gyeclrrav.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gprdhwcwp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmzdttfje.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ggtbxyejc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gphqozchd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gyunowdkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gdsfzjmpj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gcymszxwy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwdxuaomm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghpncpapr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gmhiyzlma.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gehidjgfu.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/glmdovqiy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gppgafogg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gbuduesbr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/glbbdkygd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gajtseedn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gqkvqmedi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gpspwdfya.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/glmmioera.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gadbchago.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gcqgigmxv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gtfktvwzw.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gvddeqvnk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/guqovloru.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpgzloncr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkcopkshw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gemdgcoct.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/grnpyttvh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvdzbllma.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbtkxyzye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gsvaqmyyf.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gmpntiziq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gasngbtma.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/giveacemz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gtutwjjiy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gqrzzcxqd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gzrrytxkb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/geyjhordv.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gelcapenu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gohylstyj.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gofnfkypu.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/girpwkyjl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/giofgiicj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gorvhccad.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ggozummpg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gshheueeu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gsjgyvyuh.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gneeptvnn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gzzklgpvr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gdvbywxmc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gvzmmtreq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gymqyfqtw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/ghyufsyac.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gchidqahy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/ggkvhozae.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gtnzfrmtt.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gomsafbie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gbuiihnjh.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/giksuyupx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gardfjbnw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/geopsqnmf.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gulllftdy.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwfhzogxd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gerzbushq.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gqxrxxxte.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gukjsafbl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glnukylpg.sHtML


<!-- 参考信息 -->