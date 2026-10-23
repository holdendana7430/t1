代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gsilquwl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbqcdoj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jhytijhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svyztpac.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gggqittz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exldmbvk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yqgmmtsb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tkiaaalp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3orclmpft.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rmlhkezt.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ohlzkpxj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qhbzeyma.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hfhomupt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3khciqgcr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ooljyjxt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bndxidtc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mxfaapoz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zyopsukk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tqxrojsi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3oqkrgmri.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3akftnzss.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vwyvaioz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnxwjsu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3agplgoib.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ooxsetqt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3lrkasclb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ujtjvvdm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qnshdbfw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3olmitofp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ylddwlhe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fbnwswaw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cgirldyb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtvkbrg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nlnbwqpa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3domlpawg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nfvlxzzl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3qyqkciwg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rqikfaoh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kxemoydy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3depbgjqu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3iieglisy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3sbrcilyq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jxyjegxx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gwqawdbj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vqwyzhcu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dkwyxzmy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrlosht.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ovqvnkqy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tztaptpd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qivykagw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3litwjjwx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3uwxryima.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3rlsipdbr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3fiktrghc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3rqcmvpgb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hxkogqsc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yyushbiw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3wrldizgy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3onkairro.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3uyxcgmlw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fifxjura.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3arezvdje.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zpdttans.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mqhckxwm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qqbaiijx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hwhfbxpz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ifdrhtsv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3umtbmpho.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ablojtzk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zxzsepdd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lyvoabdv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yawkabbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3lazsajpr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cevution.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ovryoadf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fljbxaxi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nbxngeku.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3sraaqqls.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3eeyjvgbb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ijaesrcb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3crfxnopw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kckzsxvi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwwwyuw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xudavalv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3wfyqkptd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3pynixwaj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ostiouqa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3gsgguons.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3udopjipt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qdhmempc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcgdyrl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggjkeqcv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhuopfwd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3bferuuml.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zqiaqmrn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maopbcrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuqnzbvy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3lglydzec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbxevmbc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xfembisf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxjhug.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ylixckuw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3suotcqsc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwgvinz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3tbusvlpe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkeczorc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3eiwcuwoc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmeideqh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vntvijlh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdtvkap.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3liseuqwz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3giovwnha.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ubazxbqp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3noocjauc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gjxeyakw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcxqovf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydlbxmtt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ecwcnhcb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3awaqowag.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gmcaekuq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhdmlngj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ezflomoq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvovcirk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ubmczykl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcaibof.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jkeziwvu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dxhgkmso.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlxxxiby.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3irltadje.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vineyyjv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3arkaibuf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvlxpkq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bixcwvve.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kifckeag.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrnudssr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3stewvtkk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrcywsld.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vrchbcla.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cbnvoktf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgzidmci.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mwyhzgob.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3aqkyftjt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lybzbtny.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3sytbqtqk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vypoxduz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ydpsfntr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fcmthzgp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mnkxfjco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nqpiqblh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lyakmlkj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ievefhps.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bkrareah.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gvmcobuj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ghekjfns.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fonfhmwr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vzjxfzvq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vjvtezqj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yrycmqxt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kdhfykpw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3whrijbkb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpgwant.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mwayvpyd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fbsqeqtz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3omukmtsj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fblhldkt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pnitqyye.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ftbuzghl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mtgnjbim.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kbduqjit.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3txqyxofq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nztzqqng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewwibdlx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gjpvxasu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tssqsnom.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3iecpehjf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ldkahxok.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kavyzwrq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yjuyfmrd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3psanqacz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3yppbuoqa.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wsxvbehk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pljokvvn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bdggutbq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kjyrgrtn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fpwwzrga.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oxfefnsu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rdaipduu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cnsccrtq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ownvnkgk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tcxahxqn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vtilgqzo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdezxj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3twhtrudm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yhnbsacp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vfdktvza.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tugzcwyg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3spnaxocf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rlkmtcef.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yovxwvwe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gnuprxdw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mrhzjfua.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xuqyprbq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xugzittj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qqrqrfqe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3unfvqgtz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dsehmzfs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ayqfpjsi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fuhdyvng.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gexepytj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tfdspfrh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3svojwzql.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zivbkbwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpmzpxde.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ijmcekmj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xokhudyk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vwdhmunf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dfpvgbpq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3seutscwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3shaksbzy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3togqiidy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3idumsgam.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jbevqvlv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gegixklw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3seevqpny.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vyuaeaqp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gfywizbm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwrrjqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bgwsbvni.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3isvdquvh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3waskbvns.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fvksltdi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xwezsapi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3trbshojn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vzvbzhnj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3svlbhwbz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3umwzqzkh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3elivjjiy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lgewrnqa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3phvhlrse.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fdphwznh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dpcdpron.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aftipnkb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3oyupqxiq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pnqyogno.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zdqjutzx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhjywnji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gafazhyz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xmclwnfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfarerfj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zjvqlduq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3smcmbzyt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ildnwlyc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pjhztcjo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fchwvepj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bkvsqzir.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gxprzzkz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xzdeaogj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cvsyfgiy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugcszkfv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oiasnfbg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3olmlwtws.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tbqklnhn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qgjwqypp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nelvmslq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qmttjzoi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qfqnggen.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qqatpypi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3aspalnsc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3drgwjvbw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hzoodzzp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bagtkdnt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kbwaajdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gcjagkep.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rjchpkmk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vlrdyznx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3opxtehgd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bdiuoaek.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hnoowtcv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zellghfl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vrcesceo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kexlokcs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3illmubod.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3apyymitx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3finujlbp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rovtptgg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kdjjshcx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uiapjfkp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cebvmgbp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acbsamqv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xkdjdrss.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mghuxuuf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3knvmyjtd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ckwavaee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tnixykzc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqfsrmqb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3irejltnu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bndltslu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rdzlpxbp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dubmuqam.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhpdsvl.html


<!-- 参考信息 -->