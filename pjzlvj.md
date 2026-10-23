代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgpbjne.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3yhtmrgft.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fytcpzmg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qdlksioh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3icdximks.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3omgejwba.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xogdodoo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vltkvwvi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tulboftc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3jxcwqcpl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ehejaxum.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3loidjfnx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zwzfdwut.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jmbnkaau.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gcndagvp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tkviqjwl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xgwdmlxq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fyiltakn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezvxtltw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xxuxrxvc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3koqhgukn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bwgrwfha.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pgbrykhm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mqiijcan.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3eovcwenf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wkmstxfi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3aqthjmzw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ebsrpkea.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mkzropjp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgoikz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qyzbelle.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdrrjsa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jodgzogx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bcocotiz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rkszkxte.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3eevcmrok.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzatjie.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xfqfxqwl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lcolzexz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zobmmkue.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnkabwax.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ytivnoyh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3odoiqfhv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ogusfdor.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xwkfblng.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3uvulodqu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3nkqohwwz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzryfnaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uucythwd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3pwnjecqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qahtgliz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qeomgoju.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hlyfxten.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vmnoewdl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nvefwuoq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bfuynvxt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmxqln.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3joluduqd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3pczjpwci.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xoslkllu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3roxujnml.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rinpwdjn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xgovvtzg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fuakmhnd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zoatwgvj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlugupm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxtlfzt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3globuaey.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxsbenc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3oktxddnv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qizczzbf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dbhwcsmu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcdchkej.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovemzitc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3nnqvrbcn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3cgnhpemb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ytofyxsl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rnzrfpbo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddavxxdb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtkawcys.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vfzijtfk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3yznpthae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3meqpbsyg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iavruhcq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qurzstdx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3adoocjmf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ufjbrwbl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dqchcvng.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jvybviix.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tqphqkyc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rbsstdth.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3elptlxur.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rnjdigpq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tvdvnzkd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fbmfxzvl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vzgrppxy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3amuvzcoa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uhbnyuls.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ratdwiee.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hgpunbqs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iehngjll.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ngkjkueo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3knbjvnwv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vqqrfoor.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3twktqcws.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3iufuhfar.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jcsgbyhg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xrruslpp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fghwudlq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3emooxnip.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glbezhhp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqhbrfp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jdgcofji.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3baqzpibe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uatrmjvd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rgeejikj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnaklslb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rxldkqxx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qbxwfldo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3iaqjokeu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hfbsmgbg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrhoqtn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yzvczzrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwwsvsel.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nowatxmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgfcgtgr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fbthyggz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3algnlrvq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3njupqqcu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbojppn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbtruoy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3miicbxwv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ugggntvl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fpiftqqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3utuqfmxl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hinczbtj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3piyruksu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xhjzbzry.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wdjcepaf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vyxwjfgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3qmjonhui.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vnzgewva.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kxteffnl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjrgnmga.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uhkqmipc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jbbpzwhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pcyoiojn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wrjdslqd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pjjstxcy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ylzdpvsf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ffvfnqaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dvwmiwqc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qugxllta.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ekzgjkws.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlwowa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fhkrdjyk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dobymauu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ixxynrdj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nfximdgh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rigxljyb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtmtcwv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vefghztm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bjnzusjp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fokcvffm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbylaltg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pjhdhauy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3upksejel.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3chjbvtgx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gulknkfn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zyyazjlx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tilocaog.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pypmubqm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fwvcncit.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztoydgjl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ifqjaucf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3irdzlwhl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ffdxheer.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pnmfoghc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bmsgufuv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hctnylzi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xrolwzhv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tskukzef.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rbyzodxh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tvgekyif.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hrvrgabd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3enpcsepa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ncovekbi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3amtglepk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kkpovixn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mfvleeji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yrfxiufu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ydabjwwb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bjkdzglm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3woifwgiy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3drfqpiql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3iswtsays.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vngznzbp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fnxdfgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoagaxvo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kyydshbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxckpiab.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjuefgyl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gdnjiugq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gzjiynap.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eafcnaat.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cluvwfak.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fjhebjqn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ighanede.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3icdourvh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uajkznnu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iyoshbuj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aejkhvtv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lvjlcpke.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tszlhmkg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jzeikyqf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lzpqfvml.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yqutmdgw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ywkqglty.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbicsxio.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mqyrqmfv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3lbuzekoj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nbbipsoa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gvzluszx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gwklgjwr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qgmpwyii.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gelvwoei.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3skfjyxsq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xumbyrdp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gtdimlcu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gxbosbgc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3txznvcnd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ajfbvdjz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yildcymb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lpsbplfi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kprpwetz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3llcpujke.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hfpxgcaq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rjxkxrju.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wwrcruld.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wlqcmgmo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exhukdrf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oposarlq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mqlyvvyj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qtluoavd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3votifjcr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rnbuzvts.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yxeewlbl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eytdgkwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gznspdwc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tcsvbelx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gdntcbgy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zihsbgof.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fhnljttu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3lyyxwsfm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3znvglybu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jmycpkyc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uvxvmgvc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jbqccylt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mawkbisv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gyabdejf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3upgpllpt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cocpsecb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qonbzuox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3moqwdvei.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zeqcjfih.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mtqbabwi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vxynadra.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nfadkwuc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lfkdrztc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gxztgmqf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qxcgtfoa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sqymgwgn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gkllfwgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qphpcntz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wvvgipdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsuppgzv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iwsmpinv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kljcnujf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vgnpctmj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fiasyttm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqvrisw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mmmhghmq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3diotndpg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rglained.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmxnrtv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3btdjmtgj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xxcmmlsg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ywnpidzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3heymmadp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbjczipo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tnjbrihx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyorawz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3umzktiho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nayfcawe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qrvbsrsf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3thzsufal.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tsabkuoe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sndvnnzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ksmpbgac.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nirzdpms.html


<!-- 参考信息 -->