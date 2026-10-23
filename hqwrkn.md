代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pjcrtpxw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qvqmcsev.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qjshescw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3euxqnzzz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3krcguvoz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3giidotoh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3zjbhngpg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gxnrofxu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pfspladi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3knrgprwh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hadgevjo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ojexgsij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pjiwcimt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3lmwufhex.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kulidwuc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3gxzhrgan.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3bthbawqu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dstlbwnb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ogizxwbi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ywekpgoe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bjokhggq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mbolzhdm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vclvhvfo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jpkihguv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3fpqvnljd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3tusokmrl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjujpsb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xgvvtrdo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vwivzrth.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pwezvfhx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ycoidzqt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgupvcsw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hurdetuf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3snwofdsd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3xjcrnntj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3fauaenht.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3mmcefprc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yzcvfipr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xhbchysr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlyfmri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3orzadfwv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cgqaeuyb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bborwcbm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3haixojhg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3amwobokf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3zanxcqqp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3hzckohoz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3egouewbc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wjwdmxry.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rhuegbgl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3inutcukb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hycgtnxa.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vlzwegxp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mtmsuuxx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eosrcvga.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3orbeogru.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3asoxpqqy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrgwwkuq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajygvddm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fuzvfeyl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vatwxpmz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3iwoefjii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ahyynkyr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3psjtlpst.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xygupigs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3yumlrvxh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pdahxykh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qbynumhl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ioenpjmw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3nbkfywef.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jyjtfzyk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3kcqckxcm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fyrnrtxe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3prgifron.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lqapasdg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xmwfbjus.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qmtaclto.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3duooyyqr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lemfrubo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3duacrlot.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3keaihadi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zjfsofym.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rnwrhfjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnkmlujx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gsgfipgi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3pokulaqf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zjjcxfwj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zuoivmfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfcqnkqm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3kjhcwuli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuhjuqpt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ghcomlwy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ykahuyjd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3exujcazo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dphkiqln.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqtzqiwb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zrmmakjd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lucweznx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ftsdcvso.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndbieshl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3dvqncfff.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mvxmpfdd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3aidlozjq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fjmaqaet.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vpbklggt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oaippjrw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nanbfirx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pueggfff.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvjwaae.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zurlfekv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jofbcpjq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zotoyicv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nijgbwrq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mnwqzxic.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emhrkonm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3davoewxv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ocotchmw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jyleqezv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmpddmck.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nvqcyhwz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3plqfjcjs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vlbvxsvw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iweknhpz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jmzwuarz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqdbhrb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wcfkygyg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dmgnppos.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ybbpfvrs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvhqmykj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hpbvialz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3phsqrkxe.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nqktttap.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gpunzzve.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3yvzmiejp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ysmodcfz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fggigtey.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3whfqbrec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zmfbchxa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wtxyxnzz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3reszdozs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ipznamps.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3initzhvo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fneabzrv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kktogjpc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbyhvur.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gzkqbkis.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bfskzuqv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tmiegbkb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dnnextsl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3snltrkaj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fljawlno.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3adhmwgdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3engyfeod.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zrzutysi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3heoyiebv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvjibmj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kjryctex.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ubinaito.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pghwxvpz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aurmiiej.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3tfmvpyur.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcnhxhv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3habdikmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czxsnlxh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vvmdoiig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eppnbbev.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfpdcd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ugnknhzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vhwstops.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gzncydum.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lywtklta.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xzzqtwvg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dozukpxh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kszohjtl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3eveajade.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ctpwbimi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nbaiylgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mnbzsmut.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ttiumhjy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wbvyqniw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3qxppkaqs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ofoocsif.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sspbwcoh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ncygsszi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vtvhnkee.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3uysvykff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fnylmgur.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lcdlfbtz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nlvdiwfm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cidsmznj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dhxfrumt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bsasoxpz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cmavpgrq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3beynwbfl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsuudkv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wkgsrvuv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zitojkio.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yyivtwri.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fxmmgdhc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rcmwhgxl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3alivlwrm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxzcjjw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nfgjlhfw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ksubpuel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yymjymmu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hlpueohz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ndcgozgk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nfvoxnis.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojhllvrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dasqirut.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pmgwldds.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qbcgnjep.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cpdlawtb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hljxpqaa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqwuxrs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nrpvjtju.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xflwytpl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gstsoxpv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bainixab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lycpzces.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ozgavwjw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3acqlkovs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kyvyoiah.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eemxcyae.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3suzwxyta.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3devfwher.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eojrwbeg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vsqsgqus.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fyuwllje.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wzudddfd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pxfxcsur.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jrpduavl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rpknhdao.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vkjumskp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mtjrfody.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qqegogvf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xcglfzvn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mnslboji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmscoceq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qjzdircr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yndztzhh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tpcwpbnf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ppovudlh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vqgkhacm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkfycsb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eryyuzyv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jinwupaq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zpgeovow.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mrtualti.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ulyghpzp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bgkwndsx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vgfqoqus.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gndufiym.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3stqrobhp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sjskgere.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3otkauzwi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yeqmledf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mhjrgoei.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wfbthbxd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pccmkiox.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjzjlmh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3djdoggan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rvbirpxm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cuxeknmh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3omwhqeen.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wcxfycdm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3huvimuwq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qrqorpoc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gmgikyek.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sicrbonf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3odzykyvl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibbqfbbk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uznpoeth.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gqtjkibh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ntqmlmgt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ewuwzzac.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ivzjemph.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3avniigdl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsbhpxcf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gxarmewi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3weirqokb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lifotwrs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbaoobj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3efodepsi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3liikzagj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mncfsrmy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3eojiwtyg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhdfxls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sipqeuqt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zzzvgfjf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzyosk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wuxxpvum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xhjxrkao.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ewouspqo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mxfordeg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mfxafaru.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3aovkdmof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cxkbmxyz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nuwkhppm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yhpqrwba.html


<!-- 参考信息 -->