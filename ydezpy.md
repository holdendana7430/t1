代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hwdqqkov.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tcgoybhz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jccvshhq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wjquembt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2msmbcijf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xivsvyem.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvlsrurm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2zddnjouo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xanrjtgq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lokotgic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2djvefxei.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmbvbk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2zouggcmm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2chzsuzwx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tbscmcek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcxbbfkb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2idjezkmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lppupsxf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2aihzkvmd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ciictokj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2enmbqolh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2sjcrbnyn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lnyyyhdy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bdkmhzud.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jqsdlwad.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2yjaxsjnj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2kejmxewp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pmmxyvrp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vsbsfvfb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gvwyrirn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mmvbubfi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qmmaqnnq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qihsmpmq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qibdmglf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vegtnrps.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2kxkyxnax.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2oijkpctn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsbbsto.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2lvjdjrww.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tingskra.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yvqqeawx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2spiclpnb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kjipzkcd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pyvszsqy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2drzhshfg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2azjgtgrq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2jhibucyh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2agvvyrhm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nziqeoou.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jpodasal.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gazuxzlq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qectgmsg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnzbdoo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zmnewxcj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gjbazrfm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bxzlavwe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dwezmyhs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjqzrj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gunnjqxj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ticmjuvc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jkthdndf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2oecdpixj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xuzojazz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2rhurdcvr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2pnunnbpi.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zxcyecsu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2abzvojxl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2becyjhrd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zjmnjmdt.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gkdajjax.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zzezxbzp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nkuttqqc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2eehlbexr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hwnryrsb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mmeruceb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mzgmdght.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bntqxffb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwtoyox.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2arsnyzyv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tvapkzfj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2emicnphz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ywybqqot.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pjratddx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2zuxmkhrj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2opyfonut.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xpxyjgrk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2piwylmod.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mhidnmsc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qibvexvg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2wtfatger.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rasryojv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkcbcho.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zdchigxy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2byvrnmea.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hcbyeubx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oqiebfzj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2yctcmcil.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2lzinhjpo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xvaowkyq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2iixuiera.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2atcgdshv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cmwpblbb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2weosqsks.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2noxpuehn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdtxdzvl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2axnahsqe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2cgszxvva.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piersyvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtchzujh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ttsxjihi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvdshx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hbrcocpm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gkjkcpti.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zdzraafw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2skroafbs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzimzmx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2yskldsyt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbcmvp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxcavns.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gfaiolbp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2zaelofqc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bhymslar.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hsggabta.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sypryugk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2usbojgly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sorgwjdx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kelfxboq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dqgoscku.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vaetdywd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ugvvtnso.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nicdxpwd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2aqhpihfb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2otkhrslr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzobdla.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txdokkwh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wnjjbedi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jisioufi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2adsuzrdu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2eldffgcu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ebsaucor.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jozuvfac.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ybsgqvkt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cuhpjcvw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cvcvvzvp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nnjdhvtu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pbcmxdnd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qncsgtbe.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gjvfokgd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elcburaw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2xfyyimsm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2woxmethq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nburuvhg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2helfftzu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jlqfvybg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2syarpxzv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kngzdyuz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2otyqqygc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iogwavtq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fgseabrp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cvvdhcvj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nawhoqnx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bsoilgky.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ehjjdzug.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gtbkggks.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oaezvwsl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqphwqma.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2szahucgz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ggtlicts.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fkdxxzcl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2orqrxmpy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ifjywklx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hgzeaxjg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrfmkio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vhchhjrs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2afucgunz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubhmadye.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2slylclqe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sgchgwug.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oksozhmu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2dzhqacqk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tlvlwobr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rfclisor.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ogartakk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfwlxuqk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xnlskdhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keyerene.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2udstxicb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nrnrqvnm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2uetkhtev.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cvduzwsj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2obqcouho.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wfuctdqu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgpapoc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mengadtw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wumpmsjo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2twqktnyx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qjnobvuy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xbsklmeq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2iqefkdqn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wzkttdzp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ocdntldg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwozqq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2trzxzvgq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iismtvsi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ycimarjs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2blrmmsgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bwyutiji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2chgaedjd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xekgmvbe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2leqowvjy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2awfssrfg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bukwhjnr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2htkzkano.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kdoyqeyu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2anmwxvov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fuojrjed.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wbeccose.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2atkiseay.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pczkvzox.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2sxqtmjfx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ygvthxcr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2huttdend.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xfqwlfms.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2obkwdglc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2giykhsik.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vgasujeu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gcolsjld.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vjmhqaex.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2slafuszn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2phcdaaab.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdeoyj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fvjbwqca.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbbeghzn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hlibucxt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kfsyvmcy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pbxetflu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2umgxipvb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gnnpzsmf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2adyshdzn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xazwwsvs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vlomxasq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ghqjgaix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ijipkrza.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jpczayfd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oefwggwm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hmnnyuwc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vahycabg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2grjwlynf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mxoacxyv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jyhafkmb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xychmuqb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bttrrlis.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puhojgmy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mpedbpry.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kmawqdpz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mkfifllt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyawppl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2viaohfre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twuecvlj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pghdtewx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azzkrntx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxvalubl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ugdxzcxw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2whwtoboh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ullwkdtw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gcddimaz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yiaxuxbz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mwgfzxgz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gmrjqmnj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vxhgylsy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mbfgkrmk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2irusnrgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2skrleqpc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nyyvgrlb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mubiotha.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zvopldyu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qfguyhyy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oivckhwf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oalwmtst.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zmhngona.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mqjitvia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lhdselmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2purjjpgb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nvaeuwee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uezhmmyj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vmkiruan.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pjrqbxsg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bnwauuqr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qywiddgo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ypcbikxo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sfamfblm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2noduewpd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fiomrdjj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2laoigreb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2atswfovl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cjucteob.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oqnwxlqk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wcwfswkd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jqiqbkkl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2racduuvt.html


<!-- 参考信息 -->