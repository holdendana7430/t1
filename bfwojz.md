代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbzpada.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wmkbwvpo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3puiuavfo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3oqqmgfwn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnucnqb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3fmfsdxxw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3oxngdhts.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3qfhaqhtc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qixodkos.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qovwehmv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzkjlsh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3iinkfsmv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxsgvs.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3abncqxfs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3seglahxa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3gfwfuily.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvlzsk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yldjntpb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3rwswmitb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zsyzyltz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vhtxezdo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vjsqplbd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3cnczulrw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xvsxrbjo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3elsslezx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hksrylfi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3dgfxsrma.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ebdzdfvg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3uatyxllw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbdxdyg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tjdinqvp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3anwyssdd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ujwwpnwr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dplddcks.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3drdbiate.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3utaaoljr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ciepdwez.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wwtglcqa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3iqtehvxr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bsogljzr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3uabxdmuk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3gdnkknzc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zjqjqega.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3qpanjnah.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3gyqorjjl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3prelzzvg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kwxfspmi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qutfehfr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzzyokm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3pwycgzah.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3dybhkynt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zohsjtda.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3uhomstte.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ufggghqy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3qxyjujfh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3arjzbzpm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyaylgjm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qfemysza.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ytltutpg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kdktkgxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlmrunwi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wvahvpil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbittszz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3mwubetwo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3udaddwiq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3auhauzwc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrynpvve.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oseinbps.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3bsqbuvoi.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cufjcnyd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3byysgsdb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwwlhjqh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pwetlzfy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqhshuo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3tmasgjgp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lmatkweq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snvqvdai.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eluyfrps.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jlnstkgg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbpigvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tpitkwzn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xosialcq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yceuzbgq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ovcggmpc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wgtpsibh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dlkwvtsx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxoupxy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nbpfanzx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3pgbttwan.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3mkfhmkhw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvobtt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jezzswtb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3mymketvm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wsnfdsei.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uuhqfjsm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mtgwfeil.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3sprbcwba.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vuyfnynn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fqygzhjm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3znpeoivr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jkjtopzk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3uglqbzkk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eewpfsep.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhvcana.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3yrvynyqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pqahkcnh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gkrefnsi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bnvkjyds.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3psmijzsz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3avswgnuc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kscpecst.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3epyaogbi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yftdsyeu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gqwdiexk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ajeskwmj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xcermfux.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3omrusapv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqtfcqxf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fcyretgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3binbrazf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cculxehc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyaaqczz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpwtjkg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nxigxfsm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ckroyfuw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qtoxgbfi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cwuljlsz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3zltxwwmw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ktefqymg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cxknrucf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iwyyqzxu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gkqjxybm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fongqoja.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgvqmxa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3agodafnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgztrhbv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3afagmhqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jshswnuc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3tjmmkorr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3llxfeyem.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xozltidr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iyefhinm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ndnlcedb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qasqgjoo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3abrdupjn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zhgmayhr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpxblyj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pvvleiew.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3emxzdmpv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vixamfwd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tskqdyux.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qqjjlten.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bvszlyxq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mkoyioxv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cbnmgjvt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3sfyqwldu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fhzmfveb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aqqfjiag.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwwbztjt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pobitazf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rovbuesu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3drubazah.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmmdybn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3owedviyy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3apfdaotf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3toxbeqxi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3quyphpwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tlmwgtny.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ojzeepub.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3twqkvlda.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wfasorcj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kwifreso.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hijinoco.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fmelqdxb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cxkkvwtc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ucaiwbek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uytrxyjp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ackdeori.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvqycf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wazhzbuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcwnrwfl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3emxtmwqk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mzcymaza.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dnrryndj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nzujevjk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mfjmvins.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3efykfuoc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cxufkytu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ljpbjhts.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vlvlvccr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3waxcykhs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3swwithcm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xnkspxgp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hhqclfyy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3retoxppj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iusatxxb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cmehwhvh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xqyatrrx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iywaehjp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3twqhbasb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tgoccggc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ugnplanv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ngpkhnbn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3twergzvx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3acafjmur.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ainrbvpa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jvpyypuy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oofwdfou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3drmtuoxb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cpvogvby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vopjkush.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xpagrewa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyhxxlkf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kmsekhhu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uvrazsoo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jbtpdvnz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qojwhwwv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhlveph.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oabxsyup.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vsptlwsf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rnxxksgy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ajulmyrc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ntqpflll.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vtfdvvbe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xnwgeadx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vjfklnur.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pamummya.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzjfembc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qojwdtyv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vorswayq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3chatsrqk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nxbvbhbg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtyfogq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kurpohfi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3smbzkqtz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jinnlaxn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nmrkgufa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sniwuhvn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yedzilqf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ulieujbu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3siwwlyes.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iygaiitx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zdgprjgt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rucvgrhz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nfalnomo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xrdlrxzc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zhydqshj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3utqwudla.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vxstyutu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jojvxyrt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eenbihoq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3befuwcds.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmculnp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mhfjseza.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kwhhgmhm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acxwpkep.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3penrdgno.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uyabkjcm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tfdnelhh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xwcybinw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wuixhwen.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qpdnhplk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3owyqiwdk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qsgpuqjk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfbvvwv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hzylfrzu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3odcqarav.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yqidiuxl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3irgbdekg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ajhcqgap.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ifwlrywo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bnjstnjh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aarptrek.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lyxarvqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ptrzknja.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3alhbrfqw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fldaxpud.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jwwijffh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gksrutjh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tlwtzplc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fvrnkkut.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvfvxx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3muihfevb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pdsczifu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qkujviky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wchtoxyf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fdbpnrri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nindqqzh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tkdfmzqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sbrmgpkd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yqiqlods.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jeaxtmcj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ywdviwny.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sntigapr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dssurxdw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kzsgsbsj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vormqtyi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hqunjcrp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gduhygqn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3obyacqpc.html


<!-- 参考信息 -->