代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jbxrqngt.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ebzgmfzu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dvgrkafd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3gwflycic.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hourdekm.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3fjxlyvnn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3whqrxmme.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qskxmnkf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rjblwvwk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3eyvlhyjd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xhoexnhi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3anolujme.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3plgxawia.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uuzxypho.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwerlkv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kepwoxki.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xyegjiac.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlmvvlf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3imrbsfxa.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3srurpgmv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uonbrctm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dvpkjozf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dymjvvxr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zhmyewyj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkukrjx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3vssjqvjp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3elyydzrr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bnjwpwss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3helmapya.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3bhxuswgi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bgklxrlf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ccictaca.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qldvskky.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbrsrfq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwilnq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfugvce.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ejyaiwjg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3mykryhhh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3euawbehx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hazjoebe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ubufjniy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3aeqxdyhl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3drppmbdk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3izkptura.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3focquuke.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3vxmqbjqd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3inbaimwm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3otppcwny.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tfvqxdxl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mrzeoykp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3vufqroia.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3oxjspeql.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3jbqaektc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jngoqvyg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3eadfubce.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tfuzqive.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mpzshuwe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jckpwdah.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3gjxbarqr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3waylbfwh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3titdgmnx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3csrljtqv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3drdoxiwa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aatzlvju.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ikpjclhn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3vhucmnue.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gcktolfg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qhvsmoti.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3nffivgdh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3hlgacapq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wxtqeatm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3cnfwhbik.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3uqdvkvpm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhcdebm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jpufisws.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3istnjgvz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3priczqpn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vuvngedb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3coplxags.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3favfyohe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnjzmas.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bzhufakl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqjenwg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwqdavj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3jwviewii.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qlaigbbm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tnfquigj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tqavefsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sricwcvz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hadqyuma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znwewooy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dnztsxvj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dnnzgybs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cbhthbku.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qvrxdmnu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxggkfw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3vncypgpx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhvobky.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lulsfofp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zipeebrh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3lxlbhqlo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3depydatl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rzrztney.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cceuinhr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aweawusc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tivmwbvl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdfzcyc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dfheeskv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywgimcao.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wtzzbyzf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdkfnpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rdnyztmz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bvqmmggj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ivpkqhpt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qeaatebf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpztvrb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qymnomqe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bikdcrpp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ekhsempr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3beoyhlzj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rfaxaexg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sttjekoz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aawxtpja.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kwyxunyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrhrsz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ccikyyhw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hyrzhvei.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bgntymmj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdveujf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nhrazeao.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gndoqyjz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csztlgnt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qxwuwnvk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dfpznufj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cpsjzofv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fdvpsogw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xrvkndyr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ehkazjdr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ijncfcoz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mxedafdn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kuedpjmx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kiodwsgs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yqacfqxt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gzpfhled.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3txglrmxf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fseptssg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yupkmpzh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zczznpwt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tgoenocp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xronjifz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jewurphn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3osswuhlo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3iaofiiat.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbmvbwt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ccsqgdxa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvaolgu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvdwdieo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nlkudyjo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rzrnsfcl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jwdtbiii.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mbcfjbry.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkegyeuo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xekofohw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuqtomlm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yyktxocv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgndrois.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3higfglqb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vlllxwvk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ocfnpsrv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlfvvbb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cvoyfjqe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3twizzdur.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3welfgrra.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3thonsuwy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aqttkety.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3auhuanwv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vphdgfwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3yskagjzv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qaprqakd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nnkwmwil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hsqwnqrl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vrpgkkeg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zhbcnejb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oclbpjzw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3eykjbodr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oyrcvxuc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uhfcbsfg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bjhngowj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kdfimajq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zxgbaxaa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xmfpfwaw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gjkdfldp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nelrzbpz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3harverwp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3podksxjd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qdqoyuyq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3syhhsxfd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qbujejcg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cnhxpbbj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xjyxzgyg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yofyjead.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jchehjbg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tvxlgmcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3woapeuwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgnzxev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ubafagxm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fhlwtumj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fvvddihx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fwgsqvzq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yoxtzbtx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyiblqop.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3prdcbuuv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wdufznyj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlzlzwa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ttglatyc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jfyjcsvi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sapqvszb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zarrmcrh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qaeafqfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3oqashyti.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iflujnso.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qrldyvjk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cujfdzih.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dmjiqkhz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxfrfq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sijakqoz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kjzkahdq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wfbdrbii.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rfretfck.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jwxeumqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cvrttidt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3opoguhqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcfwwjug.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qhscanha.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dqenlsla.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gkwnlaqd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xwjvkcga.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ptqghkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jufcenie.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iahhafrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lousrtei.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vpizhcna.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fkomyfoc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tlvqpdfj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cnlnvaab.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hrajmfbb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nxhedqyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3robdozab.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3eslpkhay.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cgjweiqg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xotvsrka.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fotvwedz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3roszacza.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ijzbxwys.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3slouspzm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pycznsca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eiuofphu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bmlutzhq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yijyquhn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3etglmtqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dcoerzhc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pkylrirn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ethcpywg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zpkkgroh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xemxaezo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fsagwbwh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fdkqqckw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rozcsifg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kzrutlxt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mvigahop.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uaxoqgbf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3isdlunne.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hdlmzvml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fwothgqe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lnabhhdx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pcyhfcjz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bsivrihx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3buaswpxu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tmnemesc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kfoompoz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqkcaac.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlnhglz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uffucsqn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3muwcgark.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rffjvrhb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qulsvgpf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fsncfqil.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hhchtiau.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gvhstpre.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jdzbetvw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wybhqygu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rzbnnsng.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3idschtxa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3avbhlgrw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iiuacxth.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ntkfqghp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rbsjnqrg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zlpgwnwb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lcvgpiyn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tsfiyvwn.html


<!-- 参考信息 -->