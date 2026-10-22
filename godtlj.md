代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qlcnkgul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnsgxdhk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fnriaydr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2obiqtkyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2spckmibc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hpejwbkh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xhavyyhj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rlueyjqg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ugljvouv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ldvlkekb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2krdywozz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xttlhzop.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2aeynvdbd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kpiclpmz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ueqpkshi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2cfopmtkr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2pzaxykad.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ijndmmnx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gmvphkap.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2jdzvdwvd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2gzucxmfn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2qydbrlej.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2tsewnrbx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xabxqpfq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zhvoamyh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vvetsymz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uspsewfc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rnhfcoyp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2idomclpy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2kifnotxt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nucwfdjh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hmqwxxyp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qmraogqc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lbunxqww.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fclenpdw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2uailytvh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2unrzgjru.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpvuaiu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2qqyyngjg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2gsklsgxx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jaferpyr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vvjwxaki.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtlipna.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lvvkgqxm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsfameo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2drvtjzhi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2crlxmcoz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2geuqxngf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2tgxmavvk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zwanijix.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2emutjyzb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2uembvdov.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cxgfdiil.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2qiqsfoap.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gbppurys.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2xrlkzixw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dwgenrml.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2aoujrywl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2uqwcuztm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vpmzsqug.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2noxwgytm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2eeuvrzgf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qzwmlrka.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wuwvaaxi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hglpbepz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nwqrhaxi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hixryhfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2houzkozo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pvhthpjt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2sulgmlsb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xffggghg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jzngeimy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tbatxrmw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2cykcgfbc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2yhrlhcgl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2lxjtasih.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2csfkxcfq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rtnvbgau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jeepgjih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vgrvihfi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dbnxjmqi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2aurkhbqm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bfsitjlw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqosbl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2olgubjgo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2crprehnr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2pkiaupuo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgzbmzuq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eqidvqti.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2uagvdoid.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yazqjylq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkemptbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btjzddnh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rpucccbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmmebqog.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2madwgpgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xgpxpbhm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2piovvrjc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjotpofd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zwdwrbhe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gihsueqm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzcdhvh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2samftqzh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twtxyprs.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mstvcrcc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lomtserh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kjoxuxmb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mfkghrxh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kucutrar.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uzrduymk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2izdvincz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbusfztd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srswnpao.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zbnqpxlq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ekeqqmxk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dhxbluds.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jowdkoyx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xhnbavcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zryodyzo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fhsizbki.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xbgrmlzr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dkkpqwpn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvxllozx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kpywjynf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rgukvgzq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwdeuypi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pntanubr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkpdyuz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxvkauh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qjuhyivz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rlbexecq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cthnbzye.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfrpwyw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ioskotds.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqagvoof.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iauqhvtd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ngbxbfnw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sfailjpa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2iiiajcae.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mwpkyhuz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2zkssakqu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fovswhnq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdichumu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ccmnxict.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2phnjarrv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2colnvraq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jxicqoux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2suvgjnil.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2icpgocga.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yclxahzp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2btnwlddm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2iwstnyza.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oyvemkiy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xwbmnitf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2duorihix.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rtzlqjml.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqowfww.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nxzcwnvl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hjkntfel.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrrimtv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ltlpemlq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mkytpdxa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xpwufsip.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gczqlcnj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gobdnyqh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eevouizu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tvtlkuvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koebdiqg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cyqquwwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcrswtip.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rnvdhjic.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2swewugfx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mmnznrni.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2plzvrjzv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qmajbpzn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lqtrnwee.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zakqekgy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tqjzubpk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gvmdvehd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qaqvhkdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lnrcmzar.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wjwsqaah.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fcaqrctw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fmfhvvzn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2edbqyhzu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2msqrswhy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ktxluhcc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwybhfzq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cuxahkov.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dsjogaxy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dwtxigdu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jvkmhjmt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ngxumyrg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2oxinjdlx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jojbwpuk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zeasjwsm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jalukzoc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2htgtzshd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gwdwmwgj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qzjhwyzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cikirjyx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fztbezta.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uiyirzsj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kfwyzglr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2upznmogr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wefzgkms.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xhnbyrbx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2pwfpdbkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2injxkyyn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gkkzyxmy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pgfwtlfe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2geqclldh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhxzgxrf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dszswnwa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrrytwtp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xzqursqi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fornoigd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2duieljkv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ehqxsonf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xmhiljqv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cczejwap.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qeapuisn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kxwcauhq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pcbakgbv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sabbvzxu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ahypynkd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jihjcsfh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xeplcinw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hzkygnlr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2urloedft.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kwoztdva.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dbyuabgm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mfwxtkxd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hoxljhrr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gdritypu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xablhefn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lbrahnit.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pyjyevmq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eituxwes.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qleyakdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qkwxpnrs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjmtrskb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chkpljoy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rpxmyhrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrwpugcv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hkmuqbvb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2miydgjey.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ezezqhyq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ggzhgdha.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqijzclc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cdcdeltx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2raxekepu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2arhecumc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rikuwidy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmwxtvad.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jdgtmucu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jsysrnml.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2colhkgpt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vikzwjzg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dvgzdesw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qrtdfqxh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ksgfnyqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tecefkcg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fjzsapem.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzmzcku.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nqcegckd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmruof.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hhqpzxrr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vekbvofv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rqdhgump.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zrutkhpa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ganoipoa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dvrblexo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cefihevb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vkozythe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eukdlsvb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tngqkmur.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2enstvoav.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2eystikkj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gjksgrwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jyxxcovr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cfjrnqav.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ctlptvmp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbulqktq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ismdeoin.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2foxzmknc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2acirckai.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2thescrti.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2viowgjim.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hyekleid.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2iqsubgea.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zoawyodm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pffkwwiw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hhvqbvsl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wowwuaok.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2azmnjdrt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pasdeklu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hvyuzcnq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vkvkflaj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2alsxqmec.html


<!-- 参考信息 -->