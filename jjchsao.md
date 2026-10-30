代发 wailian999

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaoywgbbz.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gwbmmqtlw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyobtilue.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gaxqpmmvo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gboebrhpb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjxcixrxj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gjqognnrx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtcvkplub.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gcvzqghjf.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaqishcrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gyzxmvvbn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gurmlzuyy.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gijckabpk.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gaoazclmf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gqyehtbqr.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gitqywoxa.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gtcjhdbuu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gihuxudhv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gbkulrgqs.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gbyinijsa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/glgohcsiz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gdwfrevjv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ggygeyybh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gxqkigezl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/ghffrcywb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gelrujlsy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/grnspzfbx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gavsyrlhz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gflkgysro.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gvbtodiyw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ghumfmghn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gaaqlyxjl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gnetqhmom.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/ghyudidtx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gqhqvjshh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/genmrbnsu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpebaerp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gebfqrqxv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gouqixfgz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/grtglejlk.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyoaiodfi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gdspqiykn.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gihkuhppp.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gilsmsnql.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/ggtfhlgyn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/ggfnbkdvf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/grbxmpjac.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gnhkxldhd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gkgtfvnwx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gvtzhnxhi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gpppjdrjr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/grlhiwhii.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gyobtbqit.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gsrrwmisl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjteqolfn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gmntioqck.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gnamtbtdg.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gkaztimhy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzetaoolj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gnobopqnl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gvjbphzat.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/guwkoaect.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghighwceb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gzfwxdacu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gujdzgreh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gpftxjona.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gljbvlury.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gesllpxou.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gnqjvvguj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/giknrsyre.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gpmygttdm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gwwxfabmi.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gysghrduu.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gqnkztoax.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gbpiwxfec.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghelwlttu.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/guqreluxu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcaklxacu.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gedyzuexr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gxpficfbb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gkjbufysq.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gwiclwonx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcrxwuq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gonveryoe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gcdjhuwfe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gaeewvwux.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gcflrfrhn.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/glseirtls.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzescvhxz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gtticvlbm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gvitxsbja.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gevktvqsb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/grgxqlfyh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/glssrnuuf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/galizmeqz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gvxmctnvm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/givscxpjw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/glcjcsufe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gdmlgezej.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/grlsoudve.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gfjhbixhn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/ggtrirxmz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gyvoocmix.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gqgwsegaw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gdhhazbok.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gxnlcxofe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gkpfhncly.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gykfzpfpu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gcgoumogp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gxpetewop.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gbipvnjda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/grxzsopty.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/glyqzeste.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gynckoxjo.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/guyfzkbad.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/glmxyrsqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gajqjjxrw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/ghxvstsgb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gzahhseej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gqejninlm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/ghmrauevd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gqdwjlbzb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkugcruvz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gwbytstxw.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gwpwhzskk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjagfubmm.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/ghyfzebqj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gmeyisios.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gsaykoace.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/giwhihxqo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gkezmyyln.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gstbrkrki.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghdstokjd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/goktufmmz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gglmgvfcq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gapoqnfuy.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gwylwesav.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/grxigdfah.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gjkmcfvnd.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gnhkxupkr.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbwzmubne.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ggcwmcraz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gkwkcnsjp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gorbxvvgp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gshkwnuni.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gbxsnftan.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gngemvbso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gsymbmgxc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/guqqvqahm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gmglbmfgz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvxhdqmig.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gtffnnbcp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geyikswza.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gvlrkijel.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/glsxydnyz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gdgrxokon.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gofvomian.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gmlapjmvw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/grdccouor.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gbbwimxlg.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/glbhzajks.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gkexnlsrz.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gttgakqax.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqcngneao.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gdhnluoak.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ghnwxqvqd.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gbeycwdvh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gezbriknc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gkzczvgbx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gsucfabno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gscwbaswd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gbadlejfu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gxhpgtkxb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gnckrjebh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/glscznxfq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbkizqaua.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/ggeblbuty.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gvjgjzpfa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gjfpxragb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/geipmcpif.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/geyfvvxrq.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbecwsefn.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gizqvemqe.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gynkpaldn.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkjbhhmja.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gtnidosyg.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/glqdwgvds.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/grrvrvawp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gakebkwsd.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gutjeeted.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/geccoojkl.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gtsmkmfhs.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpzjmkkjc.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqvmtxvhv.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvflkqqdn.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gyuidkzfk.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gawqaykyk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gydyapruc.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/ggxrqulhs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfsapgurb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gqyhkybii.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gsbskhmgb.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gkxcjrief.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gtiskfzdb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtqvfvl.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gsxwjkgka.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxtaupfwn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gcaifppfb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gdfjsilux.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gphesxujh.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpturtcpp.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ghmaniyjo.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gafjiplgi.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gnbsvtnpl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/ggoehrgrb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/giieveeny.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gqqbrndpv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gkamzwkkx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gsrhhjkwj.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gvcywuryj.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvodcdtze.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/ggyzgykzg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ggwpgvsbf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gpqxyssnp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gszqhhbkg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gclcscbzj.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gzwnziqow.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxwdgqzfo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjrjykqud.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyhkfptpv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggyrcgjgy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbjbkbydp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gunxmvgek.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpxadxydr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gozdakqym.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/geboyeldr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwwrvtelg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gffvvueph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gnzxsldnk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwzawfkzo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gybzgecsz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gcfiknvkb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gmdtvbcix.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyojryoge.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/grvrjmmkt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gwxxkcktc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gnwijrhux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfgemyesh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/goxcfcrfw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/grnyjxrgu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gbsdhwncs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/ghedmcfrq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gvkrfdctt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gbibyteld.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gatywqjgj.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gkanbhxeq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gifeajmxd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvumpnhas.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gecodfota.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/giutfnmsa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcxnebrmy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gqpllckoi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/glhifmaik.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gdrndykfp.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gqdkfllqw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gydwhdiod.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzdkuenkw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gbvnhnbky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/goegnmipq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbcsngw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gpzliohih.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gvftvnngq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gxgxhpdrh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyexpgqyx.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/glkfgurpy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gwxtklzln.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnkzupslm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghccrfptt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gkicytwba.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gfkczejnk.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/goruhwheu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gjmtaegsc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/givzpwaqu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/ghdiuxnbm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gsilpbymm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gwhivxaun.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gfxuhvdfa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gcmdwhflq.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gzwedfuze.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gkdxpezaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/geyalehmi.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gholdkzgs.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/glipbiuvj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gobyhpcna.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gehcrtogv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggdsnwilp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gntsemycf.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqetvdzdk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gfsexhiqf.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glvkhqebe.sHtML


<!-- 参考信息 -->