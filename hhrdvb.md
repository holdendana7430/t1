代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2gmcyygcr.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2aiznmttu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ixxclpdw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2juqutiab.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2egyjmutr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dojlchqe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rqihphyj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fekjtoys.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xhqotpxh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nkdnhldp.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2nypacxel.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfatrqwa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2sbqricmw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxrucfm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbidrhj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2reqoxkkz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nlekaowj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2cymrbzbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xeobkhky.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2zeiuberm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2awlgmxsm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xcrruzpy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ggiyccll.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2eluwmgjs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rltnlxvz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2aqgtnlof.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2poxtqbul.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bcjhuoea.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gtwafghf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2muneppag.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gthtsegw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jowvwckc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fembafzh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ayqwmqec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjtffhjh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kjhosmgu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2flxmikre.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2osyqvqia.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2zkafuskd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eoyqvguh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2twhrbqvx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2egteqvvq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jccgigav.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xjwgvfbg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qpikjzmx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2siwmwbrg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ozhfiold.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dezyxryu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jdrchysd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gancaqsx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ssnjmeob.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zymicfpc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vorxuqaf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ltdcmhnj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gyqdwjun.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rigeymfu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2litoxvzr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2qacrhiyb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lppymflo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjmsffb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ufnfwawq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2nqwrhydc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vmblvivv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fbazecfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvzuiq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qqijkdon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbneegzc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dilsirpp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wqttbhsv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2eyizjgfp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2egaeusqd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2oxvaeoph.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2knzetqaw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lopewjyz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2oggmbccn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdeuulsl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ufgdozbu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jexlvhgi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rdxrenps.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2txuiilik.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bflmxjmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gqsquikm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2slpkoifp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ijetviqv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rtxldnyn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ucqbqwpw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ywnmjeoq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2syossfig.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yvnnkdci.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2etbruery.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2bkfltzkr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2fpqfhijs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2klnebdpa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qkddgmjv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2zbfusbpx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tdencbhj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2glxfoskf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rorhxxhs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kuystvra.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2riajfnzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2umawradu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmgqwufc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2koagumbi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2psooijcz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfzcyor.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hnrgneub.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pverbnym.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iiyllryd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2snzexjle.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mcdalywk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wfnroufb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mlckdzxg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gdptsgll.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pzmsvqtj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2uuswykoc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jidzskze.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2srlchwnn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vmnnyicl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2drioeexv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xfnhhtnz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yhicgxdq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ldhoukbl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2irucxqjl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vwsfafnk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uixdjthi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgxiuyi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpfvpad.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2sgelhlor.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xteqstfa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrstfgl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2oerlmelz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lphavlos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zabtqjpn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fsjireit.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mswniwov.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bfvwblfh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hhgicezf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgvfpyr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mpqyiszh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlnvyknm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ojnoftig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuvgdoxz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dusyzzfr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ypwhjtec.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gbhuwxbr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pegpbxhf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pxyivjlt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uscnxpri.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvhbjmq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xbwzzbhb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iaccdpsn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yyhlojfx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zlnntoze.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hveeczmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2megemazw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2afvcenpg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kujbcens.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2czhzhsfh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kxomcazr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ofrezayv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hwcxheki.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mjmeohic.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jsaaqjbh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gkhwpimw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qcfzpaes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2repizfql.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxoksdk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pjwgfmvy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2halzrfua.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hggnvxcd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2njanmcwy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jtehziwr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ntedongm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vuispwrq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2exuymfda.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2eujwzkvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgsahck.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqmfsr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pbrdhiof.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zcfdhowg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vqegqlev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oyfbggef.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dtqilame.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tugmhqpj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyzodqoh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oxnpoeyi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uennxcuo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nuqmfqrz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xwupioxr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2igigsvpt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wglbhzic.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2olscedfy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zaaxicef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kbtmwjbk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ataakjrh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fhbpkvir.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pnfvnhas.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gmqfyqwz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qqrkkioe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2stvtemia.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fmdzpmlr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2blinamrm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uahhjnhh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kmiznecg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2syvrcbqb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dahjcntd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mtcwdiaa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ecynckye.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zozgnxhg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hztrrqtx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xehvdkpm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vknfwkgn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fzfbbbtv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ujazmoza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khaumuza.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ezwmwzll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiaozxte.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2frbfrrhv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cpreeprc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2jcxerhvh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sspwcqsq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2emvbybbw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2llmfyyqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rxcthnmh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2exzdeefm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mbmblhim.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rjmcfyba.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pvorckso.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cvbntctj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2seudsbis.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tajozozg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ckkwhbtp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ceesuwml.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2krzfawmv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2axuxjfeg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xuhcsewf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lejbmmve.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pgxfxjcc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zmdltcrm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rssynhgq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2difboist.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bxsbsydv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pwufyjur.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2unongtck.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iighadoi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2atuudamm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hvcfdxeh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fdivuxyi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xmujlpiw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2racwxqwd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pvrlsoau.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2msobwszb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tfglyvdr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2odpjkcqr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcpmwoh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2komfugol.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqttdzjd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plhxzzhj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwijntaa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fglicgme.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rkyvlayy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iwibckpb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ectksrld.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2adriuevq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ufdxjdlo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yfegrmte.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdmlnvaa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ezawdvdh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ebtizybc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2seehotuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2maaxgbcy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vrxlgwdv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vvfzloni.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pfmgzjhd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ypoabqqe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2obrpkdnt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2avgfctmw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pgifjvjg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gqvrermw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mzushqim.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2esieodeo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2glcmbffe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ewjrycqa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xeevqvea.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ovbmcdwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2czgyvkel.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkettb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qsjnfrhg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qvkgtkkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxkqnrah.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wwhzahxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2titmigxe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hlwuuknk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wjpcrvox.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jiibvwhz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpdrdkq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fppcpsas.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mekexckl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2exuqtdek.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bjjtcoqq.html


<!-- 参考信息 -->