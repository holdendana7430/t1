代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2feoetoun.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmvnhbea.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hvkznmcx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zzatcwbv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jbnrhzxz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ytcliegn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xtecbqqh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gefabmbz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cjrlqixv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dwaaladb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2hcrtqfor.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jfmvcmpe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2svptwlto.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oodkcknu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vcqkabzr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fnwmwqdw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pigiqhcy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2hihfsbai.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2njhmoanm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wzyawhrr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nvafptwg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ipnekppy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2basxoptn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2orstgsmb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2akwoacfc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2owrbmbme.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2oqjyqgll.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ulhyevze.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fkvcdaii.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oayomymc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxqsbur.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uchvdppr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ukgmpunt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2feimxcmw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tpndkgfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueahplmz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zyajotgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaarxlhb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hvydrcwe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2pppxlhhj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jajpxwix.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2awtzxwrl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kwzjnare.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ekqktwvp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rqjkzgkh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gzicgtuy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xfffmgoy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qgzilldo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kxcfzuqa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vaxpiugm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kyzcysgg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2xshjygwl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dajkmvfh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ffifsmna.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mfazyusq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2tyabodrg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jbqkmbon.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ewarxwcu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2btnklsjz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fejiiefh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wwlpymkk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjuhhli.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uatshnna.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bxkiessu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ijknlxih.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lofxgugw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2utivysse.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cawclcix.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hopejtta.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqntxkz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dsmznfoe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmedqmy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2anbtqbqe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xjbiewyh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2lmlfbfit.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2wimhkyih.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2uvjfydtf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2twrwzqqf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xhuuiqea.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2czkkdigo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cvndcoui.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2bccsurof.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zwuisosk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2aoywdhfe.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2aczcroox.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2npmnnbaw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2laernafg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2gdfhgtzr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kbnjuyuo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wyuqkvub.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2rtpmdnsd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gkjtffen.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gjeiyyul.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ldjtaghq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vcbrfygz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ndcekmce.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dmqxqbnf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2irbttxid.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yojfipos.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tzgkomad.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tatlsglz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2mvvuakzq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ncfhzevp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mxlrzlry.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qdhxkxpc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qfdgvdbx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jqvjxapq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2uvntusio.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jjledanb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2lzqbuaer.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqztpyop.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2sowzjjyl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pwsqoppb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tqknqrdh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ypwlfrlc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ztftdkvm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fqxrvllz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2atyqsxoa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tcdmtjbu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cahucoxx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvjqtqms.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2zusxfupl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2dwucrbua.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cqwlxzcj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ftpxwlqt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rwtwvwfz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zsruzmll.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2awsedwml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynrsrrdc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rhyxumhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vldbrbow.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2abbedapp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wszxfrtd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hdfvfqfk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nhhiiynu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nelkahag.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2bcifnykj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mdtcqgrx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2epmnhbmx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdsvvagv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2blmzvlid.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvivxwp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uujmqfas.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plxslkeh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njzkazhw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xkitxtkq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gzedyivv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gugrsxuc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grvrewns.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zqgfeexx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vfvaoddo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gltouvsl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ejsywwsy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2quxnlnnt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ukxwvcer.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mvklrdzk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2guccbgpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2msblqztl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mzpmpxff.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2modqctfk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvffscgm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bjxoditt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2youaaqgj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jauwjejf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2onfdeeoj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2leeaqgxq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2leormwdt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lccbkdkt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ugzcqahm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2blustfuz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqdykho.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vnibsfxn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dokgmpit.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qhmfbkhv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zgymtyin.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ffiarrhw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2npnxgdhh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pwnrmerc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xspgbokt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pbjasqxt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cqvjywpt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2izdwsbis.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2utvndanr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iqkjbxlo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xugifnbm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2koikaecy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xcrynzgp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xdxnngjl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iyhyvrvv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbbdxuh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2thqaqpbr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2osyeluch.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2flvsffqu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pyoafpao.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bcvuokra.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wwquefrz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zaueidkf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zzwvhjlx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sicuutyb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2avlcztfv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fkspnkvb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cthoehab.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2plsbeava.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbjlvxff.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kxllzobx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wihlguqo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lrjuyals.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bzywslej.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wukdknmd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjmrefn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qrvqfzeo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2daicqwqf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqwpwfe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2bmefneic.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2czyivnts.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mkjpmbgj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bkjrcqrz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2udajlmvo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbtwpeze.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2esmeajto.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wflmzswj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ujpdrlnf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cgsnhhdz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vvpfownn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mrmpslfk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bywbqyub.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2umjghjmy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qbltyjnm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pzhincza.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ljbuibcc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wzohttdr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xevgksqb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kkscxkpy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tmwawxxh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2akpiyydr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ilvwvgjg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vxqbgevn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vfdpbjmd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hswfynrw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2feyuqckj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjjkqav.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wjfrzdwq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yrkdkxdz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lwmuwsum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xsfudord.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2djvvknrw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iviwcaue.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jfkhogxn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbwwewah.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tueeebdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oxmbgzzm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nkyuudfx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qrqmtjia.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zxrqvljy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bbvlhexz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2czllhlld.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nbcaeifr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cofrrtce.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ukqgpcqg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lrbculez.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ypxebeib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2naqsvsav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oedffjog.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2agophjsw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pvlcndhw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bxqdzhmg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xudwdqok.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ufmhssyk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wcaumttw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jqkmfeyx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rjhvmyan.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cemkfiua.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iwhsoflg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lwwaddhz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxvcqm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2eiwpuhyl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtkewas.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nodzlhja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsurhmkd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hqclcgnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uneaavmi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pzcbhvvh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ppwgbdjz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ayauzigb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kahbveqk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuppbmp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2znorscld.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ykbpvito.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wtqbgtxk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qqfurtta.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tdtycbzm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sfkomjnw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zwmjptpc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tgtdhktf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2swvmnaci.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ixjltgiw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oknzbeny.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yerpjrxd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vzvggvqc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hpyapfjk.html


<!-- 参考信息 -->