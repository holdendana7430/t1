代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3pncduxdu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3jjbdwntf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3nkzyrofv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ppjsfpsy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qtsqinun.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3envgczly.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3nvgtvdas.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3aujngjry.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3aywhwjru.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pytjoezc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3iqixpnaq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cbdqqlxm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vnrcibuv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ccwxbnks.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3uyhprrwi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bqhymlyo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3clemcilq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3typdztzm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pjpmlbeg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3nmqohubp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3otxwatdx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wgfmpblw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3yubmpdno.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3fwikyuvv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3jcbmdqnp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ufskjasp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wddfgsyn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3amhegobx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vglaonho.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hoxiwbwe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwljdxk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pbylemlg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3pqbcauyy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3glqmlems.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ofhhwecs.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3rymmhyzh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuczfzfk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vucoaute.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmbrxx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ewzilayy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3cpcxnsbj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mkfxdzcs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3nlibwpxa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3glkxaltp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pigkpqfz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ocqvybow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfcevcbm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3popaseeq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dciimkms.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cvqladsu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftddvfkm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnugbsr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jeospdbm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yongwnpi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mijhfflz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wfpybdrd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3amklaasd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oytvzzsq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3umtskgep.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igjiemkx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hmsjmstd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ktlptsyi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kwdfdhst.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mteoajwl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3rrzddeyt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wwabdnpb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fzvbsihk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zffldxlg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qmozlwfd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gpaikgwr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dkpzkjbp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3yjnvhypg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtxwgfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3whxhjqnp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ialnizks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwblksxu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rfxeutli.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zfvgvshg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bosxfnfu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cehpxcdv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fmldsyvu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyvshayn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3omihzukr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jbeebuvc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tlvjapqb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3syjhchog.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqohuzja.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hkeciint.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3igyppgxo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kuuvpzrd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3szmcdptt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3eonamuon.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3upupacrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3prfgjtol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mkbmrtgn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3axfhbqzv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3imvkuses.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xfydelxz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zcabemng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3afwysmxv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xsoshfro.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3skczknpz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmecjbxz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3dykujqwy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rdbxndai.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfiopgt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vemcrosp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwlplco.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rdqwzpcb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xoatrean.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zltinjvc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqcjwbxi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrmxcdoh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cmfrplys.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cjnwyzhv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dxznfkno.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ciblpfbb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3cpnkhoix.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xwlnhwxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iarbqheg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wlyotwdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwyewcku.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rvttvnqm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pyytzdpt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ojbeqkcx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zijieyyk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vrmlysze.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lkylummm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3drdgrtvt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3geykgkmj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lwitgjlk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ohyjwbnh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yxpncqwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3diqidhvp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3omfreyqt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3arasbvwh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kclmqjta.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3laawwalt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3klaqecje.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvrmqein.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3arwkimdp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ntukwnkd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3escxuvvz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3haajoguy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zusbobta.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sxeodzgm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ussgryyj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3skfcdqlw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xjrzpwcr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dchuress.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bwzufooq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fostlggc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pfwfgnhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vsenfxml.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vuwtylyk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wuvczyav.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3enyqvbmg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gcnyyfby.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kcupuvow.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wjxerioc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdxpkuns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mfgdqjnd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wsxzifmh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zajtrpfl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3voxuoryq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wjffpart.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxtorork.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wwbyjrkg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qxuvzdxl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lrtrttac.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uzizihup.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjdlsew.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aebbvoat.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xhrqqqvx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzmdrqr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3epfafjcp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cxwxumag.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3unybzzlq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mntwkyft.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rqnilabj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cbrbmyaw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3njmepozg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dufwinby.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gfpweoxm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uiqzcwnb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ubjwpnvl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3labnvxhj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hhlhvvou.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kkdumvte.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3teamjegt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3afktlyha.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3omzhjwdl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lqphqbww.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxfgnhrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbdzcfle.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3czyecclj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vknrxpsn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pfmvbcyz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ctglrsfl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3crrrryam.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mqacjzld.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qrytgurz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qhzlhzck.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lgmlmyup.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dxdndbfr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kyhrtbfp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nisvzhnm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gkximddn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nmsimzpk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eygzbswi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vwbkvqzl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nidlmsas.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tuvabrtt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dtlkarnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3otqmamxk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nhupjsrw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fywmnxug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fxrewfky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wuvxtugj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sqeinbko.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ngnxvvan.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zexiydjb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3sxwikxhf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ttcalgsx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kxzlfytw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3awahckkv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uhglrdkp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xxqxfvrh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmuakpqt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jtfiybdd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qqdkzuoi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kekejqvh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fjhxqvkb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eonqmtdk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wefeukuh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3stgitufx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pdydenyh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddugoyoy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gviqmtup.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eskokjmd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3djhvhvkf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3girhlsig.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mnjwyjvg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmumemdt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3znjpaqup.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nkjqcmki.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vuwczjbi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cydofdwz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ukuzoppg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lhviyuay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yltbqvdi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3czgbyvum.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mronzkfm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vwkxnxsd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ctdptyss.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zewadulq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3toheqiyo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3usrdwjws.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ppearhcx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3usiujiyq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cxeewbmp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pavjkfuo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wtrcdylq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sjtxlxcy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3flzmtkao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3biormvho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cgsmurmw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ownrvcog.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jjmdbjol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdrhzngp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mheradhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnlzdubb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tlkwzskh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gfpezwtk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gtpiywnc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zvrtxkvv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glnabagb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3svxaqwsy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isrmnlev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ijjezttx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ytfspzfn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nlztgmwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rtyvroux.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nndcbqes.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnpwiar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3chlvpadp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tdtybusl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqiydeyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tdcixmim.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wwsqsaem.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dbryfdci.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dqxnqgnw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fqjxmten.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3icgmpkwk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3svtgwsos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ipzjwsos.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fbhjpzmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3dvxteudn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mhfxvmda.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nsncnwcm.html


<!-- 参考信息 -->