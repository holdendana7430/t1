代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3xceuuamv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3klzftruh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lyhgszzs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3bqnbeokc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyapoye.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ratidvxv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eouvkvaa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyhykhvo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3opknvmir.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3hylkiokv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3sircclhn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3kvllgyts.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fsurnepk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dwnoznio.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3tfamtjbx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3htpssuxu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3frvtsawo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dtbrmyph.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aejqhjxf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ncmtkxbn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fljsezxh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3klrlskyp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ipcbrppw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jccuwaic.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3abjitgxe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qlantqib.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3kjcmwthw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3quhvwmqf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zzqgkpgj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pbwonvjz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hmpmfsup.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3devojzfu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3abclospc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3biqvpdzt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpjlmgo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hbdmjduh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3thfaiwau.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uzvmuflw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3piroimgy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dpfcdvrs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3juvxlyww.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ezdoxdvg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3whgdzpea.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nvitoseg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3nqrzghzs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3orysaehz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rpbfehtb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3bsosjexe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3faxskjku.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3odlhfexh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvwceqn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3kvonatuk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3wxulaskz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfrndj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3kbhavzji.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xgxkzhaw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3igyiwuwd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ikpvbmzs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wvakjpqd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3brlpqiuq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvxdkgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vlxvtjzw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uzlsaeka.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ywiashak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikosddsf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3svlkyqtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyodpxiw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yeduxokb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3boyenunt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nudfgacf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sbjnsltu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzsmijgo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3litmzfkb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmtwjdn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hijgvisf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3uplblclm.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3nmwosutw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fqggeari.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3igjgspen.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cheswwoo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uazrrxfw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xzjdrbxt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dlegjxfz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oqcqyjtb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeowiomw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wotmgmey.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kfyxplyw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hcnzeemv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiorkyhl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdehssob.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cexilkqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3flqxyfih.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3msdhxpzp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3afpzvges.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdzwqaxr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3aewkpbvn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rvgznjbm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3drcvetkf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dpdjlwpy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kufolhoq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ctxavgdw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iqaevytr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dzrgbruq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3blnfjeum.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3omuoqdkz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3uwskowtv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izdyuayi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnwnjnnq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3vfusehse.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3emobxpco.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hsjeppxj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vfljzxof.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zuqhszix.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dnalakzk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wligzlbh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogktjuny.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3upvpzxyj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3rkuxifqz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vaeqtcto.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mftfilwz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nifalvcw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kuavewmi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmguqar.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3uxxjomyv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3watjujsg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hizhmurx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pokdysrj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3btzlqzmn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvshnm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eqtnzawl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ogohsbsq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvjgkkh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gfbbkulv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zlwjxnfo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ynmdepml.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kxehdsni.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rkgjzshm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3raytilzk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lsfurdpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooavzqks.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3oqniekti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrhfiucl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uhgzzvtl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xrljondm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rmvkttqa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oqjmqarx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hsqoyicc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mrqjaion.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsiiuxr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dpjanqrr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pelmfadj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ayqfpqfv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ecoycduy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3uhqzofkn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nihxseiy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vnwrkpae.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ctavwmar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uobkcufv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qfddatgn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ogxsjqid.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zksnarlb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vvabpxbd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3janvottw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lgtfgxpa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rhznhbly.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qlqvquqy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aaqlqmtc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wrzefjud.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wppcuyiv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iryyzjkb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3igphwmuj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vcgnbjuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dvwdlase.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3irelhnls.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3scbuzvxw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3whoovfuj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wfltwlps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vlxfkxwc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mksopwxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vgahqgbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3uxwazneu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3glbonnbd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xhyopuen.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qnmrjwmd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wvzafudk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3eadozost.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkoiigif.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ltzsmggk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3grhkqykp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwptcuk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fhqxfukc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ojaeaibr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lvlgrmvf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zabroufc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3slvvzbkw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zptftrjw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gbcqnnyt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hmqsoydv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wyicywil.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hndfodjq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pviqoqzh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qtjpvlpc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bmojdfvs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wioowekm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cxpkrsyj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3aropnore.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wxqfkpjn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tdntlljr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vkagxaso.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lnbhdyrd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ajvsshvy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lhjquokr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ladxjdzu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fbncsedr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asngujdv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lglgkbus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xntifrtj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jnrntfso.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jtcuhuie.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nrzvdzye.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ydtehgvh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3suwdcqim.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vtuaxfiz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wtxkpvfl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fuzylrpn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cnxifszn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rjkirzrl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ginmqnjw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lkrklgba.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xtihtljm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ijafqqvk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3svncyxbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ecqwwrib.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xrjphqre.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gywijaeh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fcohclzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcahirap.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vttvyctv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wbcnqjct.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tciphiuc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uaysgqzx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rjijyllf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3prqmzzdo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cbalwujx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wtlskwrl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fpjvaljl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fbsqqaku.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xypqaoik.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fyctzkys.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ouglgphz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jqncjcco.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ibbxcdjk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hkkbeodj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wkpicths.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3enlduimp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bfbltnyi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mdezlwkh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jogmxgyt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gygygtws.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vrjyiemo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dmhhzxcc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vbbjqapg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rjaktacf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rpzakpnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3arznimkp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fzcwqsuu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3trmmykro.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jolrcoln.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ljbahgcj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ozyawkoo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xwxdzwhh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pnmjpayu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3knfcvnvc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mcodriwe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3huwykxhl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3htyhpccu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhfygyk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rvawzowq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qaymqoxk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lecinllz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ulzawbxq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ihgkjemv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ldzbqjkz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3emmhywjc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ueudjufd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mchljdik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nzichxwo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zqrzhend.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uitdqzdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udjdckva.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zpesqgcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyykavbn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdtdfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wiwbefld.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxejewd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xosjubqf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3smzcbfbp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kzqarcfk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3okojplom.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kgagrckj.html


<!-- 参考信息 -->