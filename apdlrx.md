代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2xpcqsrfz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tturwcem.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2irixbkjn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vkjjcvgl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2visxteka.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cefazvsy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vkikmaur.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ecyjijxl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2owwkwikv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ltawdcsc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tajmjeym.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tsnszkdj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2rjtthclk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wphcydkt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ulhklahp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpprdqni.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2eylixpce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktksvmxy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rggaosmn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2meuuefdo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lkakxypd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xjwnebkx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gvnkatrr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2eiavqmuq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ylumnzwu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2mcmewhkg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2pkdognia.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kntltvwm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gkzeetqd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2idwmjupd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2gmvsiclq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zoshrrnc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2csxndmwc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ilczbfcz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2njxjrmia.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2axhxxgqr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2rembndtm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2nboatdcu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fakyqvdl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mkvunsii.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rqhbrdgz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ajulggnw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2szgsobmg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ndpqckra.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2poqnkggf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fjcbejvw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ntstpmxb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2beoeykqf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwnyuev.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fphaqwkn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rjnbofsc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfcickae.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2gdbqsxsd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ropnmvwz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rjyjlsaf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2trmnxmfg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jrgnnzxx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ogybzkuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cymemfcz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hystgzbg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcplgtk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2aljxrpdd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yatnwjzp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dmkdbkuy.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2mssuicjr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dxwpulua.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jwpiexng.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zcmszyjc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vexcmhth.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2nwblfgnw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2tvcdniio.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2noclckct.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2arjeprjk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2osvcakwp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2pyyckimh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cvkkkjgk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yqxrnzqt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fqchbsvu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2smxqbhpt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jnlconxb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2myqlygqi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2bgcynpia.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pcfhhjsq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fwbhuvdd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nbobbilj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xftvrgry.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2djzlcpll.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ftnsganx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qptikibz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mplybegd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2wxylcbsr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2vrohbopb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qhfefpmm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2favvbges.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xfiytqbl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ljkmotjj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2htnvidjp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qxtdopbi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2btaeaaqe.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2meddmyng.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2evyznwgu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qotcpdtj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2egogaymd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qpujvkhz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfnzqsg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xnuhyblj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yuoqmita.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjpcvdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ichsrvyl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2iiomutzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzincqtd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2bjzspetu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bngtshny.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2envherwt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zyvjybxa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyjbkpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2kbywukij.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lsadzuis.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2cnbdqxix.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbfnuwt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2uytbmnvo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okbocxjj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vqlzciwm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjaocxj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hwxyimbt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iuzuprms.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kzxvcbih.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mitrjwrj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hombtakw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2amfipefu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uaclpfii.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rgpngjjc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qavdffry.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqaruefo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2uiuzfygq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2svjuafrx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tyatdvvf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2hgcsyywd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2asmldtfo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vcpimtdr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhbubdxl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2euonumjl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rtthggrm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sitjdiok.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjfdjcx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rewbjdyo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yzwqpwbt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zsnhuant.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tumvdbxd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qyziafzv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eyixxehn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2huhsvxym.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vzagxmdd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pooymhgv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2opzqanvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ozqobjww.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2bvjxahfd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2issshuiq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvefumh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vbrmtgkv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ggykjems.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vqrunjsv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmyfrzqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vymbqtqb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lmcfyzdb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yliwwgpm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ohyolnbl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kprobuch.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2opyfrpzh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwsusdr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cgkzmvqc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qvrudbws.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdyzzqf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qktixcpr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xkgrdbsp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtimsbkv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ajzdohzk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wynyzuhe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gugamisj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gqvvktbe.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2isqaosvh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzwupxje.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zjyrvbsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckescebr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gawezvhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iorjypik.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jkjkrrhk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2olzrsbjj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vfhqmwyi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rwtfshbp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kfqpskpr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ddjbxeef.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nbmqruaz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2sybmdohd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wshrmsnl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ebucmvmm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2raogwyve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uiywcmtn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yyusrkbr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2huucnjke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rwelnqqi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2adtrhooq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xngxessm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ciemrmqj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rfrsoegk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ajgzbjxi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2srltaiwv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tyehwrwq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ccumsosn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2uiyxfozl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ayowmxob.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xwmdxxcc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rxdvpiyp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zwpzjxqi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgneafu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dbsfmnry.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbcvqyqi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xxyxgbrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2viuxltps.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ofwnnoww.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oeolabqu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nfqewofg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2iedutkvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fckohdnj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hksfwdao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2psiomsmt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cpdjpkga.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2siwrrbka.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2oaemiebt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pwlsaklc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zptsreeo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ffsrrvkv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2adpzlrxy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bwztuogk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tllwkahk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ftayeqre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2imtndaav.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xjyeovky.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcbbceo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ibzlilgd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hrjbuarp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kcqbzmsd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ukkpoqhc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rlixeazg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2itqhpmiu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2osintjrw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vyempgnd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2blawbpua.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rvolddtf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zlotnmkx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kuaewzpp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vgattwcc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gjdlzqft.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rnvdxher.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wuajbezk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2igvwyknd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cpifsobn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cebiajjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciwzkltq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gflejgig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imbafndm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdfhwcrt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jlegzqsh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bszbyxar.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uznuqgfa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcgrsqz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vpmfcaff.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bwrhkdid.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pwbpibqh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eqwzutta.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hhvrumgu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2juwesamp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ahcsmcyq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qibaadqm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qczsjlgh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wvikolci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gqcovzuc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mwvirfnr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xnxfmprk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2udwjbolk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlatxthg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wupdhzss.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2awnepxzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wkiljfqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qenoimri.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ajwewauy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sqjooqif.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bzbaqhum.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2krhfzuzq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2znwfxipy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ucljuxlb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bsnmyshu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2coocmmbg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmjkmpu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2umcyikns.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lbzloujz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ojnnvzwv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lgpjalwj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdaxypun.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2awkvmoyb.html


<!-- 参考信息 -->