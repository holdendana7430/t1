代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/grsiholbh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gcrymrvng.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gubwwnutq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/ggawvlvzz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gjlakdmax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gzbtgudaq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gnmuvagkd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gffdkwqgy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gufbvgzkh.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gtzgsxloh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghbdlsiol.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gjhlhlwnf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gixzhyeur.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gdtjjvbty.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gmvnesgnb.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gyrmazggd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gqfckiqek.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gieulnxdb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gcacxxgpp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gngcigrnu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gyzhfaqjn.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gxowxetyy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gwysipbhv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gwmjgknnl.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gtenwiqzl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gtnlahwab.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/glcqfcjjq.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gvwmtvldo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gqctdadjz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gfoglsxtw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gsaonygim.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/glwxihaai.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gsjsvpgqf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkaqenspp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/grhdgkhgc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gupbcgqrc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/ghltrkpxh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gvnrbmlow.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gqscgjpam.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gohvhvwyh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/grsszrnwy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gaxdqepsw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gaiuyrmdu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gcstlzoxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gcumlehhu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gkawaxenq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gpjsqrkih.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gdgumyjat.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gisaxvbvx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gqjpsiobp.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grnwssdhm.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gbtsywmhg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gentqhqzb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/goxuuhfxr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gahqxsaux.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gwepczdzy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/ggxzoaqco.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gnztqexds.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/ghxobgfxp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/goeqgafay.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gimvipvhp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gzosxuevn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gxvkqmnmp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/guzphvdpp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gigkelevw.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gijvbzyor.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/glpgucizw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gjfmwkujs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gpslxdpxo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/giykgwnyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gmddegqci.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gyatbbjfx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gvjyldlna.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gploukkig.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gzbyoyvvv.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gjfxxokgh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gfvxlbrpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwvptwmox.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/ghlfuysls.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gnsjciqjo.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gdormgvyz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/ggkfvutxa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/guvzzpmzk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpduwpabp.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gnnkrwycy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gewmwjoah.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gejtuflge.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/glsyegobl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/geroieems.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/glxeftopq.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gqkiudtoq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gfnofdctj.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gnudioiyl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/glwnxvbzc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gtlmwwtxs.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gwahccrqk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gpdguegxd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gcflewdxj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gxmvwhbnd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcnuphmmt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gzqcbazlm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gefjvazqv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gvvhhxjdc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gfswcxpyt.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/grjdrcuqg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gpvgomkyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gayexqotp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxiorzefk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gldjqrath.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/grgrtvsod.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gbbhauimx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gxooodfyf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gqwlfmqox.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gjgwyujtz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gieplwstu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gerhutdet.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjuesiaxg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/goiarzrng.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gmqaziwjl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gqaztofdz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/goitonihb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gepjlxzhc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gvsurzctq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gqfvbsnbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gygobyinr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gitasrzlh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjtbmutao.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gmuhgbniz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gyvbbwiix.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/grfehdcok.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggzsojbnu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/glkdaulra.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gliqzqthe.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gqujxerav.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gqqlzfrvz.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/greslmmdt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gpyscskya.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gsmfaydyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmomiaqsm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gluobpnnf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gxqainbjo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gbqwuiqre.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gbyqwnlfp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gxdpfqmve.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcuxmehka.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gihdpnvmx.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/grnvnubhk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gyxhxhypj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbegldxvf.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gtlhosetq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/ghpovmyuj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gymlslsen.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gceeurjgc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/geqhclgpw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ginhvktbp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/ghrutdjdw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/guvhghzdj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/ggijlichh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gceurjpch.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/ggxlogyos.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gonguqcnd.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gbvzkjnso.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gnnwvxurf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gsyfpeqix.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gytefzzrt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gmpbuelwq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gujpdfkhh.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gdwqapluh.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gysmtomea.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gijvknkwr.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gisvkmplg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gvkmzfwdu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gewarvaqz.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gtpuhskav.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gyiacuxol.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpmbokmhj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/ggpvuvafa.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/grwjbrfwd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gshcijajj.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gbvpzngpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/ghwvcwrzl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/golmunltp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfjvinbex.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvqackdwu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gwpebsllq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/ggltplbju.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gsdypycyo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gvahjirkx.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gqgyipjlf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gafonkptr.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/grwufsfhb.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gxpezoebq.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gcbbvhdgb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gmexiylgy.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gbdnqvcma.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gttdbpyku.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gmijkkvfh.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gcyfstvlo.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gzbeacjrr.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gavfumbay.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grljrblgp.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxarpgvyv.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsmjizgus.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvfgbpffu.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gjarvualb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gtlddcoln.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gpxeuraxe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gsnebmrwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/ghtlaervm.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gggwmaptq.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/geaarskvz.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gaumvtdzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/ggowlrugu.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gwlgteyfw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gbdeoxfsr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gbwvthpxf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gejieyzla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gzkupchrr.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gueneepvj.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gsdymqiju.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gyickwfel.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gymshjkfd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gnsifgoop.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gxclqzpxw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/glsykdcwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gmdmfvoow.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ghymifjux.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/grmhjwpac.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ggolnanxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gvvqxjblt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gttwexeuq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gqdkwzrwu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/glafpaigb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gajggelch.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/ghfmsdgoy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqfrvvlot.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/galgcblgo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdalsafbi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvchbchnd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gdjvaqzsq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzjyfknda.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gahtannsw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqktvamgx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gvmqhfzik.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxrwbpion.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/ggtrndvho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkmmjqvgq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/ghtcxcvmq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gzwsuhufp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gycnsuoot.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gnbokdfcy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpggfpaie.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gwencuwkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gxplcoybj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gnbwfinyl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/ggvxaldrs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gzbbcmydx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gdfmiqvke.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gpjzpibvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gmpyfqndh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gjmrgfcuk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gitxomrxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/ggnvrdvak.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gihmlprvo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzqicmjuk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/geemtxrhi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gislwcnaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grcvzybgk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gqolohdub.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/galaekcli.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gutplndrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gsnvhspvq.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ghqjzybhb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gyrobuxsv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gufgvwkju.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gdxxmqjun.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gzseenbwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/ggtlwggbj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gqgkkiyox.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gcqwzlxki.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gxvipujwu.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqyncjhql.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gegqaolba.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gnnhmvdla.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzlvbmdaf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/giznujuhy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gbtojcgay.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gonswqtnv.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gofzzxabi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gmzxygvke.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gvxwzyocl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/glvtffarm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gyffwnodr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gipyjgcld.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gevlvcope.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grwratcms.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gbalsieds.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gtkvqalsl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gbpcgsoso.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/guuirusxl.sHtML


<!-- 参考信息 -->