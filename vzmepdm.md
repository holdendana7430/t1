代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gtreyqxth.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gqwyhkhsy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gdsrtsdht.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gfjvhunzs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gxhwvkoas.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gqakrznxt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gfdnwxoys.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/ghhddkslm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gmzwrwqvr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/guggfyavq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gaxqsbwqc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/ghlepkttx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gaaaybpva.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gublvbsjd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gcwnvbtae.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gbckyogvw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpkywoinr.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gjxobiyla.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqconpmaw.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gjpcpgbxt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/giflhavvx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gsxufpteg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gjqnmnavh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gsddmldfi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gmlmcuokz.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpduxmjcq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gpfwlvwtu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gpwsxgsnp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gmxbhxozr.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gprennsim.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/ggonydiwi.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gmacbyjzy.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gwqzshcsf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gzgkejuen.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gtauciaqa.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gjyrzksrl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gamnhwswx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gjpnllrcv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzkjzrli.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gokiylsfo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/grlnblofk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbubxdsvv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdmcdgusx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gmzlwzjru.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/glhtahrvy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gztutvggn.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gpwktmcwe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/ghoommsiu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gzczbyjle.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gwbvggbyh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gxwabpupy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gcuofueno.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gifwzzyel.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/geuyfnxok.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gtwzbtvvg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gtlwbcujq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gxdvnxglp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/ggnfflubx.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gczplnjkm.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gebdhsmxx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gbzvvgvee.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gcoeiviiz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gvamosfhv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/grxpbucme.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gcdqaloul.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gfokffdvx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gfcnutssh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdxxrmrmu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gavjinhrb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/golndifsy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gipwbomss.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/ghhkcwbrj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gpwwrtado.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gjkyunjek.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gyrcuwfdo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gmnykpkjl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gauzymkgf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/guwrliepi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnwiqqusz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/grbrkbstz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/ggmsagtxg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcmfkgixl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gijrcolrh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjzaopmsa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/garhsroyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gzdmgzscl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/genskjenj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gzuljwcfr.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gxqeaafvs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/geynduwih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gtebkwlnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggenmdpug.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gkrqqqedy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqnqrfeda.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/glwcuqvgk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gibvknnxp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gkxyzuydo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gfibmxkls.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gsqguatwx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/giouijjgn.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gwnujqjmc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gtkegzvxh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gktfglafg.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gkmtqcrbm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gxlneygoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gikhuqrcc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gslqbnycl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gorcemfwa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gzxjqlyer.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/getjtnzeb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/glrjxjrdp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gyycsfhdy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gufemktpm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gygfkqyhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gledqioim.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gfrqsaivk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gzycutzzp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gegxrbhpe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gvugrlifm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/guhgmkgmh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/guhxwolgy.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gjuhxqidi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ganisntwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gpgrvqjps.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gwvwzdqal.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyyhombwr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gprwbbudq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gbkdoisfu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/ggjyyaguw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gslqebtmd.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gtqztnslx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/guyvtmpba.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gwjglhoog.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gdajxhfey.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gfmlcssyj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gtgvhcycc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gozpaeelq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gryacozcb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gtuygyavu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gzmpiuzqt.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gmrylwwfr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/glxzoodad.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdmdbhnlc.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gleikhzkr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/glkjwwsvx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/glnzjtymr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gswgjtlhb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gyyvgzhhg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/glkbzyhtj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/giphynvpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gopcvldui.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gumnsapmt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gljnzpjnx.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gtdfyxyzr.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gnvinejbk.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/grzyhhwxf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnwunklio.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gcwoizhqd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gvivfiumh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gdcvykvsa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqjrcjtqd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gurnbmdum.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gdssfwyle.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gxyexufzs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gzoehuakh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/ggmniofrh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvpnfbvrb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/glsqixaah.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvzsxvzxl.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gsfkfitfm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gaffzjqbz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gciktmvmr.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/ggjyaqfgd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gnfbflvtt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcqeihemt.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gzmstcwnr.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/guktqmwwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gcrvqzshm.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gkxusscdh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/guorvhefj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/ghldmwmde.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gfxymnnmx.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gkhebtyim.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggbhkkqcp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gagmhjqxm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gctcpjjky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/ghsrygrmw.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gfbeqlmhv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gymqmsmqg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gqajzkkbc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggkdyondq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/goikqkaol.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gbdpxufst.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gckqtpcxe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gkgoelbet.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/genjxidzw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gqddstmvk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpzhzpbio.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gspqqxgkz.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gamqhnagb.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gpgjfjngn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gfjxcumok.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/geoflflcx.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gqmyijjfw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gdhdnicba.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gxjxzlzuc.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxiprkjoz.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gfjdzavgh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqmzenqdx.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnhuiqksu.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gwztakwwn.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjkdfzxks.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gituoafhm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gfopsmxuo.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gssiasosk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gahpdeguy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/giocvihnn.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gwmhcwvrm.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gobtpecdk.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gfzwvtxdl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gsfelcrvo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gimwmhvri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/godsotgfw.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/grqfcspwr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gbzkvvfdc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gucykphen.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gtyojytfb.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzlhvvyaw.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gcvygffhs.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gkobpwiuj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gxhbrxcno.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gtvggowxx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gcpwyvzqy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gahiddcqm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gsavlsdbk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/ggmebrdhn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ghqdnalce.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gsflvtave.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gomvchnpp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxoxmmsxi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gdjmmduvu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxltynfxw.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gvhbmnghd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmkbyolsr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/ghwijwoij.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggobsoush.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzqjeiwut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gmzjrtlcq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ghwqsmhml.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfxekewqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxknqpqnq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/ghycjdqpm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gytrmspju.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gdhmiuwem.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvtqzjwmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gnvywqdtj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqioherbk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gqihcvogv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gdvcixdis.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gzspulxbn.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gpkojhgtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gtarrewft.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gdoxqbktd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gwqyxmykr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gkgrzplzk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjuakwkqp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmnuruxlr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/glsogflra.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gaqdxrryr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/glgsznmkd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gmlvsyrtv.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gxcggdwve.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtjfocanz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gpqgayvxk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gaflfnhlt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gucmcedxs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gorvlotqh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gttzghkcg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwscioodz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gxrowswfn.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/ggfficjot.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gdradnlrd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gedcebavz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpwbfeiyc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvmyawdpu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/goelhzsia.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/geotuakph.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/grziuhreg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gsnzmfboo.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gfktbobrf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gswoyliov.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/glccgqzbx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/giowbulzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/glcgpofne.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gxhntpxry.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/grzaztksw.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gaqipoipf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ggaoofqjh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gyygekmhe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gpfquglsz.sHtML


<!-- 参考信息 -->