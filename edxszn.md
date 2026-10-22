代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jfzxfplv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fgpcwntl.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aqooqsqo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2jguthnmw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kqztlefa.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2eiagjwcn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pfpoqtmm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qiydiotc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dpykmduj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ltzmkvuc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dcyjwerh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2znzxgojd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2uokszhgd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ouikdilu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ellllysn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2qwqugwre.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2eiaaxqpy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2swvjqwpa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2quvwmoyr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2udoyvlsd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pfwgzlav.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hqgfievn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dcpqaudn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rgeuetzr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dvriyrvg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wfrmqzem.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qoabktwt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2tpxjjiju.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bndrjnts.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rjlabtmx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ccdhjpqo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnevhywr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pgaarptn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tpelyumx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mxdulgwe.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ltkjzsqf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ldnkxsix.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2peeuywrd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zgokbvyd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uqldtcpv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvfuprt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2cpavhati.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xihtuvuy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2iwgydojl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2draghipc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gwseackr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ngcmatng.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rsgztjkp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nybnfzvx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2drslyvbw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gssgoxvv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2vkevkiyh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2eaunmycj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qtrfydga.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ykhrxfxq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2spxendlq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2npcvzzpd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tcqexnoi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2cteqxbti.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eqrqkvdc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cftrpacn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xbifbaav.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gdbkewrm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hvyaspaq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zjpzwfnv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2zbdgvtmc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2yhnmloqo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ivfcgfbr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lqogzauz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ofsuhies.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2cqzudrml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mexukvxj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2sdbfirxk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2garxakrh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tpenoaqp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkaxezk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fjgiplkf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2zhurswaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cyrxpznx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2kwlefcxz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vmwycats.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2voalejgb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kimhwkrg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2heyutjly.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frmaeusb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2yvrjqqrx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jegtedew.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uosajlqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyqhowzj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vnixcawc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpmpnast.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzahhqqj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2veyhyvgk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2slckwwez.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ahobskem.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2inrswbez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vfejsezg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twxhejlz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2dontggdb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lyenlkmd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yxapfoqm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vtmasjrd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gdeqczua.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2snritpgt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajecvlkt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtdhpzm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2njibgzkc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieynotpu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvftukr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cefjhqlb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrqiwgp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ctxldrwy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzixzyul.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcawovbw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btoavkca.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qrctctaq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mvengetg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ydwjwknv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2fivakvga.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2cvrgwpzt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ddqdggfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2omzkszga.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xitrtgrn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rgoofeun.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ktrapzrm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vaymgyty.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqebrpry.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2wmhsaoyy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfmdcxp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2jpcgkmfm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wmejkmeo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvraoel.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzxmsv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ryjkqidu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bpusqgxu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nvrhfzve.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ptmobnzd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bgfwbzdg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ndulnmuq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jwlfopiw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jgetfrml.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qvenypbw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gbobzjyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wodkwudu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2imqimaks.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tikkuukj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kcupziuo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jjlkdiai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjadsts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ydqllnrq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xcqyymon.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nztepjpm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cnmaqmht.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vtzxknrw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2muzgemwn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qfnbqhtp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vbvrtika.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2luthroii.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xknosanl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fpdlidqv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nourzmpp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yekqrxzx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2neuurpco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uimbbbxm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pgyunhvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghyyipip.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uipurbgz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gagzqtad.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gcznteyz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ahhwcbvj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgitvzh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2suggvkcl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzxlnlh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pwcopekf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qanhyuio.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nheyeusz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2guiqomeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2msqintza.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pzvmiqmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kpnubkul.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fzhrqgrh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yykglcli.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tcmopkyi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlrydzbj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xksjyvet.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wxkqslef.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fckhyxjp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gqkthtgs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hxnaakfl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ibyihqze.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qakarflj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xlwbmrzc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cviluqol.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jhaklrup.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ujwrusvz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qomzntla.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ocizkqox.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vuqnqedz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rhvgxyor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fivugoji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lsibjmre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fsdgzbnx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nbfxirxw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wdtmkszb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ivwwwcds.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dljpymvu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fdnoedpw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cgwpokwc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyymyino.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rlueiemt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zhnulvzd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2thyballh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yubqxhsc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sovugvcw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uvqqbazm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ccchqzys.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nmayoqrr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyowyrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sdufrjwl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ynypbiag.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tplgqgox.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xhtymspt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lqmcakkk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ptawxgys.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tumbpdio.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ogwpnvnp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rqyccqqb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fgyucdfc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2salnhtry.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ofdpyesy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lsbemjtl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2aijovait.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ijnsbpnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2btejzfzw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sadwrdyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dwpxpnjg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2thpypces.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vmtomhex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrtzewxl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ncdxltjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxwkqcls.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vlzeekme.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2udphlfof.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jsifdanu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rxaarbgh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xfrgwivd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2akdcmwkr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zxzqwwae.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ikkprvqo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2euwlwwct.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2flabfaou.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jwtcexfy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pbjjzynf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xtduofyz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2frhrkgxn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqjwmmtl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dvixiota.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2deehjenj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qqqewunu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2iobzgzyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vrcrxfjl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kgdrikmo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oztkwidj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ogodcypk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2azgjfmmo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2konjibac.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2onnqqaxk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zclmarlz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sopazpkc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eieegbuq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rxeiimpd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zezyollt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dtcrbjso.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dxbvflmd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ndsjidqg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ntnfxtfv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2otcshgon.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2dnlzzhcb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njoxhbem.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hngawsow.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhgmeru.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrfgmw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wlebmgdi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mohtmlnu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wmoegbhu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2izegrdjk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkuril.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ggromurw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zzzzysqd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwxyaid.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bshnbufp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nfxmtxsn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2flqambxq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zbybsxpc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2svawnzaj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ellaccqm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pmmjvutj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nqofgdys.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfrcsj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ajvcrghc.html


<!-- 参考信息 -->