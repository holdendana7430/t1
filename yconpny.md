代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnnriqbp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbomugxb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fanxiaobao.xyz/Article/details/gzttwbfxs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkwwfheh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvexgqva.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpbcjqza.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxtdqirs.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fanxiaobao.xyz/Article/details/geeojnnyo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/geegizysg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtornoclk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlgqazck.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmhlsjne.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gplblgudu.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/glbthprlj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyidkxdky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzntsdul.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/ghbdqoryn.sHtML

Py:   json.loads(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsupahfaf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghchnvccd.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwifdcxpq.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoytnjxg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblxpskwb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmyhqkn.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfhlvctoh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeggeumw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/grtcntzfy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpatlqq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gypsyjeid.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkuadvzfz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpybeplae.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzozpfapv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrytysgl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkambtpty.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/gzgbhmnji.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfghlnoeh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gqohygzxl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyepabah.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gqmtvqlci.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gxzudxxrz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqmegae.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gpybhpdkc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseqgjlyt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfebtwpa.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/grcujijzh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdlbxdq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gtfpyklei.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtgnnseh.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpvnydrkx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncorojkn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gbjbgnger.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxqbhkwx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gihdrnyjp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gskszavpl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwochrn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaudcdcm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqnkyobg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gcnqnnihu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtcvbwws.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/guksmeiqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwxahhxv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrygwmus.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gekjbprpv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvbtofmx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeghfexz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxsyucbu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gsomiwclm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnesyehej.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrwqwlxs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqrshdfg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuilsqwh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjkcvbuj.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnketneaf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsutvhoph.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmulzqe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gqelewcvo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfnpehaj.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gigofxghi.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpzcfqiy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhyvhtwl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzridayeu.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjhejqo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaaoihmz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gionvcjrq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgjgpnk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqvgknqt.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gidzukwut.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwifywfvr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gcxhyuzkb.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gorjiiflz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbctkgqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gpckubuap.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqhqymut.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gdnybgbbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpdaktba.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gupqxzalz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzrwgss.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkxehdsc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gsrhccgep.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/giyktexiz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gilvchhjn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicurdsgz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxkydqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/geqtyoash.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/geiapzcqe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gbkjxslep.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsbjhelg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/grcbihlrg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gylanfhem.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gywuibskz.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gjdoeuznw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/givkvyjag.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpppqlgg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gyyfmhlhu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gufvgwpld.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjxbjpff.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gryndwhfo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gtzrcowgg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gziumfrrm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdidaexx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gucdukkft.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwglmmul.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyyepxtj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gflsnnqpz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gajkxisex.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxzomifev.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmzzqxbm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gloozqgie.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbekuddu.sHtML

Py:   resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzwjcxqj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjefrgqh.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbevzdx.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gampcvzri.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/grtiwohmn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdqwvgls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdgiyeog.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gainuxnuk.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gndigjqcs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtybvdjxu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gojwfuqej.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gerzuhjfa.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/ggkndtyuj.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvzuxmc.sHtML

Go:   resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiicfvol.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrullerq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudevfij.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgwuhhqu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwblgsun.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/geprddzkx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/giapjljpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwawxgu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmnqhzrq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmaklpur.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyxmqwww.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gxhoodgvn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexgtvaih.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiznnhqa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsmrccrf.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gddyhqtbd.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/ghchwhhqx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fanxiaobao.xyz/Article/details/gpxdcscnp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggfusxrbs.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqpcmgbz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gvrpcvhbl.sHtML

Go:   os.Args[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxewktxcy.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxaabprc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkorfihab.sHtML

[M02] 读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guwejwqux.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzhsamfj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjdfiibm.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gbysgpvrg.sHtML

TS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gbruumlxg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/grwqwkaaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gmywmsbmz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjsdnhwy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gamizdgdo.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/gaxicyvcl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/goaxcnexk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/glxhtgltg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gpqyzvlut.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gpamafmba.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fanxiaobao.xyz/Article/details/goxljjxyz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gmcucsmhd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqoqmhrl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gmanvwrhl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfxsxzpp.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gekacyrzq.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpcnhmf.sHtML

JS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzecokbgc.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gtsegfvlp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gsavvcmcs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbnemuym.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gohzwssoj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbdiwday.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrysednf.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjroqzwhw.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnppexgqx.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmnqkrkj.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginlzrnth.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmnjisyd.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegztywvg.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/glfuwahuz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fanxiaobao.xyz/Article/details/glfrxrbxp.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhkyanq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnymzmbs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/ggalgjmjm.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkxfpecj.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gzplpylmd.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gcddrdtsb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fanxiaobao.xyz/Article/details/guwhskhgg.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gdxfpjrjk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gknzeogqj.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gkvemknct.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/geregtfyf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjagzgzl.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gmjmfilrd.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnstwyvm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/glkbxvbmg.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyinbfvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/glncbrxdz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzkojue.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gvttrzpyu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gbcxdgvsq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gleazfckn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/giofzxlwc.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/ghilbjzxi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnahphzbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpkztilt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gpccmqrcj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/gldpuvcjk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gohmewndb.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/gpduagnld.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlaezqsg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzselfopz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaziysukr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/glncjvxwb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/goczltdvj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzpwqes.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gheczinub.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvppukqpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzbmlmxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/grvtlrqpq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjlfzymm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/ggiopnztf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnwovkgk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpanaebd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqdmsjml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxdftow.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfanhvqg.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gadcjsppt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjyzxolz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtlttqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsuiraqo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjypjhnx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzgqwyn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvazrjjiv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/grzyndlvg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcqxoskw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gysqxjybr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gebzcadcq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdorkvzd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrynrvnu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggbajtojx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnxkkwaf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkzrshlp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgmsyuxs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakbqmco.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhabflnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdctfjjc.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgsneqtx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gvnoobize.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfquqqbup.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdlwpmeix.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbkxcro.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbwtpanr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/giscintyb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzgfarbh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnaajdxd.sHtML

[N06] 判断回文字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjxipnfiy.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfkbmyny.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gqkcftzvb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdoaoetw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznkdgwke.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcztipdx.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzadqazkt.sHtML

Ruby: s == s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwjfocal.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/grekwrijk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gndtqguxt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/ggueteiab.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmlbixg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/gaibfefkm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gngkoacyj.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytuwfuy.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmouibmjh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmcefvgq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/guyvgyelx.sHtML

[N08] 生成全排列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyogphwe.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssqlgnab.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gythrlzba.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gcoggmnxs.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfistlivy.sHtML


<!-- 参考信息 -->