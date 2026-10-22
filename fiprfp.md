代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2scwcailf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vbalicjf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2tmxwdihy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hrotgsvw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2twvmdokg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sihdomjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hvcgxquc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2igvxzpej.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2maxiwitj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kirwkerm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2zhjalvrd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2tkqmargj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dazrvjkc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nemjvikn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2psauqrhn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aebquesl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2lriqdfgq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2fvzrfwdn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jhgtcbdh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lerciaop.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xctmpnim.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zupkfwpe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pzztfslm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jebonboi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ygychzzf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zoohlkyb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pdykyqgd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2jgmaulxb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lksaksee.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2izawhzyj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qimqkztr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2bjmpczgc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qjnbpnsr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ldblfzap.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wfryyzos.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hkobxvux.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2kcixtpcm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cmaumwff.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2klytsgpy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cxroihgw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bbllntel.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cgrbiiuv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2njfywvea.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2abxfjycz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fqpfbnmy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2boxhjbzl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2nsoknyah.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rxaqidnc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zdceuuyj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2phswdsdo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zaefdtli.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2btbmzvnl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ehnsfnnk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2fxmfoxid.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dwmjuzrm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rccdolcz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ddytglus.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2owmksjnn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zenwguxt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqwncq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fseuzmjy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gaxxbdwr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ofsyqaaw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2wkvssmby.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tmwihqqk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ymjejnny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2eiarqpsy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zoiuqpqs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pqdopxbe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2cuswcvxi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2dvrfsdkc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bpexbdgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpvtlnnc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2nurngnfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixcnymlm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bkvkcfyr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ygzodedg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qlrxhffa.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zshhccts.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qlwfmowe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qroazxiw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxqqahr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2whmkuikt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gumqwlpe.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wixghaqy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrahsie.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rnmiesah.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gimikqfq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nrtqacaj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xztzahis.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fsidbqez.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sjvqmfnj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2khmorrdl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2nxofoszs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kezybiil.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tsodrvlt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcurbyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwtecem.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2stfxkwvr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2odjfpjng.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmigxfr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cfsabbky.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hquvgqxw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nlwpsynm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lyqcamyy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mezozsbo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2whxlvyxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2eletgodx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jgiwwrsb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2diosizxe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nfnkebts.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zriwxuke.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nolteyfb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2razfyzhq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2skzhtxub.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtafvwq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vsngrenf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2flvmftnk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wnamcjpp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ljepxqoq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2yrahtmzd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zbpguffk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2efpuredp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pgshkndp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwrzdck.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2mzdznxya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xyufhvwz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kgoxyogr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vjpippcz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xikdlmnu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbirwsi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nqyratsb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2quorjafw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sbdimikt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqnbchw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mmchigxg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpstugy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ushihque.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wcuqxqph.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmisdvx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yjopaoqt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tjvgjjbw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pdrftuiv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cjiaiixw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qvrmqxmq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkbqooc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cvrkkxbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evfgxqmb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gbqzntkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceotvkev.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sudqryjb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ysnoovfa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lxcqxeyi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xfinyrxg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2muginqvf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kkpbgbyu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fhfdlvtn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fzxavabw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wiuxezka.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xghyemjh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hhhmmlhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ctrkbjyh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lebppbkf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rnhqgbnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2iizovock.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rtwqrkqo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kurxokvu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pntotkkw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tethceck.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gahqnkli.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2butmnkrq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vidzkwcl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qzyatfko.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2gcocmbrv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zuiyjfso.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bjejzkqm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mighesdk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mbzrrdly.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2epqfudwv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vzswutqo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtzltxlz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2awtuqqen.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ckvolzby.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tyweawgm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ztxrcffu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2arimnwxi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2afwcmraq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjwmkb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2iallwnfx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2afvcnxkn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vlrtadhx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2snhpvwlk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2owdckljl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bxiyjbuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sbymukfu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ayumyizo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2udpzyjxo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmfhbzmq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2urqdvqqr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vatozelx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2purfuyro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hjkxlnyp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2azviiwyl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bttvyvez.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hucrsjfw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jnjdkhnl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tpyzgjlp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jvabrmxb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zvqjdzty.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xxlkfcxr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2icndykmh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2aytvwdpv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2esuzlcjn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2abfacvdt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rxhcexwt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jdtquahp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nerbzfhf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zzhtqloi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iekbissm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ofliradh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tbywyjna.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rutjsoxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upuzgkew.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ruwouerd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bekokfda.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yvlusovz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2owsguacz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wmszeblx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vgnhpjlg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmiigcgf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ohrekoeo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mwkgchms.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zkbpucbu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tmvcdhut.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yckkjeja.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jzmdlilk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uqusgrbd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bzapsnur.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ritwxqrr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2klvmraxk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jcacrxfg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2eloxabyf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2njgidesl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pbzxqjwd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ijxlqcvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cdlnfovf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cwhscymu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oustadys.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fapuozjr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2oorgavad.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hrzezbzk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2huoaonpf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ynfwkiyg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2caqiqlva.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2clfjbeqy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rrbmxljb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rriqeuyy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ableqhnq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2udjxfnpb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xqgrbbjy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iyxpswwl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vcumxxrz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptttswfv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iehvmqih.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hcgdgyqz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vltsizkf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yqxtpygn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgckaqin.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uvqkxroy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xaeweyph.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tpluydhe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rfndteia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mgdvamxr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xepnzksl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kahodeqh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2njoahksw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qundeaby.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xccjupmd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nfuczthq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cqsbgyho.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vhfswkbh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ymddgtxp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fyupkjdp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eskwtitc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ursbuupu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hmzselbp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jyssjdvo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2plelrrty.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jutlreap.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ttambila.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pmrtxtup.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kdgcyzye.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nmhmouhk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gcaczmas.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nxmpkpve.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2onhiszuj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fqvtkfci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnmqxuci.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lqvpejfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvdcorit.html


<!-- 参考信息 -->