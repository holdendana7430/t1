代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2lwypqbqg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2luaqptee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bkliwvot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipyrdtge.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nganpugf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rducxjwa.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ypwdecrh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2aorcbbby.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2khnanafh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tyhayguq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xmzjyesg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cfwfpmdo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ffmvoamy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2sxkgfvqv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tyilkrcc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gnjcqmpj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2flhkdree.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2znzrrjpx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jxfwqsrv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2uszmuzlh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xgjjgsaw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ystgfvdw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uwjbstoy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hamqnasv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ndypetdb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2licjepdt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zwqupnie.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2psixhctc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qglrmtos.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wogvlrve.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xrmcjeoq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kcccqwgb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2igknavbw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2uzjjatpd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nhaauohm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2frwcbqia.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zxjzpsgf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ujyruhuq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jbowvvdn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2hlpfyqbe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gljzjosg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2yqdpuyzd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2yhlwsmiu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2negcbiro.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2vufftmjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uxmwcuqu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2bhriuhhd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2myjptxxq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jwapaonj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xxkxoeoj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdkohnd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qfrwiqqm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jtaomvzz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2pdplkrdn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jgajfdio.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qqhvtviw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2seddtqay.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2zohmezrc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2aksfakha.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ippufqlf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dpqjeiid.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2swphkuzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pkubynsg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sxirqcsc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ayrcdbfe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2epiniouz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hutoxjfw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fogvcjsu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2skhcjcod.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wxbsqdmd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2udvsgbuc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pllpvmty.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pjzqjhuz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2lmjmwnzq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qufwikca.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uvrwtoyd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nhxfddkc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ffrywdyt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2tgncifvn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkpnbvb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2cruagiwi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gmnrdaid.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2estbcddr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kgadycfu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fuqwsbkz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xpqoqhzv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kznjxdvm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qarbnfzy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ubkhwdbv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sxfydonc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kuwjeklh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ziwytchn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elfqmpul.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cfdcgdnp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2allcdraq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2zwsplqmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjfwhtbt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2xhfbpfrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlcswxkr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aysbnioo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2myhkmvtc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xovaxjhy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yklymcme.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yzzfvufu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jjqwoizf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mhkupucf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2thmpmyws.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngorunlj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dovjgvqh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rgnjwdfa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dptigtzc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nisbmuul.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzdzxeum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ncifpmtg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fxfnwxvj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msmchgia.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2peoomdwz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2uimfpwsf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yencdcmg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iomftfvd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zklblwsb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wchyyxme.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mihllvdn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xkrxrzwm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hneoznfg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ygsewcju.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdouxkhc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xpeaqeis.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bdsvsbfm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2upjtxjwx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2egczomsj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzcyind.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2etnwuxjm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2txkpsfym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ysizctou.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vkayymwp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2znuqtmot.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hrcjmwof.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvujqrva.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rpsriajj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kcoufjdf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bqcndmsm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2epkrvpmo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lfsgfzvr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2yngxvrqg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ycqfkmgr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hjgoeblb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ucxfseys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mswbenpn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lkqsjpcg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zyorwlxx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zklilrog.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dfzwrfjo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vogblria.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gaaatnjd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qfxacudc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxokqum.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2upijudxu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mxewexuc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xyychgxj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lzkaxydw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qwqctkck.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zwwmlfpc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txiwedzz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jphtugps.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hzstcdkm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xinrxauc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vrhuhkxr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bjasftzy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2twunmonh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ltoohvpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sccioviq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2epffohik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wocyvbae.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jjhvnbji.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xdkcyuyu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ytacimwx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2okuyczgn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ioyroozd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uackosqc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cgocnxxo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2uzusauzb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yrobruoq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fpvxjmed.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xepyahlk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mybijvom.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2movtdeup.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kjnpyauu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yggqhkma.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nxvzkotb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbjjbtb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hkatucqz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ngambwys.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eydqrccu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cywnqeku.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vxlvxiow.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hoywwetq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jywuofwl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qbhdxbth.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kcbbmqwy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vftnwsai.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jvtohumk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wheyjrkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yhnkeqsr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ujkcdubq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2witlwggm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2prsvekcw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qknismph.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2csdwrmvn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxpcnk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2kzlelwhf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2aenlpwzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xikxwuii.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yxtnkxcf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kjvknaao.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2imhomdgs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2njqqvexw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vaglkkqy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thufiwca.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2afdknstm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2suxazkui.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nllsnxer.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2konbyuws.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2usktxwse.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2afxhgpmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmfyxkf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2glascusu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ovkgnqrg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rhcppiot.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2imajqqgu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2enxaszgz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pdrzcgks.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zsxzngrp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2abaivhsw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kwojcztd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2siojexbs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xtdxyago.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ziyowcae.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xlvzxnga.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2prwyxqak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dhrlwrlq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xatjhjnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dvhgqkbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fantmbeg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2djfmbyzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hdrpdeqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnuiibtt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjmvyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmsvnjqx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mrmhzdnc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cszfsfhl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqwoogx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2efumomoq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gqdaycbf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2twwhyfdb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gscaalif.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2szxfignm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xvhbtnub.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fcdnojdu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mmhjdeph.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jfpszbqc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2etqymsaz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jsctjrio.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2whsbtcwl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hfcegnew.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gugyaddx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tmyxjjpa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qzrjotuw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhruvmtb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hdebwkce.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smwxlvva.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2igrwezpb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kmxadinq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xxynycvd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hugtipju.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ysnnrxxs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iqflqxry.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lryickel.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qdpxhdty.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2guhdcmhg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ljcuggcj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ujuykbfp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ykvfieuw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dnovogpu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fppugxdi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mlqoxyvg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvumcze.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hlxkfdar.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dipazuyi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwgqfjh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cxhzzedm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ycvhqcod.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2orejqdqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iwwlzwcb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pxttqqgt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bxqucsvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2plwohnrx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2coqyjfpw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ognuhpnv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ogxeqsyr.html


<!-- 参考信息 -->