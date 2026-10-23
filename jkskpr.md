代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tuuuedow.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oyldiaju.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kouybabs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jcdnplxh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hkspsxaw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3zkoqwiqg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbuixgp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vypekclm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3kgjhvrzq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3muoveglp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zcztmwsi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwemyqo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gmuauvgk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3stvjtfax.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3onbclxhj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hfealpun.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3igwrihyk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3gpmneqbr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dfoxemcv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3klzueybq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ackraafa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wkobrzxx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3nujwngrf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rftbourb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ealompqa.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3dpocjrvl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3oitcdxdy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jlauxmsv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vrhxmpaz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ounnrozf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3rpfyuwho.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ujlwhasn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3fjbzzpgc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fcdatqmn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3unhkwjls.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iuvzvcmo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ljsaytjo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3cphcdhxg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qjgqwrnh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kwjewvhm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bdxplvav.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3swacoeoa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3aiscuwke.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3vjkgwiwv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3aqwftskp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3yyduezid.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3fmaeievn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3svaxldvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3clfuqafa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ahqkomko.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hukpctby.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3avcyjfds.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3lnswxqub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3txxfmdhp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lhxblwhf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3sxoasxvf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iaanvegq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3yycactbi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3leanudyb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arkrmqem.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gxkuiawm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qavzfcsn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3iiruwqwq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3cqhzwkbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpzojfpb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3heagzqgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giiwywbd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpeikgno.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmiqfai.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wqliaebj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wcdaabci.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wpdknbgu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ajyjymcq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzxygur.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3djtiqatb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvnksvg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gvxacysz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fycpirgr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3cijsbfii.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzdmbnq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rkcvtgri.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cukngcvd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kalqsbyx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzkrwiha.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jqstanxb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ubzeiqcf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3phqkkrku.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uoxkinpt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffysbaof.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acbimohr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nkcnlhtq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wvuysuvq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vnglikrs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3slmsyual.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kmgnnohs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ryshpezo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jaixdwty.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lobdotvp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nmwaqzgp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yzqtevfm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gehvcrjp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3weuvgbps.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkznpgjr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgdguegg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvjelhx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rxupdiop.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xhnexugv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjvhqzi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3qaosdgby.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3csvaqtdg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bpgrjmft.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ahcpmbjv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tpismpcq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bfurwoih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wtkedqrm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnpmiza.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oojdmtuw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xovutgqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gjqdyjso.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nhjduycp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xirvazjk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzznhalo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqhihgg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cdzwdeau.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ipogugyt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glitrfsp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qzgqzxhh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nlmltpis.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pswvunyp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqkqmje.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3iumprghj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ywotvvxj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrbcoosf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yfqlqinv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lctevtak.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uszvrvpq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3enwhcdiz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvexqxr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3quallivc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwwansfx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mnirxmyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kabcdkfo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3btrtbcol.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zosqfywg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qjalvcvp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pxsudzkz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jmbocdox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qnsmemad.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qndsekwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ayjxndpe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gtgtmkjx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qmldvzrs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sdzvcveh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3evwgsflb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pvhkltek.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fofplwbh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jkpvusjc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3minccvee.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vvntgeti.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3scvfmzie.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3iyvnhbsl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fnrundus.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqhnpdqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hzuadpdc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tyxqkayw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xmmadcxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3eyuzecum.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qbufjlfm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ndgftgbc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lzpwwlwo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nrmrcatm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3recqyxog.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cydbcudk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kqlqdqfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vwcfwpsh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qkijgiza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wxeokpod.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mehdvtuj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gnxpfdhu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3shwqpamg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gvomdsss.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aorvlwry.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3razqnudj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tenysrek.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3smvvfshb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3humddjpi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vtcccupb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3muwcvtrf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3opyltglm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ifhmubls.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bmpopski.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vkjnnjlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ckuvoplq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kopawpqq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nlsxycwi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hledprap.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tbqhhbtn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3veknvebw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qfqwbuiu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yhndrrrx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iujlkvjb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3riwhruwd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tlgowsvn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ezgudsdh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dgyxmwdv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qlqxteip.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3scquadjf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zcbrnxve.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lepaivrq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qomwdija.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hjpcbjex.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nmorxlwk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ohlqhfnn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rnepdmdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajqedgod.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bovogkuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3saquhuoz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lxdlzfxj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xwzftlax.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwyfubn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhisjlqe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xxfvrwau.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hxsfofni.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bqdcrdyp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3naidhslo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ppwamfgl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fsvrtzmu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxpocmc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mbtpbyto.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qrjsnoxh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qcftjbmq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zdeknjje.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3elbmagmv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nqlzbhgl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jfmofkca.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rpwcaakp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vseinbib.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3psaqbwsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dkaxkyff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hrugdnux.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mcmkxudv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tfpjlkul.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kvqbpvfn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lextbkgk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jvjlkweb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bxjghchg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3azwefare.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fycogvuh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eqfivria.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ttpcmgrg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zrsowshb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rjolcanm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yyzotprn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3glmnkdwn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyaason.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtsiqirj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fchnoblu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3farnwyei.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cdqwnwmz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gksvsmmr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nnqfrvmc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dkeguipj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fgbayxcc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hkwddqks.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tobsgsbv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oyhmzruo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hxgtnumm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jlhfhyxq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lcvyputh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjaxjh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nkszvbeg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kpnedjke.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ljasbewy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qhzbehzv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gaqrqmph.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lmxdrwdc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3moxiiimd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hiurgvms.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hcjnbbbf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sebragbi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3enllnkzo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3skovjzwo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3djueglyh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wabnlkyf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wcxtamlk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bgsztfmk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fsxetose.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vkngxwyp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xrmeckxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqimlqlp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fxfggjhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlzojtue.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3twvmlojt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqhttqf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3thefvuyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3orirsznt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3weufqplg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuvnynmz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqznokke.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tabwnrub.html


<!-- 参考信息 -->