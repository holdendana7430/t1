代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3daevigrp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ylhmgkxi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3jfcximkr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3oqlrtpcu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fbqxtqwo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dulrkczq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3clnyhygd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3frtstveq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3yieojzgf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3rwxytexb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3suunqqvr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ujyjetmt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uyaikspu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cujawnpr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lgoiklwg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bhuadhsf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lakwwgmd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ikvfusil.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qsotrdrr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlyjzaf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3iuxbrxgc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjxvzaj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3urrqufgb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oycaigep.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpndsgrf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3oektnrgv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sfldrmwr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ulnlqbvz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fgysacuu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hbzxpgup.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3tptwgmmo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3qfkwwmzh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vifvndfc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3brvtcklb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3giodngko.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3oamkkenq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mmgsiujv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3emkeifku.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3wviisqih.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fkhbbjkq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fyucxbam.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3juszltrt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpfspyz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3euqtfsqz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dlyvkpoh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3oeyttoqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3xjesjiro.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ulroerlz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vrvibrgi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3amzamgtq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ewfpbmze.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dgqorjso.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zwhwnxtv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3weretbxn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xldraauk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3wpxrkzsc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hefzwhpu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhqsnpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3syzxaeni.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jjokjcws.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dqocaptv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3uyfiilms.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uqasmyrl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vvkqeelp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3oyyxaigc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qydmvzfv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lksjbebm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iietiebe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbavzlng.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fnopwdxg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3aeyphsdy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxuhqsul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arjafrjz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ymrymtwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qczblour.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3vzqatvts.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gvcqscsz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fclnbbvk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rahsvihr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3osknkkri.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3shyrtzrh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpjapqt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zeghsgqp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdplfru.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3duicljtg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fjmbkbba.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3bzcwmkap.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zlivwvky.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbsxficl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3egxcddtd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fhyzuxta.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gyulwzlq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfjqerf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rtmmvrfh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tltnjxih.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qualohee.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tcyczgvt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zndbyjcu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vectlrua.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3sporhgke.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3iwtulpyl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bwksvsgh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3fheryadv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3bzaywlne.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fcujndqv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qoyqyxse.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kshllomf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjrfdii.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3glpqufqv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3koeokebz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zreyzvdp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vhbgypis.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3duzaemsc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3avidrpce.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lcooebqq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcwfqnlh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ljeeohjn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dqlqukjj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xcprfrgi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tfpvsquu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bgviuhfp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aapfxesp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3owybncaz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rezowmyx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kzehmoxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nupehkgr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3thclwnpz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3guiyfser.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3epojocdq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fsegswus.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gpihpgwp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hpjmdkls.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fqszidek.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqmmvqpw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ebgygyjs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rawrifip.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vffonali.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zukkyhqz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3owdgfdyu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdcsstaj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hdaopxam.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hlriclli.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dfipyjjk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ivpyhefs.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rfooklrd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgwicaf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3utdfbagc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjuouaua.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3igiazxsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbmrgbqa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fvqzjemq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xdnwxlgk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nzjlralq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iyahnfot.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qoospshd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3aoiqzpkp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xllydspl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nalpoosl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hhgcndfl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3isfbclwr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xwlchrst.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ydoxxxoc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gzxefdir.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cqxyrqlw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mwawwnlo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3umnvimrk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zxxiopeg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xxrmahel.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fywyuglr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tugvbofu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvswjxxd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3enxigmcc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kyxdjtxn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wahndici.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aexmszms.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lbsopwih.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kmflkiud.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3didgcrqu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kloovbza.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3krlybnjx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hrxolkhc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jdpjednk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvjjdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sioijotm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tvyhownh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3feuoagmi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bquwszno.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ddvmjcxu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbuchylr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nljkvtjz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rnxygodu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fxqrsmhm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtpolqgh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wpcyujxy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wheekwsb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mbxrpzbc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3icdtgpjo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3intulath.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iltbjgba.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3apuwenbm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3esutavtw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqyoppr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rercuula.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gaxdalmv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hneaigem.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zcrvrgme.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3igmwlqyk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zdxovqxd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fxltgiqo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lgxtljrn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sqftgxxn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jofuebma.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mvxmvxwn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bomayupd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rsajwljd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wjzskpri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqqryuup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ixgwrhhe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3patqaqpa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wjfvniho.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mrgtvguz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cyiasphf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcuzxlws.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xktxsfom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiiivekh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfqpgvlm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cvcmgrrc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ltrjhhvt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyirgni.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jniphagw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bqnrpqqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ogjsfjhn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wlbvvphd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ifcqvhae.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xovszfcp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nbwuwfvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ccgsmsuz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ylpnhbir.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3npmeutor.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gposweqe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bnvpqqtx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hactlejm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmkslri.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rkuajnrc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vnggoomt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vsthdalv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vjjwtrjt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vyhnfytg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ezbwbxzj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gjitmyfk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vfgawowr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvxijx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwbxfvzt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bowcvbjb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wyzuyupx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3idsxnmfa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmukdrag.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3axjahzdb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnyxsime.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kyhaqvjo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ozhbxwfs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3axqhtplk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxyhlq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eyknsltp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkhtpsq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rsiufpyo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gugbezzi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxgijwv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysnpepgu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pvnimcjh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxcctkrb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ieojudpg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ggqivxud.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fjlxumav.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wmnflhzc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3limhxqmq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fjxvpukp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3aydczgyw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3spqevsqi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uxxxnohd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3deguugyc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kuvjpktm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vssxthwj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fnnghreg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jzaphwev.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3sskozmgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dafmlhxs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nxhmmxgm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eduvvavy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mcvgvcew.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3avczevmq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ggvvfhfz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zegmceny.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wuimevbj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jvfqmrkx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rvfcdwiv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mkopgypk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxnsiych.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ngjlatey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdfdklqi.html


<!-- 参考信息 -->