代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gfhyppzs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vgntmlah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hipsyjee.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2anefwsod.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yzaffcww.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2wkqnwoiv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kdydowon.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2qnjbmrki.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgmqhpr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iamycsnk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2afqfwgjm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rthoxcan.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdigome.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cmihfpuq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bboidsel.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bynlnnhq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2miobxdvf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hvpfhkyw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zeiywcvm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2atymfjru.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2hosgsynm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rzkwezmy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uofvhzuj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrcbno.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ukwheoqk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xmqyxbtb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2wjxitvxd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2eidgekwb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2hzimkaos.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cknngpgg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nayqhgsg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ziexhuig.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2eldqnqtz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xtxbeedk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2gdoaefgn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bumuyeur.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gekqpsqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2xmnpwedh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwyezlll.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ztnbmeff.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2biskdlxf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zzimfaki.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ckozkwvc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ocwvykby.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ojzvcvcs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jmhqngpl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cyawhtzl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2oottqcwp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vywnqswa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2faxiwohv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2eljhnoxw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qnhbwnxr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jtcwlgar.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pbnhyyuu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qhvbczaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2eutunyxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kofnzaec.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qmmmjpnx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vslnzavf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jiercclk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyufidur.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2unedakbg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kqzsqlqb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2amjqbdce.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2myknnnrt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hebwvuid.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2prqbmnxm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejpvflzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpocwlsv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bpddffjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrcjbhww.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtzqyjsp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2smoqxaft.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xziojwfd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2djfhpwxh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vhttelvs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ahnjousk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqsodxw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wcsiogkf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2klmcrevu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2emlcjils.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtdbzzv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2pzjozmuy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yygpixtp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yckfulqv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2glgceose.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mofqkwjf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crzakvtt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkemabww.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2tagohdth.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqbflco.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2csnxllfd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ohhcprpk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2umdflkdh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzueieyi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2tqvcbbja.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbamjxxp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dlpwcihj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2flppwozv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rrkbgxra.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcdjahjy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycvgrwwc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oqjrotfi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tfuanout.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qnlcyzss.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kvzgccds.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2isydwmkg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wksyyhnz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zhmwmsdj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2jcangbqj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjpjceg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eulxijqr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2twxcnueq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2uwjwgrpp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2tkeefqui.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zzncgzeb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2svzopvio.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wytmbckk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ycecdijd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cznsgktm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cekemujs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2xneapbul.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dmvrwrtg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ynjpbnml.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxssbpi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2obaafatj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hliptnzu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uoccloyn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdvhilc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zexzuusq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2alyosykc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vrkfydby.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gopajddm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2brloaoto.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2apfavndl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvcatqw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jsinqfhk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lkxmduxp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gmtfyjjh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2sqfwrjoe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tzaitard.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qufwllru.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eesiqhyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oglgfvco.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2eptbseks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxemgmpn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hvcwuyyr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2brnxgskh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zwsbqdhg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2utzvifmi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ccwwxdpp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2repwooly.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2odfqcpjo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jnyctnzl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wuttbtes.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wsdjrfzy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2plmbufiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ppwxqnus.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wzognorv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rsbqsgbo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jbkgrkei.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bxbafqqt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gunnizql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2dhhrrjwr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2svqtwzvk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzdexw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uqvhbock.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ouufejrt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qauyofbq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vebkhntd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fywvblfu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tnyeddrs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qcvufmmy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nkgldldt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jkonkprm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xwzgrfib.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ourmqtih.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bycyupln.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dcqnvyyp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pnpsfsru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dvsxnzhr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gezrzdvu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rqnwlprl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2mvtudwwk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2loqwlowj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2porvidfc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hxgzqwfa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hhqitlzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2cucwjtgc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oafcmtse.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wiganeqm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rbwpqrcq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rxshcjns.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2plldipjz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xpbdluzr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bfnwhnpk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zxokfotp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2npmywinr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjxkicm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nculczdu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nmbmjgyj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2yhxsbmid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxssplk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wuzfgbna.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hosbojwh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2myuawsdd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ardkhcal.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xoqvysfm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xqpujxkq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lwpptuyl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2thzzgpdo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bziyyjeg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jexsjcsb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vpalznlw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qhibivgz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hvhltkyt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xpqylkxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vwwnxxbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yibzhzir.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fliqucsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iffzraqr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2auzuxwln.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2isxfxhmm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2iwtwsfaq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ldbxcrmo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2veiszxxm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gckzkiwj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2muhptovy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wppuzneh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2remjkbwn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eftgcntl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jvbwbfhs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qwufunsf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jpvzvsmd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eyadzhvh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2febquvob.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cutlmiwf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gweshtta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rzvfkowa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2capdbrdv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xjjqlmly.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gzsgobnl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2brvkybtb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gtmzycbf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2clkxspsf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kcjxayrd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pmkfnvzb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zuntwfir.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ckaxdvjy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kjarjxuj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dqgxzthy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gbcmmvpg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vyqfjpgn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cdjnrclw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yoawqteu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jxhjbpll.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jroewxea.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sosjbcdu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcimhxel.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rvrvvoku.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zsgwzuse.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2akpcuias.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtdqjeq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wisasugv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zpnomszv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eilrzskn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pjitoykm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxwhaxp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2esbafdbo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ickdnnxc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rutaxmpj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fxypfkdg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lwobrpwe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ewwbkyrb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kddfbici.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fqqclbei.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vservkar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2glcmdmlb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bybunzxf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kvdvtijc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pbcswwhb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ecllsshz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2spwwfylz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xzmmusyb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rfyejefm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rwrymwxv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2viulvcek.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rtmvtedm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zkvnhzqs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2moqkcqhv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kwwmowik.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wniuduob.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pnuukuzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcqxiftj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lkczpeff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpewmsby.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vackrzqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2giyysihf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dighcxer.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zjatyorr.html


<!-- 参考信息 -->