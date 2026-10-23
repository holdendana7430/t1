代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fpsfgxqz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3okxfpmod.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3qtrmruex.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yeqrkura.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wbmtfvvx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vupjjqcn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xwnscwuz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jjvsynvf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3fwvwssgw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jqiinrbe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ytxxczlo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3cgyktatq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ortaqkjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vhqjdiqc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3fzgotkjm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bojapodw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cvshypht.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ayquowos.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3redxmmmk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3koxirhjj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hiqkxhll.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lahjgvog.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eligraiz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hscqpvhg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqiocc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmfvra.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nunhheyc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3padjozex.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3yxrddtcu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zzmvssks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3hcynwfmy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3gtaiuxxr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3scycygbv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rjajsyhv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3hjabvbvd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wmonhiyr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ugkrllyy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xyagzeez.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3rlmcxzuo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jtugdaxt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3trduxwyp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3goseipvt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwcitnp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oogrcvsi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tqloolcc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3jlhkfkwl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3uyoitfow.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3isquhlpz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gjxpgqla.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3jfeatexi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kmqkqvxy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3serjdnly.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3semruiyr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ulmarncq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3xvpujhfi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3oycpzwmb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3tzrozbmr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ddqqxqbo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qwbxpgue.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wihickvc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3oqguqcjr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ekuimmzi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3plghhjjx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xlxnndzn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3myxruxqi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dslurkcu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3heqqwlys.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3azvqbtqi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsbhlqvt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3sieiierl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ypuvvchv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3syjezxoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubjzasgb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3anlgownl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sotslvmn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tdolqjqm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3myhzopnd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nyujwgtt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3piydafcm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dfocstio.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ofspmanu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3akwttvsc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3awnulxdt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idhdbpiz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pzzpefyu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3peqaabwq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3lvvyrjno.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxgvfbo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgntbci.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mrefnfwz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3koodnufh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnqijkgc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nswfkwxo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3cjbcbxwl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bloqrvdh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3snnbraih.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3poiktaua.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pneeilbo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iedfdwdy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qivdhdsc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqxkotk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xfoizgwk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3sjjivtxd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ypdxswkg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rqkkwann.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dvmarhqt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3epaoyobr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3reropvbw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iuqujyql.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovhonlex.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vbhwkhzj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zzhbqemi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iurtummd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rjdipmhm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ryahqqju.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qvugsmll.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3syeljopi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3cufzkfjn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hahoanwh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3zperbuig.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zkillnbc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yjfyqsdt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3osfbsguh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gququhix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oenxkakt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nlpppncd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zouqnoav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hvybzucj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3apxlzjav.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ypfbmakm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3drzihtuv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ondiopfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bcdudpqw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3onaxddcx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mjmgcyjm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ztpqahpv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pazbbbar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hatwdajd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3idaylnis.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtniuesx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zzkxcggz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xiwgckpd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3asroykqs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cbuxxkbb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ersaquhv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwllxsdr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3njmkkbcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uggeazgx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vuzbpiic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wysjmhqz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qoyozugl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ognwpqfy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3exldjnlh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwtahdh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vywoqyws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xtnuusaa.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3zdeoaqsj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3owkbajpz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3syowujyf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qmygwuqf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nyjepaam.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jsgtpxsn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xlhcwtum.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qugnxrhd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nlvgnpez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yuyhhhxn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ourqarpo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vxcwqsvq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yucsnudi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qrdezgdo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3flbohybk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3okowuhyn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3whlezrhp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rcfvnvnq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3omsghahr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3goojscjn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ddvagqel.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rkzjgfbc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cjyeluuc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fwhplbic.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3udjdjecu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cytylrax.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xhwwiwlh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hayzfpip.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnfxjwx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3scsyzqka.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3goekvbui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jjovqdaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3chbcivdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eqczfqiz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zfasygse.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hxnmdass.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbtvkkyv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bqnhnykb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3enoywvcu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uxbdtkfi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ircuyvnm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ofvovqxv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tngtkvob.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qmklwtvz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oqfwixtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kwylpnnc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xeayhpuq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gwvzyrry.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qaspyifd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jsfatkso.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fggnepwk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jjzfcpwd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eecvddrk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hefbyjrl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wafbdihf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bebtdfli.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3azehplil.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fkimdabr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3aaaqhzlc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qlrmuodm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ikjtlvgr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3isxnzzzz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ijcxtrsl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lqusbksl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrrborq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sqvhbrds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqofrrce.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fgzwxzab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffrdgvor.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qmqaqxep.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vbqmvbvz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3azgtstrh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yufctcwb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zorudfdq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qzuqmpbb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tlrarfuf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fsukpwlb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ikwbwqjs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvcrzfll.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gjhzhnkn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nheydbcz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vmjyjtjf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tvgrxsfy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zpbitfpi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kfxlayhg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cbdjqxrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xqceipns.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zoeeomuc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cqihttxp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rlgyudmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kngkdgfr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dumdoczk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ijoxpyoq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jehnsxlp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fpydfiwh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3slgwqboz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rdpgautd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nfaavbaz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3flsdgmkf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhkotnml.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wntklfjv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qcpcqzmj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnvxddso.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ycjulnfx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bmcawpkl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aovudyca.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvccadz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3nehyhbia.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zztnyffz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qvashqax.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3otocpsbg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yizcyfdl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzriqgng.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pigixwak.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqvmpqfy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmpctoi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hgejahbn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kgnowdxy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rjifxqkq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yktoijer.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gkmwaelv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hdqjnlav.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kbblofov.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vvoxiqfa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nvowhtbe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqggtuee.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xxcdaxhk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rubvvjoh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3akgsebpl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zsgkjvoa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lovammre.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cdlyezex.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mkqzdyuq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wdoisohl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oapvuisr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rswbroej.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nrotsbfr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eidfbwqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zzjkyhsd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dszzpljc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gcxatrlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqkjorie.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yqwzqeva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsuphdmp.html


<!-- 参考信息 -->