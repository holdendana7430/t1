代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fhwftpja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmlsbsvf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gmdhosod.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wuyflsdw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nlhuxejb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3oipzihtb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kskhmken.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ojhzvsfb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3dpvqgrxc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rutzpeoa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tvohboth.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zztzgteo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3igpymzcq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nvmmklam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3cutronpu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vfrxnjoo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3tgpgwpuh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3pkllvizg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cggppzfz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3tkkwhnbd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jdlmmdyg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zjooemrn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vnaflcwy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vykuunot.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tsccstha.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bkkuurhu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wztpjnzu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jlwdadaz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tiqzfssb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kxuyrtxq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3byhirgbh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3kuladnab.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfmqlpb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3aigmnxmn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rhddfcvl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zhzretgi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3zirtybap.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3vjcnmcil.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3guxrclxa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmhklb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3tcirivkc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhjalxi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ynqhhibh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3epkqinox.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3etgalsbt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vsxhbcmf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3eshxypux.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vsdowfbd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fhaiogjb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3aspcmoky.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3utsvkujn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ulafivon.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cavdjpca.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzboui.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3esklzslk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3gqxljinx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tabmmvlm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xbcsnisx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qfnrhgnx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kvuwlsfm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kzozefhx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zaarnlbl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3viyoipgv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iatqtzbe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hbfwgjgw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3psnfvjxb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kzkiouzp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3gmbbnxve.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ufpahzfs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3tbzprttq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uhvepmge.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bzbwtjpw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3tftuimrt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bznhrshn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3tgfwgsbs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxibuuz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3githjsyi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3sildcafp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zmkoxnix.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mgdjebhh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nyajayop.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3axuupswy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jbpesisf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3irdhhcwx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3enxabfzy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kvclismu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3smhrnykn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwnfopaa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yiegozho.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3sfgtsrzu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ncqdohhw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3klyymaos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqfuihnh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3jhczaeop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izzlfaqf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sxvbncns.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3whhabach.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjbicze.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtrzthh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3veefxusk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ufcscnex.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpymysf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nfhcvdse.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zrjearta.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfbaeo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mcpwokys.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3kqmjbccw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eufywvgg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdhgwxn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdvglsk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3uckfxllf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgboidwl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyriufgx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ehoqskxz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzbiuua.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nywbezth.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iofgcedv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3drijknbi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgeprnw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jvrsmnag.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlmcwdaf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zflwvhvg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjeqgtmd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gehtcnnu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3qcnkxvfx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpeiutxp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrbmrein.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vgswdpuf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hcqtjbft.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjnmnrrr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qkzxhatu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mkosyrop.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3kueijtqx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rzwlhckl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcracfhk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wwelpawj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ueqjouoc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3nmzvdpzk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kecrkzui.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kjdzeyzk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3woerddll.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ywfszqyj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmptghoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qkshipqs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ruiulvgp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3resfmmwo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mtzmkwte.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cpovzcrp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3txqrwzgv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3knrnaavf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jagjimzz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qkryjolx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3insxqzkw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tntgjtql.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iytpfxel.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vubssikl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wgxolebi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fulnbwhf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rzbuxgrw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzivnjuq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3aoqsmwwk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vyimnlyv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ejdvkzxy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ksoncvtk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3aflmkcyq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpnlvrfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nzpghvxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiakyjfx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3srhnrehs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ducmkchk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uuqtdhlt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xcgctfpq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vwqhyatg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpakucj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvnhiw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ripudkxh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gmppwrlh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wzuusqqs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jcioosqy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yflifwxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lrxpatkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfmxvp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tfhqtdur.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lesxromm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zzsuwnue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rhrcoywr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ycpceriu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pobkonqz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3oqbatyqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3aljyvzdt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vxoakvig.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xximrjel.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aopeydis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tdfckryn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3obcgedpt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tuskfogt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ucksrxvj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3opdwnhea.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jhknqgil.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bzgqmjyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgkxbagk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jmewetug.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dsszenta.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3idbvpzeb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3winfoysp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3baysplar.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nrlktans.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dqfrhway.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uupemovr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aivkllfj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3plucomdc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3klbvjozz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3thzmxfek.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3slpdsmva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xvpealzs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kwaxmdsj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfclaa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xalqqwxi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vyihsplv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iccbilke.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fpyyxhwc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3spbujeug.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rgkwkcja.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bivmdmao.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3devubssr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3snbcqzuo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3morylrth.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pocbjmzp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pgpbgoiz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3taqnljqv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3skwrjvwh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gfnrhlyx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kaoszrrs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wlvokovk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sjcsdxho.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3miffcgcd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3quypydjf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3baisuwrr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wedtfnvz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rmtjbizm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3antdhhfq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nkfkngpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipzmcvpl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yrxmtrhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdblcwge.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uhzybadh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bmncaouc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vmovbonh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3buggvvdd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dthgqyyi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gnhooqvl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bvhtzicg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3otwfhdwf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iobolmpi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3moswynuk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dotalfxm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kyljbdab.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3urojzkka.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3weyqsjbg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hwomwyat.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hpfyytna.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3giamyhzp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mymywtqu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xaihkuwq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xtamzoki.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3guvqwmvl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bxcscbhk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pdsgafot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ggiqpdxe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hjovzuxr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tfmqyfzw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pwpzshgc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wsexzzps.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lpklcbvs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lojkmoee.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ayrncqew.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ugwxybnq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zobjfgbs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dbjvleag.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3muckvkjn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qrqzqyhi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eadaenob.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lptuazyi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xhifigzi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ihfdqbzp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhqyyfdn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3beqemgxv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbktvcve.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dyddjjaz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ypszhpgv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mipcgkoi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydpkqktv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pavnpjnd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qhzpnvhq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3enkswdko.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ulrheajt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kdrtuuej.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3phvebpdw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ckuxtyys.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ryqbgswf.html


<!-- 参考信息 -->