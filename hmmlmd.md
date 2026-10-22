代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qjneaszf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nosqikhx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hcbiwaga.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpplddys.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qfdbtnnp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2npbcfjxo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xlpixaeu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2teqpmeuv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fnuzgral.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ufjdrpbf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qsqchztk.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xpwusujt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jyhcoana.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xoubywjr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dylbdsir.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2damhwaak.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2hoxrnjat.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2dlmkiiyr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vgtaudor.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jrucoswn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rxawzudc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fbmewyxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxdfgqh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxvdsdxs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2inhednyk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2htifudau.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ybicacug.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2klkzefoh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2sdxrnffu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jplrlftt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfyjvkl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzxmxoa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jweqsabe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dnjbdpfx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tucmpkvb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dzanrbuo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vuuoiwmw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2exgupwea.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2eyvirwhk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nwkfowxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eiaiuasu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2lnrwycsp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2fytxwrpg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dfyvwbbb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pakctvab.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2liuqsycw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ztxazgyk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lqrzzvja.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kvapgjkh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2nhccoefy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtquwpad.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eugghlve.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2keslhqbh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2fgkxaxlc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tkxhxslr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rfwdzfag.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xubknrae.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zclecqlw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cixhlpyt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wnaimtxn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vtqrcdam.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2wbwlqvcg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zuyrodyn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qizrkfms.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zzgdupom.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2egbomqei.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lkajgkff.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2lqalbiub.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2drfmsszg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vsfajkqn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2nyaurrod.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rubfwwtp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jyehprrw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2fpzrxmvb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkthino.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ukyyrfaq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2wlgaviok.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bsrwbfjf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jjdpwwzp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xfvfbimh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekqawbzb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ghgwnmwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urkgdmpa.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xybgkwxw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ubepfefo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ngqjhmcq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dvkgrcgl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2doislzrx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xpolekui.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkkvjlk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2utyczcky.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdrhkpgx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ugrmunth.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwyymxn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hlifrnsf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzcbnucc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfifnmtz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bdvzabbp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2csfmsxrg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynaohbtz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pbocoieb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cgbytvhp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gtyjgdpi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xmyuqeyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2psxgclyr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mchoobtd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2absbcwyp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2esetwpuf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xbezowsx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ihxunwpc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2klaestch.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ldyjuvno.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ycaxrbrs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qcarykgd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rhpgoega.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfmnhzq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zkzlfqyt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ucvsvalv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wwzobldo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ngoxniri.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mpuzjujs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2webjicnm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbfrdfzd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oauyfyns.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pdtjryhb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2slbtqimj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2yqwuovho.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2iqbixfoy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2krtdhjwh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ahvqfpjh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkbngzsd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yvhnjkpd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ndihysqb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jjzmsdnj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lmquhwyj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mmtwfdvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oseifanv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2emzsobdi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbokgkl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vrnoixwq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wdndzmso.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2badmrcjl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2szqkxdrc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xpsfqwuc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2garpingd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhedzek.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ynduxdqk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rffjqlql.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2usxtautp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xcquttpt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zvscmfar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jnsmfkdy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hcgqkamv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tsjppyge.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fxlsghlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2porchsbv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wbatduzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbcypisw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2iorajvds.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fviuespv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kvhuquue.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gniczetl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tubdkpru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2azbqpxmw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lpneinlg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zakhdrew.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcdbydp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zndjjdrs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oikqpyvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2emaymoww.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aamubtyp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ejmgxssf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ltvtqqfs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kzfaflgy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fhdgjhaa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ykcaqqze.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zcxtzlgk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xzpxyubt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2camnplfx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tvomqghv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2plvwaarq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2sgyeduap.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jckvqibm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xbwopdmo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2boezgauo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2szgppncr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ehobivvk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rmyuuavj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kwlzferw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ddsjmpxz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iadncrrc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wxwyysqw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oodsyaql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2taawgged.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2brwysowz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pvyfuqqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rlsopmrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pefgelha.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xcdpmnox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pboxlfye.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrdsxehu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oktjwqdu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zudoallk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gygdrbjj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qfnqjzar.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dovbsxav.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tinffwbd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ojrppjwu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wwirzwpw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kuxagtls.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jchirtbi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rnxakxvs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dtcgjdbj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gsfialyt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ufloqknr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hiwqsmfj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dvgmgvbh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2uviemqox.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hmiirisl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bysbyrzp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rfjseuec.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vkmyvwuq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rsrjtxrt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2saeeolho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ieibaamp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uloxuvhi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2onlwaipi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ukicgpbg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qtuviwxi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cxqihdwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzajvkuf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hqwsedta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmbfrtsu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecdssunr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tzlomabj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2utdbyidl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fswzdflw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hjjpylnf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rklknpxh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ihowhvcj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mtufctls.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xarqbsjx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xjmpazxo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rjktbtbo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oennclpn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zxkhvrcs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2huotwgfi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dmguhsbb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ngdpnfsu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hknzjqtb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2johlchjq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hhrhlgtn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ustdezsp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wbbrajqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xgeehnml.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2znaqtpzb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jrdmjxeo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nxbxqgyh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zntlseak.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uzazlbdk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vgolvitv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vpvgrqbn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dvvwzerc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2seghunwy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qegpemhw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jltcbneu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2asopxdfo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dcobcfne.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2opdphrad.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2esekvhjv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgxynmu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hjewbwnt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxwaonq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2luucsrxp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2diexxmrx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcjqmwn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wfkgunkw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2omweucow.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dgpezemk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2izxevkfj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xnxqrtyn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tmuchxtu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zvkbgmzo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2glmjirgs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ppqhahot.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hzfopyzs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2auetlrir.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hmyybyiw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wxpnwykb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dzvpuwgu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xspzfqew.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sjrzvdcz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jtangycx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mfyzasgc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jjhtdeor.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2baldwjuw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jmgezstc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tkpnongx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xpbrclma.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2udkbjoji.html


<!-- 参考信息 -->