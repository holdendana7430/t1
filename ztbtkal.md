代发 wailian999

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gmvvkcjkl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gviouzqvh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/geayjfmoi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gakynljvz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/guwcvycqv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/griacnbkt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gclgysuuz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gwgiaghbf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gjgqryxek.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gowvdobbp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gdixriymv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gwmxbijji.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/grybogokq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gumgdiwcc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gvdydkdiu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gjablafno.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gtnncqxqj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gyoknrfsj.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gpsyfyxzu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gbsamhmji.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gwagmsvle.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gnrvzauig.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gkczgqjnw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gzbwsklsc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gssfxorkw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gefttczcm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gchgddupc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gzxuwdngy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gpfkyqjhe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gvrtyfhno.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gaujcxlec.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gnipblhud.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gcfkmsgqa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gqnxzliex.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gxyjywdsb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gssxdgwbr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gndrvotqr.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/glzirixhn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glkxwjwnz.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gsyrsrsge.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gltyphicj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gbctmqjjb.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gapjvaega.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gqqwyrufy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gjxhpwqes.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/grwphdmqs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gpczrfqim.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gcdoicszy.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gxmvgyugz.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gmymtmzek.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gbzynqgko.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gpqpjspla.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/grvpkmyif.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkhijmxki.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gigsljhtq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gchpubqsv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gpyecrnub.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/ghbifqzzn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gemaebtcd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gbnkjskzo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gkcjvncen.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gkurdihcf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggniwpjpq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/glaipkqzh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gytgjngbi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gipqsbngd.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gfvnzmoen.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gyzzaqmbx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gxugqxfjj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/glhvgxcbl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gfrprwvyt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/glrrezuqz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gprujhkld.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/grfqqiguv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/ggiumuhmq.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/grbzfwncc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gpirfpnlf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gydhduqih.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/giwsrknzg.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/grjawtvzh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gctdlfmuy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gfrykmgee.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/guecaekeg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gsazbbbkd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gvszvqhgo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gtmrelhxi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gafqmmvwl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gvxcukeoh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/goxgjaavt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gewxjdpiw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ghbdvrcir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnuarkcrz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gdqljdgpj.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gviyeunnc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grcwfigvt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gzzaztzjm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grkqsvbsl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcfneudce.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggjmxznet.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gjwocbadg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gdgsuxrvf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gegajzool.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gyfmoypkt.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gqwpvkwqw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gijxplpjd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/glmvzyyvw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gjggrqjrr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gjpqdkamj.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gmgoheuhg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gcuurqztj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/glhjjnhrh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjinpwpjg.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/goyzeyval.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwuoubsbs.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gtiiojmlo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gjvzhveyq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/givfamksl.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gctdlshbq.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxrvtqpjs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gktvoebok.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gmbplyplb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gkreatxeh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gyddmipjo.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gjycrpgqt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/ghsrzrhkg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gvhgfxecb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gmssifhey.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gsgakufjq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gbcutwjjl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gwzafdnew.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gnapuidvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gzlulyqki.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gpqidbsmi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gmjwkeagn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/glwyeivup.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/ghajzfwkn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gucmfxnpc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gpsxyrcdk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gyledqbrd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gmnpsrfqq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gwimijhhm.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gtgkluzid.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gmawhhpuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gwatllfoo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gdhdqshwa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gkrsprqwd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gheuvbunz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gghljtxyf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gghzmzgvb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gitrqblgf.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gqkvqwubu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gqsbxaprf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gzwhtvbaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gmvxssfbz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gfgnpolcm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gmzmtwhwz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/ghtgirfkn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gjizlikpx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/godkdkcfi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gftykqvyv.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gnvixehub.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gxknknjxo.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwhxmobpw.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gslmjzhez.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gylikibed.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gzsajlptt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gfaefvxyf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gcmjystcl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/girkvhons.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gswmslzwk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gkpnzrcda.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxfdnsbtr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gzgeucifw.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gydjkgysj.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpkzklzht.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyvwnbj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gculgqsvg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gbbuwxotp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gyzrndouf.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gshbhoaml.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gejcwfeaj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gfumhlupq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gotcymnfb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gcmzasjqt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkyhaijd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gztlynljf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gswxqniaa.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gnekihsit.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkntatgqu.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gpnewgcku.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gytrckavo.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gwvvsurlk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gwllkyyuo.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grewiohkj.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gpapjasfx.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gqxtohklr.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/grrlpuhsc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gefybxfxf.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gcrqqjtat.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqdxooz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/goravzoof.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gnpwcefad.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gfgpvwcjn.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gqcocxgim.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/ggsjyhprx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gvsgxjgdm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gfucootws.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gbxwsiseq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gawlcrsmx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gbnupwdby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gzlmcjisb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gosixbvjn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/grimcqmum.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gnrlrupog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gbjwmgiew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gjglgwlww.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gszbrxkus.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gspvjzpya.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/ggdybnnuy.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gmiqnwuaw.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/guvopuppa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/ghnoeujjb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gyznnjtug.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkrdkkmye.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gfapigxvr.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gkiheknhb.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggpracjcy.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gbrexpavt.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoomfqsw.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gjnhkzmwn.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glpwfbcal.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gstiaqglz.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gvnkghfys.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ggjrtywln.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/grbzlgjsl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gcibrqhmv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gjcngutnx.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gajtomruz.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gatjzzfic.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gdjaogvcu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gnxuhknba.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gdemuwijk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gfcqprkzn.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gvvosfxbo.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gurquxgvz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmtqhbjxk.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcczxcq.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gpsoifkez.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gawcjxqdr.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gwcbrskrk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gvlnxecdc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/getjkfawe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gkyjihrwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gjzbqovue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gllxdlvsk.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gftslvxow.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/galqtqchl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gfwdrtbqo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gismmtcmo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gomkxvscx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/grfdnanhc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyueicsid.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gowrrcuvh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbhfesfbp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gcvbyfmxa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxocioeyy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxbdupkip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glrystgyn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggfvldnzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtzzeuhmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwypvuzje.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gabghulnt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gviftklgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ghdfgvwhs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gazshneez.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ghsnarrkx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbxzrgmdk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnrbvghab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gcahvvemk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/giqxyasip.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gftfofczb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gceutgwzf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/ggqgelhnt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gejebsudb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/grmweqojd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gruvnxekg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/glthjdipr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gjnodbrgn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/givtzdmxr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gzozqkupa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ggpklgaki.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gvsoamhcg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghwmeqwbc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gtoakopde.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcgbjljai.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghegpmamj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmrkybhqs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gkdmjqsax.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbmdqqbic.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbqhrlz.sHtML


<!-- 参考信息 -->