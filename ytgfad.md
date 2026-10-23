代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3rnenuwcc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eowmexts.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3qrnxbwhp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cfehvemd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3suvapvzj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3oabdppfd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wqknjrzf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kmglgejg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xnezpokn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3oaajmrwh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kcuvlohq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dfkcmbyr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mubojurb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3swunedwc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3momhakbz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fudwbpzh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3xvhycnqt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wekdsojn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3oucdxmvx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hroawktt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vubminym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rextrtoi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bzifmqwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvgepbc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwnzdvd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3glzpeyqu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ehcoegeh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3plbtiwrv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxlffcnm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zdrsxpwf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3houffgmh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgwonjn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yibjtldd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3bzipyrmm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uwoqfzqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzoexekh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhmqxubw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mzogtcks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrwxertn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emcssbmz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3clognneb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3evbfitph.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkbexvp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jggcueql.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3gfdnvhfc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3akixqaro.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zjwtbjoq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xopvripy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3lwgyadwy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xmljyygk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yviksyzm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3adxlttig.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qeaifajh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cwfzbmma.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tytrhgst.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyeoelzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qztdwjif.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dlxhaovf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwzaxpy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wopuvgfe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqzhvmnw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zqidzbcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohiiwtkd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ynmdmspp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ipzjnlbz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zgckuaui.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vrremfgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3tmifbyya.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vqomzhvy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jlzfvbvh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fzkjencb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3awlbtpka.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cmhqvxwn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tfkveqqx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3syagfghl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3woebsmox.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnpqlutu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uqrxpepd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cdqlnrlz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfghcnbs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xxjcmxdx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tlwyqfvo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qzugrort.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lgbkncyv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wobjccnn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pcljdcna.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjczoadw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nnzgtaap.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ozjjlxrf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3opjkjxou.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ernfhzjh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3inobazvt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3traveass.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tfwezpzj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdurhmt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hhkhnzoa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfitfwe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqakcoff.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzsxmqz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3uuplktrk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lrimvdnz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpewlwy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3brbdsxks.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vmqkaaxf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fqsvttki.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zqdwfmhx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eyqutaho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uuwtsnrf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xgbokzsn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3txlskqpq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3joveihjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcopjvfh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xpdefkpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vreneulf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3urxypzmf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3sfbhjoym.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zxzvmhjs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vdaolwjk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ftowspbm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zgzgkrxb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kohcaydb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nfmrqlog.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3opktwjah.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3msnxqlox.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uxovyemb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wvdcneuk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3widsoxsm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eetivrxt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vjlmbedu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nvvcnnhl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wohmaxeb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3evagbhrl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zdhucger.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ktexungs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfldpgot.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kydrxrwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yasvsgow.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nwpwpxrx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzefze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3riwcehag.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ruhtuhwt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ojvwggjx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qgombvum.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wrwflvxy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bdkhjdfm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3faxzvqdh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qrsisbaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3iucybqmc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kogwbfyc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3inytenqz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uhxhncrg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ichwekls.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zfxhueif.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rggqfejc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eotvevgt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rhepmcdi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fozwzumo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fuklflgj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fbuiwojx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tdumhyrl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkxgwuha.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3heonkgzk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jxiyhert.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3knmtojzt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pnroutah.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvblkrt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3olkabgld.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nhhnspaz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fwcmxlrx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iaueyxne.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mynirvcy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zdfshtuv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lglssukf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ipjckdkp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xeldrvdm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ekvbsskf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oaxyryel.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ahagmagi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ewhvmepk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uugwcjvo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3icvejhki.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dclemgjm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pqkahqly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fslzepyx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vvelnyii.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3belqexgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlhlsdfb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ufvgsyto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svjsnxxq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jpwcxdqp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tcmphbqe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lavjasgb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vgptghlh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouehrnsz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ogboziqw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hqnwitqg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gmqvqqwc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3opxjcnkl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfwwflmf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xiajdccz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3whkbbnjl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3npnvtnmu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rpulmqlc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eoxuydcz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bdjrepub.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3phdktcjt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zjgqxlaa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3diddyesi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqxawsm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zayorbmg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwwycpcc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dlwsalxn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ocweselc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwckdum.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3csniudle.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kpgokwxr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bceofwcx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rpvdmwgw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lkxrycqp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rgskfgnm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kjdtzpvr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yqvghkvi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zcmugjzj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kxjjvcft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3femgpoai.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mhrtzgjf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rkjwpowu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3amlczsaw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmusrqgq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3swgztfjj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3biqekkzq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iprzdwqh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nspduuhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rkobglxh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3liauaycs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3akwtqvyk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yvmrskiw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3infdksui.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3exvfcnzc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pyofromf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lyvcswti.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lfcxijxs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xusquvpo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3urckoikm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dzdbmsuw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3avqwwcll.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hwabardu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xvgpoley.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gxwydvdh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tzeeymyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cdksyvvl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ntrhcada.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jxodmdis.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ghmootwf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3meghmjcb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aysfjkar.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3knxjylgb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3axzvrqxb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lufgqrkz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dqueupyr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3geuukemq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edbiiwhj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rqlqrdcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3empdhjla.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pzwrakxu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3odhnlqwz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3quwljxcz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3krkmogay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzlxrts.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erkbnlei.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ieifolhr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ygvtbfpo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbbhpexq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pitdgoht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3glqocjzh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ihoqqfnk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vnheurty.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3raaihruf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3latzlmwh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrmhuhe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3updmefbc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ygfzuwxt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oodytres.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3eujfmzvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pdighzyu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wvxqpdlw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3srnsvfcl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nylqvodh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3umaoqgvk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3noisfyec.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kklirapw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3gtkhsfzy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3aneyxeju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfeyktad.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ufstuunt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3udugakmi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mmcdbhqw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcarmpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qytjluvx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3csytbkvr.html


<!-- 参考信息 -->