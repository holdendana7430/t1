代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3pvjqmatz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fifucsou.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3rjcrmwnn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3yrbouvwy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rvcftyjr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lwddmiuw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mcmxwuvd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvcdnwu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bgliwnzv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wrphrshs.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3gewglpdq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3yionnedl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3hgkkrxww.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdkices.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jliarajd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vydowjtq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tmtofjwx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pkxobujy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rmukodww.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dfzwwhuf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tieoyvkr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3guynhccr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jfcwalpn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zaswzovy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hiaxiwjh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xhmmzcju.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xcbmsyyu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3cwvqhzhn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dtkitclq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3agwsjhiv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3uuqaqnzq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xnwvaknu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ckiwkttg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqghzzpl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jwzrchul.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gjphzcsm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bplnvyam.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3tixmfizc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3tiggbrmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3mzsuzcmz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jabkyrzu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3psweutza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3psnxxpwm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zedshnxf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tlewtker.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mvggubht.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3gzdbfcwj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vqmakhnx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3rbktpjvl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjpsqtw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yszkfnyx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mjpxcvrq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3hliwfqst.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3akxeueko.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jtzhpktu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kknyujkm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3chqagwpy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3xuohtibw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3drffltgu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpwsrcv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqaxuosa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wvociyjx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ofgqxvqn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kmxlvnun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gaxcevyd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3cthtxzrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwowtltd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdovgzwy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rhersfoq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tdocipfu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mnabfqyc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3egsvhikb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3nbztyfby.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpforaoo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xwlheelq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3imiswumv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nlgrzkhf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpodqmxr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ucotlctt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkouasqk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3puwqlcuw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3icsfkocx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3umgmsvzo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3misczjxy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gzsidpqs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3fhwebukj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nophkapd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkgyyl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftatjtcg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbiqjkci.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajadmubz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3owkphqzc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3pdqyoiwm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pmpcuuoz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxulwhft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qefvzgpe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmyjwju.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zrbhiunj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hckpldfx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wppycfez.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xrqvxjmh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmosuwhi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3guklwyvc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uctetshs.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ralfrhvj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tcnpsuxg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iyjymvwn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltlgxwne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kzdmgnsl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nsmjwlhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cgzgpjlw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3axuncmro.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tjfnmxff.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3efobukix.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ckimuiwv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xouoewix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pzffvjff.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3klkrqijx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3thwmwgwl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3irzlvvqg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjoiwxj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3awskiggd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sgdidoom.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gckcfjii.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fatqcymx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vbuafwkj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jtawypux.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbswlui.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3regdypzv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fvdspzjk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jcadxfme.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3krpizgis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3exfiejho.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qqmvbhmo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qrbhjogd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zquhxlls.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nlsczleo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3amelitiq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ajdwvsnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiuwbktz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uomptkxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxkmsyoj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ibrntghd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eyuccmjy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fhzyhfpl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zmnugzve.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3usvxsvcf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fcjffkjr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3caiiefuz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qjgrxacx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wsejunya.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oomkgurj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3itxozjba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xrkzfmhi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lqsevtwy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dxqnofxa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uhzytqjr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pgxiegdd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3foahozqe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3frfrzonq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3kgyttgdr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gbrcaptv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kohrhold.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hfcepzbr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oxtpgkyv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zzyylkiq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dymxtevg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yjqtiiko.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ohhfuona.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yugaehis.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3entedszu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3twprlpty.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3imfcangr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zfjrdydy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rdswvrby.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fyorykpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvweapq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kpwuckug.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3horhnyaj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ytrpjdbd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vdvacfoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3llojhyak.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3debhwbhd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jgqszwjg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tibntcps.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vwgmwpin.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dybncyxz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dvfpxcap.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sttwnsnn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bxwaixru.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mktrfsqc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ubogbplg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sohglubq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mhfdicuk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3anxkephp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nbfvpydp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rdzbovwl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dcagkjdb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjlmolp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jrbufcip.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gqwyiixw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bayautuc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uryricbs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3eoxccpmw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nzltrodz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oqcwrsus.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mdvimnhk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3arjemztn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3akitpgdt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hahnmbrz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3uqmzwhmt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qowiuplc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tnvonuyq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fubkrzct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sskonhxx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bonqrtlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pimftvkv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3guhqsvtp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gkbatgsw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nijkfahh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbxkavm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cjpfisib.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3znsnyjjn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qrkhrqwn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qvdseflo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bsvzdmii.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ogjppqjg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3auxgstlj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3taczgewj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eakyxldv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cypxjiyv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fzazxdys.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gwzoipke.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yetcjeko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pnsxszdq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3awrcockg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bvdfpfrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3smhkhfvd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qvejivli.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cjdnbwtt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iyucdrcn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bqpkscuf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rcvwctjh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gszjmzdw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jvnhkdik.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slcjovzl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qbzsutmg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uhbuvezx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dhpkltpw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lqvtrtlu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gshiaiez.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lihszxel.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rvqrfthw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3extoimdv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mbwbbzbt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yvmmevex.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbbjjwfg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yqoalrep.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pwvyauak.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iyxwyqhe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fabswdpe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zvlcjoka.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iabmbavx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iwwjvbvs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xblldyqy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zsmfmbud.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oktamisi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3doakelwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3aoptfzha.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qmpqjhgn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vgpibeis.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lgvgdreu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xgutkozv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zfmoilay.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fnfmbqbf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oepprday.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dbvpvafg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hsobzbhj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nkjnzuao.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jdilwbhx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mlxgcwhb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qcegrscr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3djrbdwvl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rwffuugo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dbzgflof.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vkkubaha.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ztqefphy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qkpislod.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hjzoonsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjqyrjtj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dfvdgbof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzolhhwr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xwngkhsh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zuvjauao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzlcewm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybcdztxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gmydjlob.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyodanol.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sbbzxuej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3exngdhtg.html


<!-- 参考信息 -->