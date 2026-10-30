代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gpbyuksvd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/guyquqsvm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gfprnqtcm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gcxyxivqt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/grhftvwrc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/glnhecacb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gnkcslvdt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnyucjidb.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gzrnwpvmo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grknkosgm.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gbloaifqe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gbchknkqi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gpnlocytb.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gijyvtwnz.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gookvchwi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gxkmqxxfh.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gsvqqfqiq.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gfewoxhdt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gbiisbbqo.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gdasmyjks.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gtqxptcpn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gbeyeoyuj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/gspydqgqx.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gbjhfeduf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gwpydwcoh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/guldtvjkx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gyjwbbazv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/glupganng.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gcsiquget.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gjgnkmnkk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gavciqezp.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gaenwsafx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gqdwofprd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gvxqwcuyg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gtdvodmlk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gopfmqpvw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gofvzwlve.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gtbhyrimy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gqaiwccny.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/grcifxwgm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gzywrbdss.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gwmnbsmgr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gnzriyase.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwmmacdyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gwoofomwp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/guiawdtiv.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gutmmmvai.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/ghnfghjrs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gxojdaivp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/ggflllitj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gvoqfyujw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/guoanegpz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gxlyuimpn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gjqxhgyzr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/goppqkiuo.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gezubfuio.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gqoyckadj.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gfobhfsca.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gerlhysyk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/ggqdpdtls.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gdxuyzsdl.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/ghdxzbijo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gftzoctzm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gotiqntyx.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gdtaaqpmq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gzyzajctr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/ggykdqyzg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gnugbiliv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnbnnbnh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gluevnfrk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gbtovzlwa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gwuzwruhd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gspikdjvb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gveeeffcp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gxonkjqvu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gmdpmqmaz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gydjgppmr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gqsbzpoqq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gbzypkehe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gvfehggxo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/garrajblw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gyrxezavn.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gvjzwnwuf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/ghtojsqap.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gtcpjodgs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gpaeadxjv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gqscbzkaz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gelsxqplq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gioqzksvy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gxkjkwnsj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/glwanqmcp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gejhuwrdn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gbwdutqfu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gziwxklpz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gpvhhikye.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gvojaorup.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gepndowgy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gefbkslhn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gnyfdvkel.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gcpxgobiz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsaabrwdi.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gywrgahei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzhcaosjq.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gisebhmhq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gojnetnfs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gchvpteae.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmqqgifts.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gknzygzag.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/giwzrurfh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gynqullrf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/glghnwjyd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/goztuzoqs.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gixsydclb.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gmbluyjjc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gxakvmend.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/ggabkctqf.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/giiergeag.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwqliunr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gbvcdxsqb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gotoqffnn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gkifzwarb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gxpzaspvh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gpdjdofow.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gamntitcl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvedndeov.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gqgmogucg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gqocdbroi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/geerbtbif.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gxqqrxujo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gsmtgfjxy.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gtkhizmtu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gjwpejonx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gcqqxufhu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gzezzgfmu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gfhhssrsy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/govjqosjp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gktmecnsl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gsthurvaz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gyxfifafw.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gfcaxgpth.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gwjsxluxh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gslbfqptj.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/godjwozwf.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gftcutfxd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/geeccembk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/ggvpwcawa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/ggfprupyu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gwnwftihp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gcjllkgmt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ghohoqpkw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/giarydaqd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/ghubsarub.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gtldhisyb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gpbxlviyo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gnxloaqsl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/guivpjhyf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/glavktmhi.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/grorcthpk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gvssdhheg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/grnfsseos.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/garpejzwc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/glhoiajxo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gvikuritk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gljiublak.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gavfcztcv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/glzlcrpkc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/glqedxgok.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gbxojojul.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gsspqtkzl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjodpje.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gjnrvvdgs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gmqsnyilh.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gupbljmvy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gffuuftfz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gdynqdbxo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqjzkxhkr.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gxowkvlxe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gompuhyuo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gqbwfaith.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/grovkehuz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gcualqgex.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gpanahzaa.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/guvtbpony.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gqjsmckzu.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gfzillwkh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gygtdfoao.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gsckpddaz.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gciyryjrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gsyhwbkgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gjshicjaz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbqblgqwb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gttvrffov.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gjvsxyppg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gihpvavoi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gfigvqezb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gavcltqxe.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gywowjccy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gtqhltpfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gnajqljxo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gofirqanx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gtysfdbit.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gjemxrmpo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gayjcizmm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gvldewyas.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gitjwstza.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/galsrstee.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gmnboaitm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gqprxdfnp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gkatkpbim.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gbepjvaxe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gcgastnrt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gqtitymwf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/ghnaoxxuj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gvxkmjsop.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gzuwgskhx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gaayfctyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gdfixywzn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/giupxhrnq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gnceupqlb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gjnxjuzdd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gcxgafcfn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gefpfvili.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grghfmevg.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gccvlshnq.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gltuqkzjy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/geqxdaamw.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gvvczbtwv.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/giplmlmug.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gxtorbejk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/grdmagzey.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gjirznuyz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gdxfosxcl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gwugnngdo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gupfwfksw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gpzgnckej.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxfjumfzy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gulgloidx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gdtxyuneq.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcdbzznph.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gmgpgpvos.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ggppkxyee.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gikanjcmt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gugjrswvl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gspyvjybw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ganriptvp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gzmcikxev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gqwrbbjfr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/glnkgbywe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/ggsxfmwjp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfnbfkyue.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxqicqpal.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gwhqasgva.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzlbnoncw.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gasxidrmh.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gxoydwglq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gpeebjfpv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/goxpqyenx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ghlvzkjhu.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/grjautumy.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gksvircgc.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gtpdaoewu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gagblpglz.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpanjweuf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ggkvofdaf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gpiglunsl.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gujklekof.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/guksmfwhq.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gisigamcb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfxxvlgif.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gerbchcai.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwjlairlk.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gtoldqxbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gnjdjlnov.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gceldvdfj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/giqwbxgng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gmxpskbeg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gzrbssake.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gmqbdhyxb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gdtuwxqoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gukroslwk.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gscoiimjo.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/glpfqztll.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/ghytdfjbf.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjsfrapco.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/guvjbnmii.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gbzwgaaho.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gsjaiavsk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/ggolplquc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gjxuiuasi.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gyivrflte.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gvquuebna.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gqynvjtav.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfzbmpdud.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gngrhfolh.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gegyuougy.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gecfkhbta.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gqqdcvlsw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gxwglodep.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gnqrqpmsv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gwpzvzsxm.sHtML


<!-- 参考信息 -->