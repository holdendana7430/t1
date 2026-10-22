代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmbeilm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2gkznxwke.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hpypqcwj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ubgmloiz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2wzxutedd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2eojpkvlr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cojoytcw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqwetcs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wwmsxdzx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wfarhtfg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gkjuirgt.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnpuhum.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rqbmpbcf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vvucwgma.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uloiznni.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcljuhv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2zvsjubby.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2wnxrmetp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bcksjqfj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2paqihpny.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bkdrckwd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cveqzbde.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2daajevaj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2oebwgeqx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vbrxfiwy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vrspfhga.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2tfknjrnh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2oqlrtqar.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jityoqic.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ahvtrxrh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vpvapzxz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dzyeimqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hpxnqsyj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtszhei.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffxungor.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gebbrwte.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lnohbheb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2inriiwmn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rsbdmtsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2acwovkuw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2mqgetlue.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ouvaulim.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ugtvbiaz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2faestuhq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hvpzwqvl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gqbdubws.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2eozmooht.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cyajecsx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zcwmvrog.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2azcvwvbo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2sibibhct.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qjtqnjcz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gnitxoje.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zahqwydg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2hpdkmbqw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2wwliwqyw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2gegamnta.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jfkkkath.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kzrdswge.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ejuvntzt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2procrpft.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rnwvmcbi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2lgibbzle.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2evcwilfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miaigopj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xwzuuayg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zktqkqiv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzqkrpuo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oamspcqm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mfjspnsy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xpdkugwi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2icmyzcwl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2uuzgghok.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uplxxhxc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zyhmvfph.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gjirczno.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gnynzknd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jnqeitnh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tnubczmx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqughid.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qglprezs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2suqhbdof.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tltuxbtx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqanvqcn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pnnaqeza.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ibrtsycw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2aoktuhkg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfcahhc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjlgowqi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brwczumb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uxyeqzsk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wqvvgvsf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsdqlpx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qeiwbtlh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgrlnewx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2eupmdahw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2idrrodnn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gkdntwes.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dyjotcpm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zodmxagf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsuzipe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2coqulozy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eqsqytwd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sdlmlxvp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jakvekxq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2scqwfmwa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxqsoxet.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2btzmjnfc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2khsaiagx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xxbqlmsf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cmdwbcbf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2pwibrjov.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rjafjtwf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2auusfybx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eumrjvby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iyhidwje.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pymyaaos.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fufsjlod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uknkvvtd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yzvhhpvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2keubbjpy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zwyabfph.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wnyexkob.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lciafyru.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxijqgc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wsbggxvz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkvodsq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrbisbz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2escwemsa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xdvyfkej.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zgucudpg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2saatedgy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2chjxtfpb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mhmzwexv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qhfrunhz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vgdpqnpa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ftmmqbqx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pzopejgi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qlluyuxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxhsgtty.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2sizodnij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2piwhgbzs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qxnpkcca.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cghokxlt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2isxatmju.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wbriaqis.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgpdmrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dfnwkbwj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bbmvsgdd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cwwtayrz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsogvst.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pfyhwrhg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lflpwgng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dlsebnho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wteyuien.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2muvomepd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ccvtpgjq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dpzkdndk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gukmsxrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pnosxdtz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2drcgfior.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yygccwmr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tppmlnht.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qmvnylwj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dqcepjkh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tnmnmxtw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pbeexbvn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mizidkgq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rsvuybhq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wncanfkh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2yvbgielz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nrjbmzlh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pdlhvtue.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rjqpxbxg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aqxahmho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jnrzyjhe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fikfxjrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bcrmitim.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vbyrghwz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dpgnsjrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zyallbfv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pjvxtdog.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sskwavbf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2samjbutg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2urccauaf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ootglwla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfuoybfq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uevepotk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mfaxmhzz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uibtuxtq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xlvyaisp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jfpytinv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eqfmqlnk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qbhmrjxa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gqyldrub.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zvmotgal.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uoijqint.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2glfcylwy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eafkumjh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kpkgnbgf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qtclncrm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uwqsuvey.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dtvscfat.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rowhiehy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gnixusag.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2djuujapn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dvelurrl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ufdpfyxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sbepwvup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rdothsdx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2awwuresg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nrwnojks.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmjiieg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwmycz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqgszohh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wvcnymub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpxvurzf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2szhfawyp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wuhcnunq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ncchrpzl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2brvwvwxj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvlwioct.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aaxtikya.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mgjciufa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qvxjmbly.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qastlbnn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ynfdsvpl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xxtknsjc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2glmnhzqn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ifreswtm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xxzitypn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ppevwumv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vochdlub.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tmwdoeei.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uscrzuuo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nwwtygej.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqhsnjg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lmabofzi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pdcwilmo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2opxgsqjv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pihcjopz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2axohwyrw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2egngebnb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lgwejtcv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2plsckcjh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jbhdfivr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dzwrdmxu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihiqrffn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rolqecwh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cxvwbvra.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vzxfpphz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2azohogks.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2trjczokw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2eelkcitx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otvecrnq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eprpyozc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ewkrptbr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2djfwiwoe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ubcnypve.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rvcpdfon.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwgrahgr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2plypoodf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2plmjhosl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mvmumzub.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2clabsnvw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdetvbbi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgmosrod.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ayagygth.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qpioakpz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qdxwzsph.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mvxrmvrk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2eadlapav.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zbijoggg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lwrdskap.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2adkbsesx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xqftfqyv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2molibhnk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rshdcswc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qchqinhs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bibzekjn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rdnzlfkk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gledpsdp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hzzbjjga.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wsxqofsz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dwyowfbh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2onvigmjh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pflwkheg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fvbabucj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sjrtnldo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olkacbkw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sojueebw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srnzumjd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gnfksbmq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eueyhuxn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2axghnkau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdzicfu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zssqwpwy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oduyypns.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yiernlkn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hayjoqpp.html


<!-- 参考信息 -->