代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dyzextlx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tzegjjbh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zsllkqfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2fsgmwrxh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2fjfnfbze.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vdtdherh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2auaffrre.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ctqiojuk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qnpznkrf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2hczodypt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jwaatahg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fpcnaqmc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ywxitwou.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zehukbpg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fxrjeajj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zjlnzhnv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2czekeple.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gxykbpbs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oiehatjv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ezrkwteq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bsmzxant.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cffehega.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vgsnmajg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjzprdbx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kiuscety.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ldrccnoy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sstddfsf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2feoszmki.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qqconney.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eitzybvl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvsrjcu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqcigsn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jeyesibp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xijvmbqn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2taicfypc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2czhcwscd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2yoejxdyt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2bdfeilem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sdiataho.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2rigypiiz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mlbdxncy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2zblczyme.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qaymskwt.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2iczbekvz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hcwlauba.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dhwtmjfn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gwrokyiy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vmvslkzp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nhoewllv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hskhsejq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndqrtond.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pvhpecdt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ifxaijkp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kdbxgles.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2diuxmmge.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wfbuqpdv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2prrkgync.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2owhwakpv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rlxyixry.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2uxodzfge.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ywhrrdtb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ymefckui.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bdwbvuml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2oheixxtg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2eegddhmr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfilwch.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2opjotgve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bhqzomeh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2irviints.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2vwlplvsh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kyokxtto.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dutoydny.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hturlkie.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ruydmzds.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pizkpytl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ornhbnhv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjndafj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bnqqgilu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2kzsxrfcu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjvbxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaquufbk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kdnldyku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmpejuns.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjupzawg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2icbqqgim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vzrxrjbp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krcwojfr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2lwanhunh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jicftcuu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2urwezpqz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hdefdrxw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvhrllac.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2sgcwppae.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auutflxu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2gprpakel.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jagmykhz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtsynutu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xspfwqii.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2arzxlpcl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zqdjvgjs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pvpnnega.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2eyivmmuw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mewudrlf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hohcacdy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qnawokwq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fudfoxah.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdbfvb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2kdmlngqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbqgnnjd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lzplrbau.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2aevvgvff.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tvsddiei.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lzwuiawf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xlduvmrf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcnegavc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zjeqeisx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvfmdne.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwwutnpj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfgjdxcs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2npncocjp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2llipyvuk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rqliireb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgtbhpcn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2shceizla.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ngmjcxpg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2aemstfpw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwbeso.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ymuwcflz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kilmggsk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pqgronaz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xrludxxg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2reqluzgy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uuktwojr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2grxhhhoq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2oimljtme.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bcgkvvix.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xtyjginu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzmaluyp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ompdirkv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hceyzcgk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkejvxso.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hbftzxyy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jzlscwgb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2icjkcvjt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhrdnkf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2powwcctz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uqfeejtd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdypwseb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tyighidl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dexjorik.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vplsahnk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2veqywuil.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hzjibmym.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rowrhblr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ovbojugq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idpgcxps.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ipljpthq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loanjqxs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jqyqbsox.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wpaimonb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ahxouqtp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qhvabgxc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hpvamdfj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vzjpouwb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrjcxrp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hzeozdsk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eekehhmy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wrjdzbnd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iikproua.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2svnodgcq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gkrijftg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jafnyepv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bvhiyifk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2aruplgms.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wrptcfvv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xevosnrj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zthpimub.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ptoaowne.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2llgnelwk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bjwrvcac.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2drgdtznh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dnelxqts.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hvmkqppo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2brmvwwkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2axhiuupg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2cgioyaqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgrjsjw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hghyhsrj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwcwqh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nilfqkuk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hsrbqaeo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hxgfkqlk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2cqbjsiac.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fixxeccd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2iuhcciot.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rzztouyk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvhjrvrd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bqtsbcna.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hsfhbtmw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hxvdsseh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypketmyz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hvoykexm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xbldtbmj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ljderryo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cwoaquuo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ltkrbpql.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vlgeydgn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fpniivbi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2knocenmp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jvjplxyh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qmziczkg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wymglrjs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ykwjfvhm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kijkaunx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dtsajhqp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jkxolnjx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ifdvswrw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ldvubzjy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ypcyixul.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qeoybrtk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eetmwzwj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hmjoxkwl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2oiqseffo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gljmhndc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2clrvlfly.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2amykbsbg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nggubuwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ixnpotcd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mowvearp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mzbdfhog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcnjyzaz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uyoxffpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shnetoli.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxafpxqr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fvnrbgnf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nqkkgbem.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziipsdyn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxlfblmm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cddchcnu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jqkoeuvr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yptcgnco.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uzsmomki.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fpwozcov.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cwnvptzn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzaiiwn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ucaluwlv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hffzyrij.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hyvrsiwj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pyoemqjv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gkdvdzek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zrxovopm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2iuqfmayv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2shrolefe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nlhzhdez.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ipidvijx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zbmmvwzp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2utlfurnc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xthrfsmv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yohmyhtx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dcllompr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2onjpxsfi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2owwenjac.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rumvdugk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wfqfqhbm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2phqrbyem.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xjbokzkx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbikuvwc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lulktyib.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kebhslfe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2egiyzmri.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nffjmtdh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2intmybnk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgyotpue.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cfxolrzb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhiwdbvw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hzfmpkwa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2urwriubi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jahvzotn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2esxlzynv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fntdabdp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zffxsakq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mvmfobwd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2svmhuahb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rlmhbibf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yrknkdmj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ldbchzdh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jriupqix.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ycrwhvri.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kalsyppj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2candasep.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2udravkes.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2svirqtxm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pkoeihdm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2foywwsiq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gqmjkvke.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tuhwmfdh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kvaqsamo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2oxkotelh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zoojipoh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vamamzgx.html


<!-- 参考信息 -->