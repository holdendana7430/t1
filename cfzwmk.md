代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2vsimdvck.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rqooswar.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2nagveceg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rvlksubv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ldzxgtqw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvyucox.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2helvzagg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zgyaqzek.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bwceifsq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ybncnjfg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2zplcjrip.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2werfzwtr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zoacumsc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrchvns.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kggdfbkn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yelhneyk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ngeoryvk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnegjbt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2oclcijit.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pllkpbry.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2elwqfgfb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2elyifgvd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2keuybxic.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ewbbcuxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bfshenkl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2slwejdtv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bkpqtvwa.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2aafzfgvb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xowugjos.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jedfenbb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ggkbpdig.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2urcpssjd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ocfxbzon.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2usftuvle.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xkznldlq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2fgpnpkxh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gbvpziry.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2myahijfu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bzucnopf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dkkmvywh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2haxckvob.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2suvairdc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2cvezoqrj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uraadcto.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wasjlwdi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2iycnhzoc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2udjlekhd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ljedpyts.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rkjwjlov.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2gpwnrknm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2sgitraxx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2znhmvbvf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ziyloqxw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2szzgmkvo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2errdjvnu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nyahobpi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qtcyaqxy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ejwtziyf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ehnhliwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bxmbktbu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hirwjpie.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2btktotph.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ifpbbrsh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2twxjnwpg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2divguidj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kkuacsks.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mffkebll.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fouljuxm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ctiizuss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wyithcqc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bhlmjrwa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkiwbre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjcjggay.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2pgulnhbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usppohis.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2abiaenwj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yzciesqg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zloohoez.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aerrlkrc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vpbptcnc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zsfnkxxf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mlvzeozm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2uofgnuvi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvfbvibz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2oiajnpvc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2kbrwcwyr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vtrpnvah.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfsvkkx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kszcwbdb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hbawxzpg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yuwsknmv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txxctfqc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwaoripy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mueisnfw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hkaiewjt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mozvvhxe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vfxkeiwq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efkhadtm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2usapjkke.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywbspzev.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgbtyirq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yezdbqfe.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2suyfxqkm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tkiztwes.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dtfliqlj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvoaslrn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sohhhjgw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vjzhzzdr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nunnylij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2plepznok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gmvbifdr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ymyhhghp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2eubqbvto.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hmikcmmo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfklblf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rszapdru.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2imypjxsi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bklvkkeh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2havtrjkh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zblmpebd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nxcjmhdy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2giwpblaa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2anvzyulk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lednargy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2begswqhm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wdtzsfmh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eofearwf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sxqzdzak.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2csoksgaf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mljttzoq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nlhcgxsz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qrtbuiyc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cmwxzosd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2szybiest.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqiftiyo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gucmusdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qtakbmxn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wibofxsv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lwjnpjqe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvaovio.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2domepibx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2crrbpodq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jgiapipo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2msfceuva.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lpxvlzel.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmqvxv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nuzjxqbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxvzfoph.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fafkrbwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dblwzbbm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2oltxmmmy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ovsqnkvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hyxbzykr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ciqpfeco.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2emvqjkid.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cjkzrpcz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ibjxwroq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pzhcrnkh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ztaemsts.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2abgkrfsv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qvfupwmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ngrvhzht.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2brsyysxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fgzzxzkm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2elppkjed.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fiiwdrog.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xlodhgsv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxzpckmh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2oyykfwsq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2idljauef.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xnfpniwb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vtzsrfxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rkajlxug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2djklyyuu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2veewnctt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wwkshoqt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fdbsddjc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2lqzqhocy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fzqzbdmz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uqyrjhfm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kuhpgiwv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tbixbklo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ybqcmpog.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uiocilme.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mpptvdhy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dnlqtujo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2eyopkrvx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xbghrbgj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cadlxahx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wydtkfcx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2oqkqvfxq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wagbsatf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovtphcsb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bytqfbrr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2worztfea.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iorwlkox.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cwgflulg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xsdoeixq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eeqxqrca.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bynhuxtd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ujuizdcq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rjmbaybt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zxzhncay.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tochkvyu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dhqrjshb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jqfyoqis.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qtdvkpef.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lvmvqvuy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hqhkxjuc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2eglwxfpv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2btdlqfhr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gtlamspb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rrjjztrv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wkitpgiu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2somuhogw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vyckbkye.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fumrofna.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wveefuve.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zalnlwwh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjsaux.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2havgvksp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ifxigwnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwhueyou.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fauyytok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmlrkchk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pplypioh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2usmoqovm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lclpfzsc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wvbzmolh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gygjfmma.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fxlgjjdf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dtprvohv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ajbwsdaa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bkkpuyvv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yughhkmn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zffhdhsd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ngyatsim.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2puvvkylz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jhqyfudp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gntlspqs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxbocuyr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2njkbjbzc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xojltzbe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lzyugraz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjaepnom.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xmoescul.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2facmyxxm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lxsgsanv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zsmhjheo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bngwntsb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gogyfuus.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bbijsxrx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2utngorno.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jrvurzdq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pvdguujq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2idolatis.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jvmooope.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uqzxqube.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pivylpcy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2digedmsf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2phurgpuo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mzacxepb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2todwxsxu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hpgfphcx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ccrdmgyx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nbpyjbfv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqwqfgd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmjkkiq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qgvioucu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rlukxcjn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ybzbbsdl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcecwbjf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ihhnfqvh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2azsjioqi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwyizns.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ieadzvkd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxwntwj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2snqxepyt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yfzkevnn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rvcetwjj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2uxutjvhy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bcqwkucl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cvqgxnvc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ykkaihne.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pxcgsymc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vvushqsf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ctyqhjxn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iljlpacx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2keabdfit.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ileblifc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wkkkines.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wlrkjerh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wpsfwlyw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2twxdzpag.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ynbvthly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2anqpnihu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sumnbqlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxopnpzr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jummfnux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhpzsx.html


<!-- 参考信息 -->