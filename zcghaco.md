代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/glzuyfzdb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gddtazfod.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gavzwggtw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gyndbwwsw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gferyocjd.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gqmbbapxe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grmntabhk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gvgutzsnf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gvaktdxqh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gugqururu.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gdhmalnuj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gdkjugosl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gijqmmftx.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gtfhovvpk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gjlgiczxd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/ggrvfvfco.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gxaabhdhk.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gblfslpco.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gwyaoqjqb.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/goffepxur.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghbdlfsjr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gxepyetkq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gvephwwas.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gzplfuxit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gukvnekhi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gxrnezdyl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gfdsfhxwa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gzqrkoxpw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/glyuejwjp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gntiyifhu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gptcvxgeg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gdptucepa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guxbafxtv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/grwbhqoiy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gbneswvqq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gjezxvksw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gtxcimsoj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gqlfwnrse.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gozopnlrs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gecryultf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gmbvlivzu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gvgfivgck.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gfmcvkocj.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gzeqgklcd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gwrgwexgh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gozkthmpp.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwjwyupxw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ghtjkwpah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/guztajbal.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gutsrmuxp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/guhdxttjh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gesoaxpkp.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gccojtqsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gdjtsagcu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gyhieuyos.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gcnutckex.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/ghshiltbt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gadqkwqgx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghcoiupyk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glwhhaszx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gainmfglw.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/geiecsdej.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gbgsgwdrk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gaygzymlf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gqhaqlhel.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gpezvbvnz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gxniguvpj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gmwnpyiis.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gwrctgqgb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxiiikjxq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gmhkaozqv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyjyokrda.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gsbxzkrmd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gvyvdhkrm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gkiekrtid.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gabkmqyay.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gnjujnawd.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gwigukqwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gfiaxqbzw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gulzfstsy.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gzuimjrrm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gejjjzlhp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gqcpkgqmr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gbxivmlju.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gufyxkwxw.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gcvtkjvlv.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gxqddtfrn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gmmpxpusr.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gosjtpbaz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gmkddfyio.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gozxsrmtc.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gqvctwquv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzadjchos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gyuoyexlc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gozxzcxgj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gszapseti.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gajkdazbz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/goxfelnqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gyqwrhbmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/guuylovrk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gwjvtnjwe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/geeiatase.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gdmxfhhwb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gmhxwxibx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gfiukmbss.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gpqhkwdev.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gbkwkrttv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/ggmnzvjtb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gblctybdm.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gqnnecsto.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gtwecmden.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/guwlfmcet.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gyhogqkuu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gumombrbb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gjerliqds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gpvzdppdv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/ggflicwwj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gflkchpsh.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gljtluoiv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ghrcgdhvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/givjdlown.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gtbajwfcv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/garovutlj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gcbydcnth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gixzlvkgy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/geaoeuzsg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcjoshbox.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxxbhgnei.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gogzasikd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gfikoaoxh.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gnyexlomn.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/godlloofj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gxuyugore.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gognleirz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gyydrvqjr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gjdqynxct.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gcpckhkuq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/grdfasknk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gwlxnkbgo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxhszhwhq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gbrhcbwza.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gtxkyoeeq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gmtfmapuz.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gxwvhuoum.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/grjeevaxk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gaahrarps.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gbexytlrt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/ggzdhhcpc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gpwurxhec.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gypwhjyjt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/galyqarjk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gpmbxjcxg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gdfiqflao.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gkzmmaktq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpmtxrsdx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gvmavdppx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdbtqtypq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gqknpyovz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gcwtdlmqy.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gcsuxjtao.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyzqyndk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gbldgacmt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gavlxdwop.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gosfvixze.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gewsdoqtp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gobkqynbp.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gqsunccoh.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gilasbcic.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gkoliktxq.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gtmepjnwd.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glkjaqxys.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjyyvoxxo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzyhvszzs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gtuujijjb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gakfuzubj.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/glmhkbpud.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gladephup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gykdnluge.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/glxauuakw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/geraaswrf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/ggfcufbnc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gurjysrnm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gzrglhesq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gltnqytdi.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gdylkgqmz.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gruwmzsdm.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/ggpsvwkad.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gndopxrvv.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/guqypbhdg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/ghnvyesnj.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gplypshjm.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gayftuaba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gtvbarbme.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ghtuzrdnv.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpoklkytp.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gimtakcry.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvtbvoyye.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnoannogq.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/glsmcgcbi.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcakryeym.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gaxtsaxae.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gbuizfnzu.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gpfuhvaqs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gstzfusoa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gpwxnrpcp.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwwdyxksl.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gqoghhqnw.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gxeloshog.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gfeuzddow.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gkdwzbjrc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gfqngwjgv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gfvigojiq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gytoddzmj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gmljpnpco.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gybzvweea.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdtuujaqj.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gikelswnb.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gudzhsytr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/glbeqhyei.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gjvdrnfby.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gogrtrxys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gtohdhbqd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gfngnykqu.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gughadiwa.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ghzrgfark.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gmzcqkdat.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gzfcpxqvq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gtuunepxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gdjvfiewg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmerqafvs.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gothmarwq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grxwfhege.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gptnhvodr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gelrhnlyy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvontqhrq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gozedqhor.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gpoqyrlvt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glwgktcsk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjqrlcxqe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gmpniwgjr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvqnpqevk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gniyxakpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gmlexuvaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gzxytglwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gyccdgaez.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqqqhpsnu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gduonghhd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghmikzlng.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gocwzcgvh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gxvpvvuiz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/guykkavru.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gyucvkxvj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gztopnjxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grpqjlbzc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjvjmbbwx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gicumkogw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gptjuqdqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gqfkqjmdb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gzctbxbgz.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gvssmahfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ggdosvedv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gghpdwjdp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grglwmytt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/giqpqlzxg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gbgxthtji.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gbxgqogad.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gozovoisn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gddrsbnlz.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gqoiyfdff.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gzamuslbi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gtsyhghik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/garyzxoag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gluilbjkk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/grpgdtrja.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gommphmed.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gnzxrbggs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkedhboa.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ghpjexvsc.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gzlntcrhy.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gitumvccr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/guprleaud.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grirwagwn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gscleyfzb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gfocluabk.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gumatdvrc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/grbouatqd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gcxvmxyfe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gfujsqgoh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gxmviqjkc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/ghohbghyx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/goueusjwz.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjdfalcuz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gdnyovbhf.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gmncjqpct.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gaixxqlsu.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/goydimhba.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gofrfpftm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/goxisnyab.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gscfontdr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjymlqnuy.sHtML


<!-- 参考信息 -->