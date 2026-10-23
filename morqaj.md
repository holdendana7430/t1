代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ozkqyygd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hnsbhmqv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3eprclcqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wquouers.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3dwjrnzis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tawmrdqf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hjspivhz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kawyjtho.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ewmvrskq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fgmxgghs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kvoyrvyn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ovdvawtw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3czgwgrqt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ejdqjziq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lajswqqi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nbwylgnt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zobsngyf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rhddcyox.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xulwyydx.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3djbhlequ.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3nifhbvfz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wkickibp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3akyiycuy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3zxadoefz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3dwkgjtqv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jmmlycub.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3bjpfxgcv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qgjlueud.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ytahwmwj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xzzwrjsr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3miisjxjs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ztnkjlpc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3geglcnnt.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wdpnyywx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hyuhpsbn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3mzoxsujz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rjpgluuz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqxpuxi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dfnlkpnd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jswfjeff.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lcsjjsku.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhsomdr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3msstsymk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqxoikt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vwmshzgb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qmprkpba.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3faetwpwd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3msldzfif.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3irmbnscb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3gqbqalwp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xdvwasdy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ygsysdzr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3lygghvow.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3natolewf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sosxglwa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kmjlherj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3oqnytoyv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3cavcnkxm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3suuetcej.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3voajqnmx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vxwalnhx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cepjpyvd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lrgbuued.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3yoxjpwbf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tczingao.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnvrkkzl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3sfiuuugv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aisuxjaj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nadgrzvg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ojgiepsm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3cxuoevlx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3qlkecbpj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3nrtcstjm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3suhcdkwr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3hikxcawq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tkxqlizp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3iprwrjnr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3whivbzta.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3apjkkrej.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmcvlzp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mshtjrgp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ughjpqeg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gdboxivp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3edadmloj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mwfmedtr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3unqzefus.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3pppylctc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pdmuqglh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qotlrtwu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ealzkrqt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uukltwwh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aarvzozp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eemqfxiu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mjzalewa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ynganekk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxlvytjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzqcbvbd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3jbcvqjvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxpfxdrg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3nlkhehnd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwmwqdb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jurigtau.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hltpmvbt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nehgbdms.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hdzpdioz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghtgdsnu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lwviwczt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mnwviucx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3cvfhmnvb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3buyrhwtp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwnuvtal.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vqlymzyx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owhwzvcs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxinqww.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fvqcmvzy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtliocl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jpoelidi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xpsutnog.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3adcsrnho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3robinytx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gdespuch.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdvfirvl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3czzmtfvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ikxcolck.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jobmhcxm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3obzvipbq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kcrplygl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cqcjxtnp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pievpojq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3icvejqda.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhteykzq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qamjttrb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hvphvywc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3drvtzbug.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3desuajdk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kzbmnecb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrxdboed.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tirvftll.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rabnfsyv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kvhcslef.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wsbkskuq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3olseewpc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3oetwpbvq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vewtzezp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jrwmnylr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iibsksff.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3pefbvuia.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3znkounvq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bcpcgsat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3igcywskv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3htnubxwf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xqkwvtqw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tbgiwnhw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kctfxcwi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjydtmki.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qkzqotud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ljatvclp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lrtchfbw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhijkre.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cryyuokc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bdluqzjl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlhjlkq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ivawempb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxkmzzp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkbpnyr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fnmcwhay.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3csiztcuk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lmuergbk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3detnqqif.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmuxkjus.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qxxoucoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzyxdqxs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ejqxxdye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdbqamdm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ualniwpu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zcbdbfxg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3hrofpimj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fzokajgy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ubqouros.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rwkgmylu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uegjgfpq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3laowjtba.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3krncwqac.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jqaazfrq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3llmpflnr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3iiofjyvv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vppagclj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zjgdssfa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yqnqmdzm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cgeswnuv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cmhewtco.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vjakvtwa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wyigujte.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ppjaixyz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rluvemsg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rocvtizs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ztcxbwht.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zjihywsz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3guclpxar.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3niujkwff.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3halikcez.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kgumcyrq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3azsiovbc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3upilfqsm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gqomseza.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ahknrfep.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xvuioqbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tprlwgmj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbvcuya.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zduqobba.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mzdhbboy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vaxqvwdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbfxftuz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lhrezjge.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ziqnglfn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kadikzzm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzvchfak.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dgmxryxf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gcmtbrnp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mmehosne.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xuligagf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lhvkbtwn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hwxrvqsn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcuoyjpd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3adtarfqg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nhwvruui.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpjxxyq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nnxdputd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3guzzgwxv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bjqmkjny.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rfolenxw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kfjmsoun.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pyrlvlxd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mpkhlvgv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3smbxndyz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gvdjzjmu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xkmlwtxa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3eddudkit.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zdagcwtd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lskatyqm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fgvvhigq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pemsqleo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kpcgjmwc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3juxgbxrc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ivnmeblc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3clzddsmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmsapwro.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ivbithvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxssduaa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jddtnnbd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3paofbexm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gldvqekm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lwqqrdfu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sohvnklj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zlccetvl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lsataybi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xkwdyijh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lxadwpdo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3goajmnar.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tlghkebz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wwtahkbw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qolascyb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxpbvb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bfdobdda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qauzoddb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bakdjswn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gvrooqkw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qyhuzvqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ljigpgsn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tpuegzzk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wgrogeke.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eywsjysj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hnckcoar.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gjmilikr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yrvirsaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3alpplqbp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vzxhflbv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zmtugyqx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gtrcswxj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdvxyslv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mkdaznvm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vdiyrxqx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qfpirjpo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ejxdbcdn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3unarltpk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xaedporr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obbranjr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tksabcoq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vcodznpd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3upokerlw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knkapwqt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hdcifhus.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifgucbdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3httxprla.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmaplh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ukvdcicp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uvlrcszw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gyljxcyp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mprzrtoh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rjrmtjqk.html


<!-- 参考信息 -->