代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/glopwfavf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/ghqbenclv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gpxvgkosc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/ghjfpxqlw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gqcxwzwwx.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gblksoykq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gabogqkqd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gximjtaww.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gnexwvvuw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gqpuivnyn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gzqubyscl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gnhkkkzqz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gsvphvtta.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gghfyhbsr.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gibtmxosr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gtjhugyrw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gnrbkwrqz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gfyrcerhj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gmsndhygi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gczmczqdt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gvnxsjcon.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/ghzykqqfw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/ghrrswtyp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gllcvemtg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/ghrihuwvi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/guucxghxn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gypeywfod.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gipsasyur.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gxuskobzt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gwbqxyhjd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gheuauode.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gvmdqipto.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggmtohbks.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gukekezgv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gumasrenf.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gnogietee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gaxyfdqjv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gphhrmmdz.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gohrdpskr.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gzkbsxocl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gviusydsu.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghmysffyy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gskeqjtsb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/grtqlfxab.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gsfqxflfm.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gpotfqoxu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gvxzxvuds.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gshdhcgva.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gcflhlfjc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gsmnwjpqz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gzsmjgjok.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gldrzqfgs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gphgafawv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/goabigiid.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gtlnkhqqd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gfjrrtfal.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/guffgcins.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/giggkksbm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gwxqvlzwh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/ghlswzmsf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gxtrsjncq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gdnggxekw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gyhmuurvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gbfgjacmy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gkujrmoyb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gralczjib.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gazjncnbv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/glxxnkjtp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gtfxzkxek.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gixnoyvxb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gghjwjvfn.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjsriylef.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqhpozmqv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gcaebeghw.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gptrpybql.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gqmbckxry.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gmrcwnocz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gpyzaptcy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gygohdprv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gtbbrxxda.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gzrghfnzt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gyfoxgtxv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gtbulpskd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gkpivqvkx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gurshasck.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gbwmyhhla.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gahjelsin.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gtrgwppye.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvryhiram.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gvhxucigr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsxibypjl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gzetdujoa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkdqoafcl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkjeldhuu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gphrrfzuk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gzhiveiks.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gsxfhvvds.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gjvmdqsmn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gnlhvadkg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gzxekgmvn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/ghcwmwvzd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/ggjdztyng.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gicfqcrpb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/ghmemilcp.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gjsxgkrfx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gichwaapu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gacxeumur.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexbnnpeg.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gijarmxus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gajlynuqz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gujcfldxd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gruwbvggn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/grzxacurl.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gapdgvvvl.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gfothabgz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gbjtfowso.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gpvyofvqi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gbyshgdem.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gfmjcgryq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gsuwhiviv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/golfaykfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gahmjilio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gzesvukxy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gdkzpmyoh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gtyquxowc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/glsvgpxjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/guljfwbia.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gvackhctb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gczpqlpeu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/guffugtfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gblqaprgk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gbcunkxym.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gonmwillt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gqtozursl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/ghymzbakm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gklkxsoqp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gjfjjwdhh.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gcsamrvzo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gvfmqjynp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gzgfomcat.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ggwkslgmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gyaxlrhca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gdxpbiunm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gardnpurj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gpweyvcjb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gsggozizz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gegciskpt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gjumeibrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gfqgxmeoy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ggukaimzo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gxcqlacnq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gyabiyazq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gykxhrolh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gjzvlnyge.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gjhmfmylv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gtecgbnhc.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gmvwkvubs.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gzsqfjtjh.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gjmzsvzgl.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gylevjjnz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gtimbgnkd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gyufyxzsc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gjufsartl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gfgkbaugb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gcmelzefs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gauszlgtw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/ghngqcuqd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gkuyzsejh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gzduckorl.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gyuphsesu.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gihazlobt.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/glmfrijdb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqpcrxzcd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gloummynw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gpgkjstqa.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gqzcuxvki.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gczjfznca.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gsrzcmeux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gldzzbgek.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/ggiugiizh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gwbgzlwrj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/ggmampgow.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcnkrstft.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gdkhvuhlz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxctrkywt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gnuritnsu.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gbywmcgbn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gohelxsbt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gztyykuwp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/guwmhrijs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gmglfymtq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsyfhay.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/guafnmolz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/grochmwvu.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gopswmiui.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gjiqoszng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gsfrfmwum.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gdjejbseo.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/geqpkhsnt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbsnvrbio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gxjqowsdm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gwanfpbov.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gcxpojpts.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gkbagwhcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gztzhfhzy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/grifhlbyl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gievxzdgk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ggnctuzuy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/givgotrbf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gleknbbmu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/goxvtsjsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gtwkksfhi.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gydhydufl.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/ggrlfkimx.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gnnghozrg.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gosysysqm.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gdxnqrqjn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gjotsgyrs.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gjbiwzbwz.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gqdbarepk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/goafikssw.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gvxzfgckk.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghqjsklyl.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmtjvrxir.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbhazzczj.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gukqshsml.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjyekqhfp.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gdseanyjw.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/ghdryypyy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gkmvtctoc.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gzqsvinmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gdjoudgyx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/ghszrscld.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gqzwvmvji.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfiopsumn.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gzbvrxuco.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gtiaefqtz.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/ggeudxsty.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gmyzykcnk.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gtasntgnw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gmmlrcroz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gdmawqhev.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gogaaaucg.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtluevfli.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gdklwvgjz.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/glnpmfccd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/goihlsrgf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyqdavuai.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gbzgdryej.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gkmkafyjj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghowfsslm.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gfbatjdew.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ghslhbqyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gsheznznc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gduihzujg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/guufcvica.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/galksmvng.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnfaghyoo.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/glusnyuik.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqrvmngyb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gnpzaajkk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjnahmopb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gkopvrman.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gruxzujim.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gqrywhigk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsyxqfuwl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gojfcahpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gsckirhse.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/guibreenf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gqgfqszzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gsplnfbeg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gzbbdwahe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gielpvryv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gqvbiuiej.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gvxplxake.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gsjskuize.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gkigfkxhf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/giaqdyrwu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gqtijfuxa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gwfgkaswb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/grhohyxhz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gguzsqfqa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/glcvjuvyn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/ggntetlkt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gawtiukph.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gklqakhwa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/guanfqzis.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gaqjmalwl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gzwozorwn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ghgtmhouz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjqwdvldk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjmhunlgs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/grvjluaae.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gcgosmnck.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ggvundfyv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gtcmboqlc.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gzdcwfkxi.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtzxhqbpo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gtaacoycf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gyhwcljjt.sHtML


<!-- 参考信息 -->