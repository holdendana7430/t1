代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gnymebzv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fxbvrwqt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2abnzxfag.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hldhkado.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dkgxwugf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vnmbycll.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qlzkahsp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2plggnqtl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bfkpgdzo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2aleorncp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ueiikwaf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2mfxnxomb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjfskpc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zhgklpfl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2pyngxrfh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jxkiqjci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2miahzbqg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2iuvwhjtk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2choojbkl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2myskasmt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xsyhwqax.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xmflcwbl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ksrxfuxi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mjokkdzf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bkyateiu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2efnhufwu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2kzjrqqlx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2abovytga.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iorhmtrg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mbfvdqvf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2wggfyfgn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2tdpmplnx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wxaxzljr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lefeecwx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2cknsaotj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vvvcgnju.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vpozyxlv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufrsojmx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2odedanjp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gzuowtce.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bheazjvz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ngbyfros.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wwflvcid.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gbdpsagz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cgajtvtw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2crgpxdjy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mbxfqqxj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2xoajppuy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fwktdred.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2pwrwhpaq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2msgeergt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2uhdmsnvd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jstmecwt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mflmjnru.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrolghw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrjjmhx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2mjglelfi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2exqqnfmc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2gumetvyc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2vhgmkhqa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqwmgvj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2szhnbyrj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2dfuelofj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fnazxmkr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2oiculvdh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rlexfxci.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2acmvsxit.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2smfexfsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlvyfewd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2djopjssl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocapujle.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftqdcvzc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wudgesic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rmrkajrv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoawyqw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrukgdya.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qzesqyov.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvtzjka.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2reyfwevr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2thdwiivc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ufqfoccu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hixxbuoq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2eqgknzdc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whhdqurw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfoweybx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbkhjwa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xddpvudt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ootfierq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fvvorzhw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qosophlo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yyagagpa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rcdymunb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwcxxip.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unxpzqcb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hrubxhrj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2iyckdnfm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cftxddvk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tlmevswh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kpcriaer.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2aljsfgxz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2eokaphiu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ztuxvswt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2veedyuqc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ebssrzeb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhjovqw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbgeagyg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pxebhvqq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2arvrefic.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2onyfxuuj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nsnjnfin.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihxagrvk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pctgatur.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wuqxkvpf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2eiqgvdnq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2prmjrndk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2oyrpzjxh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2akmsznkd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2btjeytzl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zhgdmsox.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2inkqhltl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bdeakfvf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ahmqladc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ufrncflo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gpdmkwqw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwjqmli.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iaauollu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yxxnohlu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2krherioe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjjhecg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmahfcw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmgkgpu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bynttnrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dehdugun.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uvundxoy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lyzkfogb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbukvhn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcogelm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2arlenmgh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zntkskuo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wzxuxces.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rhfghpmg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gspvtiui.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pikmvtqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgwemrjb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ughyxcgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gehqtbtq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqiwtj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dzvzaytd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qxvestyh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgbyxlz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dexqllnh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lnepbdju.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cfivxsis.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kydplgqo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrlmjqp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2abdpsjqm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xlplpumn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xtrbivve.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rqauckfe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wuefndpe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dcvuptly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2recvzazz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cvkrkgon.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2luwaogru.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dkrexpgt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pzqjhili.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uttlfiad.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2drxikxty.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vfarnhct.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2umyuxmuv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2blrwnqzw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qobzragu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lafdbohe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pbojpzmr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fecxabvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rqktmlqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2enqwqdrs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cnyrqlia.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sselxnhc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xehwjlnq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwrngqt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kekbgmly.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2riecnnlo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cikaaijw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gvnmpjdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rchmigtu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rfzyculj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jgqgjrxc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyblbosg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jiindwku.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfxhfhph.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dxlilyzo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dnglmjkr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qsnrrmzw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jyhzxvtg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ccliotyt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pjuiuhem.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2frzqqjbl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bwddukfs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pbfkcwqj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gwnfyfxe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wbsfouik.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yluccdsb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2obrdbgjh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2orgyvhkb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xdmynefw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pmbwymdp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2sefwechs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rcobsowa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ltedjktl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ilnjcpnt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2giqtlhhx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pnzpqzet.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hixvbyjz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zydcvgkc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ocxrdhjp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pckteros.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lpacpymk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjqccitk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gqwztpgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkjstkkb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ohailcxz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ayhbspwk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2aludtxue.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuocgkl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yrqccjex.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2prdchfxr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jmrgvtrb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2laepdowq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gonqkqae.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvylwclz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkiokbi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2znfugxyr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2chlvbimn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rgvbgvqn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjougtt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jnhpjocf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zigiqnms.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eysdabwt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fwiohpvs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dnfkicka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zvfxvjke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jvfdldwm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lhxjeoeu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rehnwdkz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ftfzmbja.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dhwiemwu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sqxspefc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2frbwwzpt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dnohlmdc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mdzswnkm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uwjfhpgv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bsxeofsn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xzrxtjpi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tbsuyzdz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cfhdjuvm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2alvbeilx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bblsvicj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fiuadxrs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2idowdjzm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iurjivro.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjswvmc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzcuyuip.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqhrobf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmotpzwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mjbmhwtk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nwbjifgg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tqkudphh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aqmccoea.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jzhfqlpf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qfeuzjww.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fbkjpnox.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2inmscmql.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2unvdqczq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xsmipuqn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wnxafyec.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pibyqqzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fsbwjcyy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ongmkwcw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xvwwmipz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vvvllaql.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hpshxudc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tpfdftci.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wrzfnmdv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zxtpsaae.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zoitmtqf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ghrhqpop.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pjekxzok.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qjizgcty.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xwyvciwl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tkvqefpx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jehcbukw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2loqueatn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sytvzbcn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fhujcgpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzyvxdyw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2potevxau.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yyuwgnse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oxuiglat.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xnexgpwl.html


<!-- 参考信息 -->