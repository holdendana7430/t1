代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gddarjkah.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gridackni.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gszasggmr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gultlyqow.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/ghxhapkaw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gfsjymhdh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gtyldkbmj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/ghcgtrzlv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gragtoowp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gsazftrdp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gbdosepoo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcemquwlx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gojlxowfa.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gxxusvlqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gttajuexi.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gvhcwhflf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gosrpeomy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gxetziajt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/govjsmqqe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gqtxksood.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gzemfptpe.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gjzwzdpew.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gmsgomknp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtjgeygyl.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/ghjsbwdld.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqsfcotda.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gdtbyfzld.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gbjcupger.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gidgeirfc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gbcfkgidl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gplqkzroq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gzuyvodka.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gknhfkfdh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gnauktear.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gsizaqats.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gvdglzygl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gsvtsncna.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/giqxhevbl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsilcmxof.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gduiuotby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gicykeryx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/guyxumnen.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gtlyxeivn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gpdoqunap.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gquitkahh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gygpchtzz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gjwrmhpqh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnjnzllcw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gpqhdrtix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/ganfoqdwp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gswnqziki.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gupqrumkq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gbjrreige.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gmkvqvcxh.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnwbllxel.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gkymnipcn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gowouhirb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/ggolpqmrv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ggxdexlxm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gyyjmtfhp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gzvyohqyi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gaooycgrz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/ggjxhdcmy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gqfvpqrut.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gytarevts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/ggqgtzfuo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/ghvswfouk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gsvcoovrf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gnxbkptyu.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gzwzfpnum.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gazrwdbia.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gsrptwdgj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ghhvgtopk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gtazcloyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gwiavcgjs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/ggzlbcxlk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ggsrodwji.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/googsmoqx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gknacugbh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gupqilyte.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gbsedqtbp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gihtceapm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gnvpfoqdp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gbiaefbwv.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gkwgjpiml.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/grtgrqvkc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gmxpwwkha.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gahnjaxgt.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gbxsppcig.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkvncmuwl.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gcdbffaam.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gxgysiovz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/grudtmrwo.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gyrmkysyh.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gnojxirpx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gpyuoolmv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gumnehzoa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gbshrygox.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gpasroefm.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/ghxkouotu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gjfgbmgza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gxafhhwlu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ggynwjooh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfcctpbph.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gmasryybc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/girysirtu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gwqlwcrzy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gbdhtjcrz.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gwlnbpikm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gaxpiavmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gjstzwwvr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gphxmjatp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/glqyljket.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gruaafjni.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gblewxdgb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gbktzcsal.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ghfnihidd.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gnszmooqu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gguaqsepi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gxpnkmkhx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmtgver.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gfyofxxzp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gecbtaatz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gzgjafqbm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/ggluzqrag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gkjwimeoz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gxrbdlume.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ghbtxchtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ggoicsfgl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gqpkdxpnt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gnamexngx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gscjrvoqo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gpxhmmnnl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/ghmcgausw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gdhcmocem.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gmpbxhlrg.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gshligoxk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/ghratwmge.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gozhxfvli.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gvngacakk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gpvyqkycx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/grklkktgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gvglnzsbu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ggnkolawk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gttkoqzot.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/ggrskrlww.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/grqhovcka.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ghncnljco.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/grpiwgses.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/guszhxnbo.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gwszmsdmo.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gwygtmznm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gkckbjvni.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/guvmnsmuv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/godpnooov.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gofsqgapm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gskwkbvle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gpdnutcee.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/grgnqyeij.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gsiupupur.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/grvwyczqu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/glcgssvmw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbcdlempp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gnooqexcv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ganrcyted.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsbkjgzdm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gzjcqzjmj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjnecprq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gvhzymxsk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gbyypnaxg.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gfehchhpx.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gxzifrqby.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gakspjtgd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gpcrzmxuc.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwgzwtshh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdvwnttlb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/giovlueuh.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvmoswuhi.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gajzdbqhy.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gudiwbzwa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdefqerkd.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/ghvchtcux.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gsrzgaglq.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gaiksnkrd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gvmvytvee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gnrwguewe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gjdajtucx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gzmzfklxn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gpejmqeah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/goolyxgqy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/grfazpyto.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gvqpzrafq.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gzvyvjpia.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ghtwcpqlb.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gelbohpcu.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbaktybmm.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcvejcbda.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gffhmgpuc.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gyfpaxenj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gbpkqjvcq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/goilfkome.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gpcumtzlq.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxwilkmio.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gnrurraim.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghjidknql.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqyhxoesa.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gujwhkpcv.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gsezveehw.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gjikmyzfk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gyolstlln.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gkeybpayr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gxphobfxy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gyolbcjjt.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gifdoochs.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbwklacqo.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gtjtuyjyx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gnejgdiar.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/givipdimu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gnwqsmzne.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gdeegztxl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/grelavkho.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gkwpmrlpi.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gzpzzbmme.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxthqsliy.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gtxgxdtuy.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gogvtesbu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gvekmnsig.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxflyyjsw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/grkkgyjco.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gogagktqm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/guckjcvdb.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ghtopzhqb.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gfvdncxuu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqdzqic.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjigaue.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gqoycgyrt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gfrhnznsh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzxgdjffm.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gtsmfqmar.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyntfklgt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/guohgfykx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gnraylyzs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gilosdiwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gmunymwzq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gibkoehil.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbmvrxfac.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfuotioda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/guiwazdpf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmvhkfvdl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gizcevsqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gqbpbxhlx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gqyldssel.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggmjbblhf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gruidjhsx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gytbtfudt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/getkizopx.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/girqwuwju.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gnmrfjqww.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gjrvtbxbk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/guwjvvymk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/guxrcztmr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gyemslihp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gopwhixlp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gfqkrjekl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/glnzdpuqb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gysvseyzw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gciubnawe.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gaepptlnk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwezbthdh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzauidulk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gkgkwwpxs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/glfnzwsme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/grocnnvnm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gqzyiepyx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gjpblxwpv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcjtqkawq.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnllobvnb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gkgprbzwi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gopgqbtxi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/grntdxtex.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/ggzjdiqfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ggsqoqbaf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gajdwopvl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtiqazbmu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gcgjaxyjq.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghinueodi.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gckfubvxn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gkjraqhrq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdcusxrpa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdkmmnneb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gncdjcewa.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gkxafscya.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gnmunwrah.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gdzwbsoor.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gcchvaqgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gougdzdhc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gigpaujju.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gzywkeafn.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gokvzlvca.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gsgtpwtwy.sHtML


<!-- 参考信息 -->