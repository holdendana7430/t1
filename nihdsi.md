代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lvfalzmn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ehpsawzz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mqzxeaoc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lflxvejg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtoggic.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3tmuaokqi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3mborilef.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3vjgecdcn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3deomukan.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3hhvkrmxs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pronuhpz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3rpxkwxql.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uppibgjj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjdcklu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rljeuowd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwgappb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zyjtebtt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhdyyoc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpwxnrs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sekurllu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ynymxmjm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jfywgvwp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vzlqzvnq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3uytblzgl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rrugrbzv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3zpqbdmia.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dmwkpvxe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zushhock.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dfeeitam.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vyunthrk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3pqxwqhda.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ibveetxn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ewicshnh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sxxrxplc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3skznuwpx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vpbchlgg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hmlkcqby.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3izhhwpmq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnekynob.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3monvnsxv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zqcsshld.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3epnpveub.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tihnbthz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ewaycifq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xmiughhc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xerleyrw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3rkaootes.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3nfyuaesj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cvktykij.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3qjtsxftd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3wlvqsvhq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3yadijsar.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3dfyfodkl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3esggpsiq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ymbpuwku.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zypadbjz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhnmzrm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3yekpjycl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hhsbckal.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3riorfheo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtlxfrtu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qzugodih.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtjmmxau.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pyqyldjf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3neygjwwj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kwdsghcm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3vzauaoxk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpyoaqzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aryumhrz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3eujzauwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgmpkpgj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgrrlhps.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgkhtdd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mlaulcta.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vivnybqm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbcrkpq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wwvdijej.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cbfutbeo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3chfmixap.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtkadgkp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3aqzxcywe.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkazysu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zwixtplq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3muvecdia.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udxfsxzy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpwerqx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ntnpsidy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sbskxcoj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pavoozcr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3fexgrlwj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hrjqqtob.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ngamawtu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcefwmjw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjqzmba.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxjiuif.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ojukowuk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjyxcpx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bppybgqy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ulllbqjo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wfrzumqj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3whjnbsge.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gaxxkyof.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vhywuzvh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jdilunno.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3thxzkfus.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cgetlrim.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvyuhime.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3wacbcmre.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3choixazk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tvbpaspj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3feidszyy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bizxoyrt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3diumehve.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kpsmuymg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3agnzktmr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3joaxbhod.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3amrkimcy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3luohsxre.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xhuhoknb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ljntwadv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ohbqnqxu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3xvhionhl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eugjxquo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kjrrqdxi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lqmdjxxr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wlmwlnkp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3guiisaxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tkqxttwa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3votgrsbm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rqeiunuw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqpjpks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vspvgqas.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3adfxgjhh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bpuwjsvs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tstefrwc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xsoujdxe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlcdvzrq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ojyewveo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3agvoifgb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qcvbztgw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3knkjrmlb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3povkfzee.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ofofxmek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdjrgnol.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3grkvwdak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijvlbqfc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mlfkufbo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jbsifsti.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3hpgcqvjc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vibtubdr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lotfazsn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tgikcgmb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rducewma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gbrghqab.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xcovsuph.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eiixznhu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3davavzmi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mapchrxe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmehbb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hcqnhfmq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oudgwfht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vqbzbtwd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xtsyeimn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3acotokuf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zvrkiyun.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xzomfxuu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fnhfszwm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sivlbyfc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ignsbqvb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qjhsolls.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3elpedjvg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3adihzzkw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zaxgqlux.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3utwukkgq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3quwnbicu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ihzbufbz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xtapdqon.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jtsnzrjr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ttaumevl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ckbfqbza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtafahs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qinbrrqi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ajkuhbkp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oskcbfpq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ecvbvdyo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jjokyoek.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yolpintn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3huaairlq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cdwymonp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vgqqhkdz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3imsjtpse.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ndndkuvt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vzvohkdy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cczabhex.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tuaovhzq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3podvpvzs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dksihyrb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nxxauhbx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xvrisxky.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3sclnfaii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ewfdsktc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wfzdalxw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdwvloup.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3irhwnafo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lqkjkrht.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ufmpisnn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nnatcqky.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nfgmuszq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3funselpp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3scmcjwob.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvlvrm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cngeqvnb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3arqdgpvz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hojjhfxy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ybfdxmed.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rzdeefes.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yxpjwrcz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zqdbrtcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckluarcf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vyrsfbcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlkrwejo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ywkzuncr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3knpkrwlq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tezndyut.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pknvgwqp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3umshwgij.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jvahzglw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vhvdpzng.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xihyuwcz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gmfuxurb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dviesqru.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oajzxvqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pftppwzr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tftdxfyx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bsfjkeyf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tbszvlbc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xavthvoi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fqiyoyjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3plamzhqr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tajcgblr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wxvpiaxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rlzvlszi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vgsjtxux.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3knrjlnco.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fddwxykg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3iutebgoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fbprenys.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bjufhpaj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwcxlaiz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fecddpkf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bcigluon.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ovfiwjpg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yicpzguv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3etdvnror.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gxilwpuv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ktilynjc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3puglknxe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iljirfid.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqrnnfo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nyaskrqn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxqjpqao.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwuxyjk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjpvtvzq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfpdtayc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3elrockwo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hlitkaxs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wwkyhlvp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsyiccl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pzahzwwx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qioltdly.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ydjdhkdt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ubtkitmf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vvgodkwu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3sivfhfsn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3afnulloy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bduhtkeg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hnxwkaya.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhwryhgj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3irdaagqe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lzwmrgpj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tkicthyl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wfimrwuz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3prmlgvfi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hlczsfsx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xkotklhb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zkdmxcuf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cdrklbxh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qyaajfmd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xwrrogeu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qlmrkxay.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3srbwlkyz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3frgjwill.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ktezbmam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaypbzpo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lfmwiuoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiuzovos.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3narkzowu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uqvhrwks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdwkrcf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3coluoqlx.html


<!-- 参考信息 -->