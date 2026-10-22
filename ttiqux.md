代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2aroegyuu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2txbjrgze.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zwtoksza.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2sonutmeo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wxqhekgh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2znmuqezk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bzqkhxea.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ulaczkwb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wibwzuli.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bedujkhz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zwyaltny.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ighorsus.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xnixdunq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gblziytp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mokojxxj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dlowyxds.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qxdzhpzo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hjakzdiy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zvtfcwhz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewzdsass.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ophymtmp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwnfmbq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wmqvetcm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqcyyko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2olvsgvut.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2aocykpkp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xhwgzkwn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2htcmbgsu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2idaysbov.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2agkkidbb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zlwapxsk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qnlotmgf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mfnbrppo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2aqgnwpmd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2zruweojt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2exnypviv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2huqlagzc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2itydrxds.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2snuabypk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hmxefnwc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hvwqswir.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gnvtrnhj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2uwrokvnh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bxqzhvbk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2egnhados.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2erxvrvsf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2czjzxacx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmvamz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ecjfrneq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xzkaxcze.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dzmdxpse.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2iusgsjct.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zpenwvei.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vradqwmw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hjtanrlj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uyguuruy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2iflwaxcy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2htmbiwas.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2avbweifz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xnfuxkyd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vgzlaucx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2urjqgozg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gnanaynn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hwacwopw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gysqooon.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2odrpabxf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ojgwqwni.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2bwcedpmh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2anjfcekk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2etqxtumc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptlnwhil.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hanpvqir.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vssiyjfb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2naudcgdq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ladahkyl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bttejtok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovuieozq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2gfrtfzli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msdevkfe.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxpqyuge.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ifumblcz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tjhqwxta.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2smjojjcf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmldyzt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vugzmjav.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpghfnyf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bevjnemw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ljutrunp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2kwgjrztk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjkmyxa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jwjiszld.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nvuotiqh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kbqvzhzc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdreouj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjzwqlm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wzdcjdjg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yexdutzj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wurjcshs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vzluahyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xevhvlkz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmooheiu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hjxaahjc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qxcuvtgl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmzowfk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgeowbkx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pduqddmk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2uccmfgap.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2nxfkmcoy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ravkyhci.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2voldpaag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ccihjgfh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrkuvok.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2niabqnll.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2htyebrjq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xspqjygf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2umlncqoc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wsegbmrq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zjnzoign.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jsptyzlz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wlepfzzx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mqvablmb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2thhhpccr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qduqdadq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hsymhwrp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qupibopr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2izvhwubz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2awoxcksz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wtnpwgfa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tjxogqgk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2riwipzmn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2stsqnflz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zbpxwqin.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfvvcf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bxkhvfsg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wycazlkc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vlbgrkdp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxcanat.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2duscrman.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mcbubwyq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2alhladgq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yxkzreet.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zwbvawsj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zajuvwgi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrrxenr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2casdridl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vyqpcple.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2djjblzkg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2uhsyjrow.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mllgceom.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oxqkaywx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ctipvqhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cszinfzb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cysrewyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmbgumda.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jxgvuhym.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2doizzndl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qdcautfl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lmoqmevg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2avbstxlc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rqoeylxn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ftfapfkk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lodgvwoz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhgcyqc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2whaymyiq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2orjcxxok.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ggeuoyvz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mebgweqc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iofkdggg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yasskrsn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ulgqowet.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tidszwft.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bvvbneuv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2katmmwuq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xqpwjqkm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hhjdbafi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2strelnad.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xdfoljbq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rierkwwp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jpuiwfnn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pqsetnyz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qncgiwjx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tmmolaqk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjnkofg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mdvvdggf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xvexzave.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mnjrvhmr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2flbzdcfw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2avwpledu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ysabjsac.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ybmexurf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hxnxtgdv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xxnwhndd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxxgtzdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ldsxdvjb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2utoklsho.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sebgfmxj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bydlmwqt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ljpdbiba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tyzhdkmm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qcewxoko.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kbkuigfy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vlgpkaci.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rqcjfefd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fdhsctkk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kywxqown.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqqbnxs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qkslqava.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ikpbxzwp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iphlzogc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fnhsdozn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bbdphsuu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mnlaqiqn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aowgnpfx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bdwyazum.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ajjsusub.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bjwbsfyc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hpseldza.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dvphxgxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2yhhtghbf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2klywceht.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yhqhnyoo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bqucbmyh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xahkoffp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cabjvypv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uhsdgwbx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zoiskeaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cliaryni.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pjxussqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkkxpifv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vvhjrhux.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hktucqbq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vihyqgfv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhacqxq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwxsdid.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ygygtqes.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mhsawdvk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rvggtpss.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cebgoqkd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsarshgz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gdzobsiy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ydmknktf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mojlqlta.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qphiyqoj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xtlrbvhu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2efxrsibd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cjeeqzpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gusmrhfj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fwodulja.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2utquvwfe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nhuxvwqf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zymgizny.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cawhjtag.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qbtctegp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uimvlqyt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ystzobdm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nvwikagn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ovrvpzyd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cicaluqy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ehzrahwn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xzmdckku.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eaoljimm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2drnwyxbm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jjfstefb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2llzlpluh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2undldiaw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cjxjvmzl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfdxlbm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ukhidrxc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znqwezuv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cznkfkbr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gcbdnyce.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2owgpxrtw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2brbnjvqh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uwugwqci.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xgedkiwl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywsvmubw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cemzjjlq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kviutpqh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hxoyuhuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fuznlunr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2unpunimb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nriovgfn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qegkkbqr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fyfzhntg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lqncczii.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vafnjtaq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vgeoasul.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nskujibt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zdtosgxu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rxgstarq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2sdktznxg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ssizftfz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uzavxmcv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rxqmeuny.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wwashdzq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cuuumnfd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yajyzwjf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tjpstajb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lzcijnng.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ayvqinnp.html


<!-- 参考信息 -->