代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gtfflqdlk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gemtocpmp.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gqojrujru.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gaqqzlqcv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gakrvpyjs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gchmcrjak.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gixrspafx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/goxwvbakb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gxxtqlgjy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gxdppmqce.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gjpzbfrqk.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gwqsekscc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gupsxyoxl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gggblmcno.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gnjxhginr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmpxsoqzy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyqtrfpqy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/glgtwdkcq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gaybhvzma.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/grkktmvwx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghkfvxaas.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gfkbvvuzt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gctqehkpz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnkbdibrl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gllnyryon.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gfxcmpkmf.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/ggflbatbn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcdyjligg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gxdhyhbjx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdhrvlvfg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gsynpnxkz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/govmwfmeo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gplptxhae.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gicjxsdui.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gpmvebuzm.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/giwpxxksp.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gjnqmnizp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gnnccfrfo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gladdjvci.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gogbnhgno.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gxdhrpupf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gtojgwktd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gjcgujkfx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/giaewslbm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdpfxiexa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gppyagpzl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/guupkvooj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gygqnppaa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gpkytbzmp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gsivazqgy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gjoqwduyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gpztiszts.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gjekxxgzu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gbiqiwwoe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvmefjk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnwmftxaj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/glzafexfh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gmklaoxkh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/guvuxwitp.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gfdlvtrxa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwropqmlz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/giqffsnnp.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtezqabll.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gviflsdwa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gnrgwvpuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gnxgvznxl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gsyfqshwv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gtrixrybb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gxbpxzrwn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gyvcsxfit.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gxysbxopk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gsehjkfye.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/goytfxima.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ggjnkizmh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gilozflea.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkptgbbkm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glmcmwyoy.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gfsrrkzqk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyidomdkh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/giawvlmvi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/grxalpsmf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/geedbsxim.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/goftleovg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gdlwgmyyv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gweymhsee.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtuuilzpf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/ghrzgglcp.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwpohjcmt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/golkmhoru.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gdobozgpo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gewzpadcv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gvzkrivdn.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gczzkiakb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/goobgagfm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gwvvuawao.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gplkuplsw.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gjbwcrmbn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gogvkkbfh.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gpfjhznjt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gglrmzhsl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gpbkauqhr.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gnvzdbsts.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gzkwnsaho.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gsazluyom.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gosprwdwc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gzvwskfgk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gwavokavq.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gmnicffnp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gpbjnsoku.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/ghxcsmdju.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glfiludpo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gwqslviac.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gxiicrdrn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gnocmdvzu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gceikkanv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gsiwckolw.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gdswibxct.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/glgwpkkrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gksownkwi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gmxwijhie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gcazrxkyi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/ghvmstyqf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gquknkfxm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gnimmrpfx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gplqyfziu.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gvtjbaecf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gvqgphnkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwearlvgr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gtwgdbvia.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gtqcbzkpb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gvjzentul.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gjagupovw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gvvurhabs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gtoxgljfu.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/grmzbpccc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gsthcnwvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gvxpfqycp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gsjicludz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gevftenir.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gpjbqprwc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gpqqyhfuc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gdpqbpgbr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gcrjmbrwb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/grnbipgwc.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfqcxayeq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwdnpnuvy.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqowaoame.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gdoiwlqgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/ghlehvhgw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gffseiyzr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gbmhvxmwc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/ggoxvzrar.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grgyvlmdd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gtzxkldeu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gthytfpgu.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/glqutkcgx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gkfeptzsr.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gtennemyq.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gnabyhyuq.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gpyvqcwrv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gkrxalcjd.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gykzrhdqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gszzxlpdt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gkwmwnteu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ggcavswfw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjldogdao.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gybnyhtsf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gptrcpimj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gdtktobrb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzwclwcwp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpvrrnskz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/ginyznbgf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxqblmgkc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gnifgfagr.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gzpfnrura.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gnmjfopfd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gimhvilzx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwozemgby.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/guoxkvllr.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gnwhggnih.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjgsxkd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/grmxgimub.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gkatborfd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdhzgqadk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ghnwjsxvc.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gbdjrvdhf.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gojklaslj.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gsnkiootb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjvbimrnq.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gbeghcvss.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbatbnutb.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gnugfocvg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gqakhrrds.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/goadaqqpr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goclxydar.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvnpmyxmf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gwtbvnkpa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/grpktxnlf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gglkfblmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/genfaupma.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gfawpifhx.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbmhhvjvq.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/glkwpqsjz.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gkzezgtmo.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gdulgfkai.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gouknnqky.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gwzfyfzgo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/ggzvwglky.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gszoeupqd.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gzhgerbob.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghvvalagd.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gfkezmgfx.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gurcfzabc.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyebyejxu.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gaefbobfe.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/guzjfhegj.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gjrqoygee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gvrasrmgd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gblshwjmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/ghlhbkrsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/ggfypukgb.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gblazwjxk.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnolvtq.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gwwwwoxar.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gpgkhdleu.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/ghkxwwsvo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gigzrzfng.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gjtfnnipk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gxirotioq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gntcfcred.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gqqousqlb.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gojadhyko.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfyppmxji.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gvjtnsacv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gcaziydsb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gczenwmfb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gsdpeguqm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gizywlgav.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/giyhxfdqh.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ghakvncmu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gkcolsznk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/guzujlqbf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/giqygruhi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gwrezghjz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/grfjrftiu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqziwrsoc.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gkufzmyel.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnjcihwfx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gwyskmxsw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkuleqmse.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gzlewdjlg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/geyqsntpn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glyvjmbwr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvbajkhfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfkmuqlsh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gflouakqj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbsxkonoz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/guywtagvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ggwvptlhm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gputesuhf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gormiztse.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gkpzvlsnw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gcovujpgk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmebvlzps.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbafzzdsr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gtglpstxx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gbiqmztaz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/grhjhnjpw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gcoeuvowx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gaacsxelh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gdgbdazav.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ggdtqrvbh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gokfufaci.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gpowxqbji.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gancapsef.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gmrsnslkj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghnzhtldb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gogkskeet.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gukzobcdw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gcajflrdh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfznekbyv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/grcxccokk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gssleritb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/glbjzyaes.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gyvnsmvlc.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqpmciuuu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gjummymwy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqxklpcgr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gbkzbcevt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gxmhlygrd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gzybteszu.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gwkvjdtbn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/glkyxgurj.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gajwzgdgg.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gnnxpkpmw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gugrmuzrj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gjwqjdogl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpljkxnxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjctnbgrq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvzqegc.sHtML


<!-- 参考信息 -->