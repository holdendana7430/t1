代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3jwdpoyqy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kpgehedn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vzdsvmmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clhxucjx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hkmvoigi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbzkmsin.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3juexzfxq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mliwppbh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wdhzsimr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fccdsego.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3boqikweu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fwmtwofj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uaokimtc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jekpkvvb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3pltuotkn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ekrnauvs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3triyqvkg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3eewfejhb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gshklqcy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3noagrqyj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3rusbqnvi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3kdrwigja.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dmlizeyu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ghjoetak.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ajcksnnv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3lvphhmru.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3yvcqjezv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aqrfqgar.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jhwpyldn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kstwptsr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ucoqzpgt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3azqejbas.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmpzchl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ekwbomjh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3eqtpmdlz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3pthzchox.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vnxjrgcr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rueixeen.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhhckha.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3geppgirq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fjtistby.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3tbifhsdv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3byubexwy.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3hznbupio.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3mxsdxkyd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ndpzqegt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jswhhxmt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3pcfnlbbg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3koymycfe.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hqbpqfyd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vhsoajip.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3regxobcg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ywsalngz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3nsjbiovo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3gsraeyeh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kifjdkoo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ejuypupy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqapbsq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ulatzyld.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wlvaqsvj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3htspmqrn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fzbrxcst.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qjkrfomp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mkbxkqpx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lhlofrwl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuhklvyh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3qojltpog.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eavujsqu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cugltuwx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hcspkokb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kbpyweyn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ujubmulv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xfyazwee.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3btldyqvw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3adaspssq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qfaylmzx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3dmdahwcz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3maxjpebh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wkcnlgel.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ourvpzuj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3eyypzkza.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3huzuqdsl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fbaefnmy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3yydbhrvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3rmdwfbwz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3vhqvzuvt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rxozlpzc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bnjqycnb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3eflvdkac.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3pdrccmqq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xjnlqtlt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3srbmeqfc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3akibdqqb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ffkqyxth.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrmrcw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xulgdjlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brsmiiwp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tiwdmydk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xihmxoyi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gzhysfdv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tfuctxva.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pfkxzqrs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bumverbc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3crlofwhs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kfiasrrp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3okyuwvur.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ckfjtmoo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wffnyhks.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3wwnjrzwd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmczzwvx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3shjlpfra.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xhvetafk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ognqlxzr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mjfceyxc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pgfpoxyc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rplsiuob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeqmlpm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dttvkjsg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kghlrbyg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gerpoiot.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxpttxt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqusspgt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugirrdky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wyddwtkh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hukzzwlc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gtaboqgn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uafbmtrv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kjauggvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vikoyymt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qxgshmkn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpvmtxqk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjcybm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pvlgxwer.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dhybnxdg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3svvjcmdv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3iiiqxccr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3njottqjl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lipyvtgc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qitaycoh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqoctwt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3naspgczr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3rvzlvjex.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tcnhqehq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3iiabgqab.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3liqyhyyh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gsardkpo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xdknwnek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xcibdjij.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xhlppggs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hjodomow.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vspngjay.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mojuvowg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kgmhqktx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vffkgqks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eoasxmey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cyuznrgq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3agiybwin.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3degcomyw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gnjxdzff.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qakxgupo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nigxwhbt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ifqlyhre.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dhpeqore.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvlyiora.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ravszeun.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fcqlkrql.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gezbgiyu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3axtgpnhm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3htetergw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3npanuiam.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ozhiibnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egdbpidz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ndwrhhqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfjeffba.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ecqchszu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xggdwklc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gyjkyiis.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lgpkkbvz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lsjqepzq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wvglmfmw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cghaoqbg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kqkbhwql.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dxivihmu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kwowrnwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uqtnjrso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kiildoxt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xnfnekxe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3swjfxivy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3eldlgace.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fvljplku.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xxupxffy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvmkmeou.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tgitknou.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ohsngauo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqqbfvqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eezedxen.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hazsjvdp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tfatjtfx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pdiqmeph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wnkjgqap.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3krhvjmbg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3agrxqsnl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qqfvfefa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ynbwtfhb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gwtcciqo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cxhynqiv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rjvvjwyi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nazqfsji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhlyrrg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zzuyfyto.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gayiuvbo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kfdoryrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3svcqxqwe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3arwnnbci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tlkijrgh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jtrkkupj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ggjbvwlh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mubbnhfj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vlhirjhb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nlyjsook.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tnxqfgag.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lseffgio.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jstoywgv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aldbbndr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xfyexbzg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xszjpwee.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ljiyliab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3udmatttv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hbtxxrcs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lepxaubq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eumjzpxn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hdlenkfv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ysnbyywe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xqhbhkod.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3brcjmtyp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gpuixdla.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oztzfyoi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ngpyflxc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qzaufkeh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzxxij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wwyxtzvu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3teaqjohk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eipepsgr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3diokipvq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rcoudqpr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3oawyczkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfmdwmuh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zvdtxdmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxkezxsa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vygahxdg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hysyqqce.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3acpkljpr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vsgyjsil.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3agmbevgl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ymtpmafc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ynkdlabx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lythkidu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qytsihkr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lkruhmye.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xrgtotpk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tvejzkii.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mypsuico.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ujhwjgpp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3opgaiptz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hogazqzl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ttecduid.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ltafzeew.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rsvklukr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hipnoybz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3sxmxcfgu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nuuwwrsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3asgigeta.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3whiuzgqw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3peltaxcu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nmjczyjf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jklzfffz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ymbfrctm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ometasep.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3reuvocgc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3usuybgqs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3htctsvgm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wkquxkfl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3riqpvqdz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3esjwfiqe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jggdbiia.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cehipkas.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwswgxyo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3istyeuwn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdzcrqo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jctddlni.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vynwyjiv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcumprwl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjkybasj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mpjiubqd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxiwvt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxupmxp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qfxkkhsc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ahxetmrq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ihssuegx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uqziqcgy.html


<!-- 参考信息 -->