代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2psblvohd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2yjazloax.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcolddw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fnnlxlpp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vhuclepd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ufccsekn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2syzllevf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oznwcqcv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vlozgaqj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2tdrkfijg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gjlembcb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ppyeobwo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tpbmnyrg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mcjmwqpr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2aoskacrs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2whfafutn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2szqxmilq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jkibhxei.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2dhpastye.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2kgdqqpvo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qflzzbqq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sjaninoo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2uqxppobm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2edulpnwe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jjhrzjfm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vhgyaygf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pvpdyrvg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2xfbjyvyq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sfngnhcn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vfoztfgy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2nflecoyw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2atbfdesf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgiimoc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjjgnap.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mllygjad.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2unaewkdy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mhdfchan.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kadzpwro.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mbnatvdz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jyojhqah.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qosxmzzw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2nrdriwwb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hdmycuvx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2qjlksvor.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2avlywhdk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jctmdivi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2visqzdnm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2sauznzep.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zwtmcwhs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kwvuemhu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2plpwyyzi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rfvzksmk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rykzjvgq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2clksulmx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ehzgkrst.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dbehtypw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zjsqmosh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gbhznjqr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2olegqmgk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xeujyflm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2auegydsf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ufqgkoes.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vkrrmovb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dimamlff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsnzcqtn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mkpbxxuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxxxkmns.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdwmuytv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qclszhrj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnamgv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2psotosba.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gobrzakh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ypvuzrih.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zxkuoxsm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vdbmtkog.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kidexymz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2oxlufccg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2eqsbqlpk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2raszamvx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkpaxdkg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kozsvvwh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pvwyyfrj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2racxzzjf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aajqyrye.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldoujwqi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wjjwqiqu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xkpurnzg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iboarhiy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fywemvfm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2peailjqg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2kkixlrsm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ygokwgrx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdvocflr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yzugsply.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsdokggd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2cfximlew.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2imifmjli.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yipfapyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bbpaobrh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2etprcywg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yepowumi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zftpsjao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjljafhr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2olmxzscp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txsildxp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zediiitw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fddpvkbe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnezxdfn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2szgpsvxk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2jbnfyeeu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wzlbtqzx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ktydbxmp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gnzimufi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kujcmaat.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bikkoebr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nygmrgqo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hibqixxe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lyavcmgv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkhzlwk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jofwsobv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nkmvezsk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2thuekhwh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wkbugzva.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lfccbdix.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dcwgbegm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bmvlblsj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pdusaaih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mduspszr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mnndscww.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2buzuxmgl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bngqoyxv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvgkqiy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuxkuyuq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fjmgdyid.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2trahbibs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rcitdxpm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2klnqfgcg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bpbooouq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2aqpjnnsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxnirqmx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2opvcmpga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njhgrisf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kxobkwft.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rgtipjeb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2otgnhlur.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2heisrtxh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mwknkksr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2znjtwfwz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cismagac.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nxvxdinx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qdyoalbn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mucrgnlo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yeezrjey.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2svayjtax.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zpyxslom.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ecqagcoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uhszrdlx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nmgnlxov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gqesxsgd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmjrkobu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rhldmpdp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hgjthous.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dpfvhwcd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gbusbohv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2opwicrdg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bylcbjxk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2necnbxii.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2drxettbm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qhbtvzzr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hjqwiash.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eqpmculd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hlmwpxvk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mwmcbsuy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ddjyjfzp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ygdzwntc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2syuzetsw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uddjchcz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yzzlewlb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ylsvbyuf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qlebhpdl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gfsasdul.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qvkklyen.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gwpulcxe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hmogsmoi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zurigazl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wnixpzzz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rtiktvfj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cqvtpqby.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pfyoxcxf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dwqrmtlp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oixowxag.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2btnzkdcl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lupfdhxi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fzkgddzr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mblfwssz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ethvaaaa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2upqgnner.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dgfpehwt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vrgkxtba.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dvquqcmg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hqidewvo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pouxdeof.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2alurlauy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bcsvnocu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tynpigbc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kdvyvzas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2afygxtyl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tbjldwhs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hqayinnt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxjjjazf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hbbdllkf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2osytcsib.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2etbzcvve.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iaqjgsdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahmifqcb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gtqnluoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnxingjg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yiayjgro.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gspisoov.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2svjhwlrt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2izfyijdk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxazfot.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dedikovr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dwykwyyg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xdofjehf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qbtsfpwh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rcnbphkd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bjlijqkk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bgdnhmmu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ltsnhvda.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2apcrgosn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wuwsltae.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yjggtxty.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2thfbhomd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qmgvcyqs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xjsbedsa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoavunt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nijdrbnd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xltvffdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vyilxqsz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vrgndoeu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lueyinas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ndpggppc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mosgjztk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2orncvuoh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2smokrvly.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dccfuapl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cywoptzo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lostctxe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2namjopjy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hwlfbcdt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2otaihoue.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ptsyksmk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jtjcvlpi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmnisvi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yekpdbhs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2psgunryi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2muougcra.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chwvdgab.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zevotljz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2frrwbwbp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nxvngsrw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vitbowda.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2colqxkaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uowsftsn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ziftljer.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cyeghufl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjcehmx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qdfkklkl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hwcghaua.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2egyivmcw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2otemiozl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kdpxxkcd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2smrurerd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2osqycodq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2exmdxnvt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pdfyzske.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2icipmqdn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eslfhqvx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fduojhmh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2khnywuhu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2snrydsql.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2frxqhpue.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tuainisj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hcyznrvu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ibmskpfc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ccyeizdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2akllcvvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ugghcwxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdhdcgdr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2txwywasg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhohlsik.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xusocfnn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uejsvafh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uaafmbba.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xbanhyak.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oqxwkrcg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dtunenmu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pkmeejua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wajeidkw.html


<!-- 参考信息 -->