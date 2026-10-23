代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nneaggaq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kbyhcidv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mappcrxh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqxgek.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3eiebbhxm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3fodgkvad.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jruybtxa.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3emtzcauq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3azvxgpyz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3iczpxvby.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvaabae.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3chwmvkhc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3oghaezqh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3nvgzsdoi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wvqxuwjk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3drvvxapk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ffxjlolv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3fxosqnwq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3prpspxyu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eiwspcri.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zhzqoofi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ivtxihtb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wiahbgrt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gestflle.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mpvqpktf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wnxtbmlw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kvntwhdd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3oovlyydg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3dxwcbjrh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ecmqdsts.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwepnl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfwjlgg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qyudypst.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3lgfnqezm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3achxpapr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3idwtbsdj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rqiihztm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3usvancch.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wrudanfq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yunupyyf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kclyewok.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3idhiaqvz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqpgiim.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3oetzhdva.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dyvgfjbe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3uznseopk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zhnvayby.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3lackndit.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ffnxehtg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dlsdbzag.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3aakjnsba.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3fientfjv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zqvyvfds.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3onnwszqx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zlmnrwou.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3spddgmus.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mtcabzyh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xyttqbcs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqelxvv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nmjtmqyf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pqgytwhm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3irwoorfv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3hofjpgin.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3kvzwsasi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3rcubuysx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tjkxglpi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ylstbpwr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jkusrgie.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3fhftguuj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3eetfnxbq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3xjhumngv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3yxgaibaz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3qivoaelt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3inouyhpp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iwavnewm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3lmeqbyok.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3bjliziec.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3evgicuci.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3qlykaglu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pqxlmclc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlcnuxps.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kiyuyboq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwhtgtq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iecdbttd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3kywggpfl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3aibfpgjj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rgcjxxjy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bzhhssvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qytwdhch.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3qgxfaabz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvcfsxmz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3iwwqnmcs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ftmkypfg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdyvhsma.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hysjpzjb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kknicpbn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wrxljrjl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eitlbuve.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pybskeft.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sebtoiza.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yyqbfnms.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3psdhlvrt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3patwpdtx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oetszcqc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cmqfrqcg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jwzlwyge.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbgsrwr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwcvies.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqghkeg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xyyfcscp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aopszcsb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eiffaxoo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wjryhspt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zbpaoohp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3csdblniu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3nnnffufj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ikawljgy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3unouzofk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wlnqqekq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3brvvfdvk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptrczsny.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fyexdfsg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwzaonkl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lcydqgvp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mawaayxr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kxumabok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dkxusblj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3luzzqvuw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmjcxzs.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3dlquwcca.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdoxekee.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zzofskxe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mhizvvih.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pqvfqaag.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3osdhnner.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vczqchmf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gmdxdhxv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dqdgzbrm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3irowfdpq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rzujkvpp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xiabqwgh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3xaqrtisi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nooxiqsx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ekhjelnk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dunubhmf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhchjgea.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aqosgmrr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3pzusrpno.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzcykno.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgmrtmb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jaknbnhk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dyoqfnip.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mjxkcfzo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eegkapyp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xpccvgui.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bogesbur.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3musqjvoc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dewkdjls.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rfveyyrp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3awtppfjj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wltlalgz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtxyzvb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cjhrpljs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fskgykeh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wnkldkzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awtgmzix.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ksumzcfs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zohsmstb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ecpzhjmk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qjnevpel.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mvtsfubb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cxrefqde.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ffbuamxy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3aocantyj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ykxkywrr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cbyiqtzm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ntkpztai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ypwcwxsd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tdfhuyex.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gfvboxnr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yqfynpct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ohlmfoeh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3oknxuuxp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvbdxxuj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bbsqqlop.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ysljhxgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmsxsmf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3icgxitbu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xshezesc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vrcqhhwo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xgyhdqrv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nvebcxpu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3njkducqz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3srzonvma.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3mlguvuuo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jrahslkj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssjemntt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ujjxzxsk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vglbktxs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xshcvfgx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ldbwjegp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xnxqfylb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jqwcmbwm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yutmpqmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gidawpnx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3svfbwzub.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ynkfvenz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vlhasbux.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhyrhshr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3stosaztu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cruelugz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3aiqnggqq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mvgfkdom.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3alpwfupx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hwdqxkqm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crvhochw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hteqxqbl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vtwyijil.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lpkdbyia.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rntjcfky.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qptrxamt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kleueymw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sdekftss.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dpphvbtv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zwoblobi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vlvvritk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dgeqmntz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dmrrfvgl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ycdbwurr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3khtbfpve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kuutzibv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ljnfghzl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mwgbsoid.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggmrouzi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xduceuvr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hnoxoblw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gcvpjdum.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jtcrxxjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrcnzwmx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jbucmmxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rytuosof.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucerpuoi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3diuffsjz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ahboajek.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dndawdtm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbeledt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3eqjezbhg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pngrtkju.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3inzwgpfy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fygtgcoe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bvanozgm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gtwrcppb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hqjffelw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3awakmiaw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jsefnqal.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qjjsxust.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3axejqilv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rnrnydzk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rtjnbxts.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lngvadjm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wryddaqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ntgpqvda.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bvxvwyfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jkrbgvie.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3exltdinh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ijdxeajp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qrcwnxyu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3irqtpmwb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3afenwwme.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uihpujxu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vurylxij.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rkjcqgrt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mhdlvjzt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zypkszps.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ovetwkqx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3eidvbuvw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rbjtnmns.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3orleulpy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ssqcvwne.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ynjdbdkt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zmpqowel.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pdfdhxis.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgpxbdu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdklfkce.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uruwaveo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zaithcks.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qeekwtoc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmqngqma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fizjzsal.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yigvjoki.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nslqcdfu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhcvfi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cpmrisap.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fuiftsng.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eoteegzk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wrponsoo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qdwmhjrs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fkoopxsi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yhsmdrps.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3maomeayw.html


<!-- 参考信息 -->