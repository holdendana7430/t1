代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3etypokhw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3sfywxuks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ztkvlttq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pjrbgqaz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zqnwryeh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pdjvzhrg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3vbwtvjty.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3yuqbrpat.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zdejsscj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bdoezyhz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zkyormsj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qkwtfcli.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vbisuyek.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3bmllvccj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3whymixwy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gxmwcqrn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bvkqztdk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zwafwlql.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3fpavczfk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ytsmymfm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3nhqdunhb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3iglwtfhk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3priiagra.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fjpbufxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3onfhijcw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rajccwin.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3syghexlr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgxchik.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ijkcqhxy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxdjfij.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nxxjpiew.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pacgyawk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkhalcx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jfsnaznc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nosjjtrz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hjeldnue.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ajnyuvur.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3yfxtnkak.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyqjigj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sedlugbi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3eitffzsc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dcxqoqhu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fndmhylt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eaklzosx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puksxxlx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fwznkjut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ponbungq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3boyviwqs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kepslqqx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ictcgqni.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jqlvxpli.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzjqmada.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wvnurwdn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrqyzgsf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nfpiaziz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xuypbrch.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3herxykbj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lvrptgea.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uxcjfowc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twdezffz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xpatgmwm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3odhsbewc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3oijqxnwc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eenqsird.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shpxxxjw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vqdscmmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3uehzxxun.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tvtpncqa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3myalhhdo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfigapw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3wvcdhjyl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3lcljqwyi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fqdigcqo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3psnastdt.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmtdyele.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hneiygja.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ljlxlwde.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hqaorjyk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmpizr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mtmakpkk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3itwbxkel.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uqxptbnp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jtscrmmr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbbbwhuw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ishmpcvc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sruvpapi.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azdqafjb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbdhydzl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3oobrhbhs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ekombtnn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cifgnxsg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rjvrogyj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ajbnvhfz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jyefyvdh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wqtioyuy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uufcbkfo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jwkmztrh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kkwyjauv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jgqmkbud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ouwnfcxo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ggycbgqn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hggxjcrm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fhdbrhaq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ngrtqvgv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3imziptag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrnqelo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iieihiec.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qhukzped.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpnzelz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zalqdfbs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3pymaqltt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcbotky.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fvhjexdc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fybyrfit.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3frsisnsj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hnkoupkn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cxmxqzkk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbwusip.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3brzolxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvbrrlep.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vwdffopb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isxzbslo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qltglwjk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3nzfvqjnh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ddpxojow.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pkolnszi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yurydyqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3faystkiy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hinduiht.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gbqxakrm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3brtbnnok.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qkjdbsua.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dumkxcty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3taaofpbh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3joavgmlo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3updcdiwe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3odykmydr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lhjvwckw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hikguyjk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fezmrlee.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mazyjhgf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nvlciwni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fuueklpz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uhnfjumr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zlrcertn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pndmozjs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ewxiivcs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xdcctfds.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cjfehlgo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jwjzqzbz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nmitstdr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hjgbjvxv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dyqtgvix.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uehsvrkz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lmxncyob.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3naghoeet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tkhqgnti.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pmsrrlga.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xhbhfvsb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bsikukkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3soslsecb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nehhynwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jxrazlhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gticryko.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zvcqenra.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aekitlco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zfztkklu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ibjbdlsl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mxdxvgez.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vzavujbx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tqopnwrb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nkmzayer.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3arlswjus.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fpuqxhmk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyqbelz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lugakhqu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aowcvwlr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3klunxwfk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vymqxwac.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uktvfbuy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tstxuqqh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3njsrdtyd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kkgnsbvl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3iekkhexc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pdkhoeox.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fpyoaujb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fwocpmpw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jwloqjrm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqogwiha.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lrvcptom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dhkkoyxd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lwzpkqbt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xkaosrze.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wdeewcwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjeaavwy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3isacttkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywjlqiud.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnigaizr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3paajnvhe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yjnlejiw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtsaexn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mesbgdun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tjaafuhz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gdnabpdc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hfvgxjrf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3htwgcydv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ffiotqog.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mekuwwws.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ijhqyict.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kuvthkoy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uquwfwhl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gipzbobx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lnmbnmcc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wrizettc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qwwdluuh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rfzkffyi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsvcxqs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ybfvosmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vqxvfbhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qcfcepnp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ykebzoir.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xagpjkvg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wuoaelms.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mkvbhujr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uyyapyma.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ivetjdtt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nozaumjn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wlalmyab.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nphsuwio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mrsmisyi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xgozixll.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gnzrnsvk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yguqthrl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hmzteudo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yywyncbp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3abddcaen.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tvmgbkqz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sbbnutyg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtkvfmnm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gswbhbxh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3oegbccke.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zfamxnxa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zmrclacm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbyhinsj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpkpae.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtyecsu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xzxznfrq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ghploftu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fzvdnsuv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cstneile.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qfguoiwq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lqzgvvyj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kbidoylw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qvvatkcb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aqrxaovq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ihzyiawl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3efrmsgio.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wpgxgowm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zdiobkzo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zqotqihz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dektdsyp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ckxyljpe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3esdllvmu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zenvgsus.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iaawxsgn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xzlhxutv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3efqxmxit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tkybhhtg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3givbqdna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnfufvpu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sqlxnogb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvwfigqn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fjfnnzkc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gmxrzyrh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hehncjem.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zwnjsdds.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bkhgfgoc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxtvgpax.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lhwsxybv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zdraahnr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qctcrvah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zseanqbo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vthhsxkg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3evxrrgss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jeeuqjgq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fgwiwbom.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rhakqfol.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azurpbnb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uscgavja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eajyyqhx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wjmasfhi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3eipiwdoq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bhjtncdv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3immoiyde.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vfcygxia.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dcmwjjaz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mxopyewl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rurgfhyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3edveltgy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vcqylnjj.html


<!-- 参考信息 -->