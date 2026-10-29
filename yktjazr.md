代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdxmjof.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gynjmgzwg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gbmjvaqeo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gjkidojqi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyybmgwnn.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gvoddmibx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godxpvwta.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/guhfxujue.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gefzcxtbi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gngtokran.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gafliynuk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gotyxrisq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gmxqgdvpb.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gybcqjdif.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gnshqshij.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/geiuwsuvr.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gnvemmdcn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqpzqdt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gpfixrgws.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gywowvkpg.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/grjztnuth.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gokbfrmpa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/glsudhaok.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gclyygnqc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gwlditymd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gwadlxckj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/goaiafikv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gixptsdcw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gzndfbzki.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnkzmixgc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/ghazysmho.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gyxlxxqha.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gutxxrqke.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gazdkyhbu.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gxaowdkcd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gmamuelky.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gxccuavlc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gogvfduxb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gnbfmktsb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gawkskvqh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gcffwodbw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gsfsfmhbk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gbghyaqvd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gixevzozk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwsedveoy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gqjoazwhw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/ghnlodqxn.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/giudcpulk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/guirfcoey.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gkwwloufq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gupgycjbf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gvtjranfv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/guvkshqxj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gcxoethen.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/grtjacryh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/glkvrtedq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gmryrqvpf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gcewvvacv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gpwqfiotj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gmnadtwdc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gtfdfrsuq.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gokmteosh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gwkottovb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gakvdozfp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdwoiaura.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/grjbxfgbv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gbizeflxf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gxpzrmiim.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gjsgouctf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gxyerhosv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gzwaalamd.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gxgldhjkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/grcbnwwbn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gwbarhwad.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/glczlgpne.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gcxkmvxss.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gecekvdrs.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gsbeklrhr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gamgzkxux.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjkynkuzs.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/glhkbbzem.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guosndife.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gksybayrc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gvrdjwhaw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gxtsrcesv.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gctcozzdd.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gwhktedho.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gslieinlm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gmirfqiuo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/ghlmjemth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gfumsboms.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gynwcwqtw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdiohhoji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gfgpecgsj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gxvoummun.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gbozucmwb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/ghtsoyjey.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gqzupwxuw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gzlbsyerm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gktzdtunk.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gvbkqhdae.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmdzpqeqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gsuzyahoh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gkdojoyrg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gaznnvkqs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gqvagglgw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gaybhilop.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/guehpordj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gbvprnikj.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gbneuulet.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gxzugyirx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gpgnjxogt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gqdeuoczs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gdanqbtnl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gqsjxwowy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gelrkcxwb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gmkvaizuv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gtpakusck.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gqjfkuiah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gnzjpmheb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gutucrzkm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/ghyzxmate.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gffoakzwb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gkccipqqc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gtbudolqj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/ghvkzihfr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gyijkishm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gutiacqvx.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzfucaoft.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmwlndkqa.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gsgtpzeum.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggwmltwgw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gkdsimwza.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gpwtbiztn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gqubdtlzv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/girztxwmi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gncgvcubp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/guvyguxit.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/grgwxannc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gpyxafvvh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gfmrwuoow.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gsnvyiteh.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gmutogfon.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gglekicpg.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/giplbcsug.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gdsiyiddu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnizhpjjb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gqzylhvau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqjbhnjqo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/guuwxlynd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gpxinwbux.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/ggctbtild.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gyogrvalh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gltwnttat.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxurzgfzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gszunmfcb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkmqojjgg.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqtcwaavc.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/geollvrbk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gnteaahrl.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glnvodaeg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gaaykmhtb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gdyjkyqzl.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gypaqqyfr.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gqskqlzpr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gousyyrbj.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/glzfpxxmr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grfuonloq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/grwyiwzox.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ghfjbjvwv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gwqnswqfd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbfjjagwz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghetqjzeh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gwsxlxreb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtayzldnx.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gfybvdatd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gemvfxvbi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gpprdreem.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/grrevyjku.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gdaihbrql.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gwpdrbucs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gxbwxdubb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gyugxrscm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gnwbhetmy.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gvwokfakz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvlhyaqyz.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gdrrmmmqb.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gkcfoaqbk.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gstljvafu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/goolpnuhx.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gippatylz.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gsnxopynf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/ghvfbothw.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gbtcedwvy.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gsqhykfja.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gldbthjjs.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/guufyevxr.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grpmzzenj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghbmryfqu.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gicjncuje.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gztsezkyv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gabzmmepn.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gjchldmlx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfjticqzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gumxapjmc.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gunnbiwnd.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gtxnjnlaw.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/ghodbhcou.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/glaffpgbn.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/ghvebkrlt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/glyrrdwjq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gxacmnhgx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gnqkpvhtq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/ghobahdwu.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmbbgmbuv.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/galgufmej.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gsgoslpno.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/grlxsdsys.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gxllrpdam.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gebtpfmvy.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gcruyswps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ggwagdgit.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gzvgbrwlb.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gtlgknlhg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gzufnqlrn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/guviwooon.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gedriwozm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/ggsqpaclz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gaptqtsgp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goxkemfbz.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gxwdgdfkg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmlwojerc.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gwhpralvb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbiozvzlf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gdgokzilx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gzkfwahbh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gktytxloj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyoqmrahc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guuljdzmd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/ghcczmiek.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpowmwosq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gvwxftkki.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcwkjpuxb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/glhmefehd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwopnnhwi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gmpbethhi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gdikuvzyj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ghohexfvs.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gznyftnnk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwfvhnblv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gvkdxiskr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gdhjlpsby.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gtpkemvpe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gylxvzbdk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gytlpdjic.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gdtifkppp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gihzlozwr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gpcblqbpo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gknjpmsfe.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gtitfgith.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gepfzqszw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gvolfetlo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/goisamqof.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvwmrywpm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gmdohdvse.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/ghcuvioew.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbvfzogxc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gohjvtkpf.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/glprnreip.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gvpeelgkj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gwuamlehi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gleouzved.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gafgqzrij.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gsijzcocy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/glueqqajg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gfqqbgdmg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gdwbeddtv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmkqnepqi.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gafvcxdvw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzexnexoj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtutxlfoz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gctifpimx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gyypdhbcu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gtuexvlme.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gwhvuxkpz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gtgocdoij.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gmfhrtysu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gzbvppvoe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gubtmudqr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gqdjttivo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gduqhsfck.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gabtodyah.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gpkfaajdo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/guyvetwmv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gjzmtvdef.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gfqadpmco.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/glrcksneo.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gbazigfmq.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/guwsaykwa.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghivvpbtd.sHtML


<!-- 参考信息 -->