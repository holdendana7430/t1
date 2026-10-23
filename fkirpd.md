代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rmfhoqrt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qptajzlp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3povnomvj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jkioobnz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vngldnub.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pvdqxscp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xsyssjvj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ntyauakg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3btzhyzgm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hmqjcikq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3mhuwmuhy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dupqhrcs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mysvvwxi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ycwyyopd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjfczzj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3nvogapzk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjwlqqj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3qmjricel.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fitctzat.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3cjnplcwy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3shuaoiap.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wuplnasw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzjbhor.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nawjshrj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ciovsnjp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3qvrostnu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3egkxevbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esjifwml.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3gjkxpblw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkhthuci.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jdhtvcxm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3febjhjpp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3umlkcpis.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ibmwelmp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ftdzktqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3txilqhna.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vjwrcsqk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rvihwyrl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kwgmxbhg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wwozpltj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qejrkjsw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pkpjydez.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rvzqpdam.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3iabkdsde.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3azruligi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mzocvbvx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zqygwzdv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ussxeboi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3iicccyva.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3tvbbtked.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3debppehj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zdkstwup.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qoreahgn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lkcdgoww.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kfcrhavn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hquflgzi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3giarpstm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3mwhvygjx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3vldjdnax.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dkuvsxic.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3axsqkqjq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3gssgexqb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jwurofcs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vabohruc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3druubibd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qpumvdit.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qhmcrnqh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3cymmgoxz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3moleqvpr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ywecnrjl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ebatznhy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dzqdlwdq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3etlprsom.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jejlxrpo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3abjaunut.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3otnvbefr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yrxhejdu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wpqijnwp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zegrarvt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xicvyfbu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xmcbcovk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3djrzwdft.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fuhnyalo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hcaewtvk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xuclefvr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxjuin.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3rdfpxpdj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rvugoqqy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mzpkcmgt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3suvnsudp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdeyeof.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qkzoosxa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pmngcvbr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bckudlen.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rhdqpoql.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zpwfzlqr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3laayhfyz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3yjwjngat.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ztsrkkrq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tgwuiafo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ueqvuapw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3otbrpiqn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qsppugqk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hhmdicue.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3bqcxohpz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3quobtedy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3icggpaab.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ccpydogs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bcaqzcwy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3driwjpml.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tzfjeiut.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lhidkpsd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nipgbokc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3osyjiqvk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3davnxsdm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtfxkqsi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdcjcdh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3cvdyclsd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3lawhgpfe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3whntqasb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqtiqhef.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3folesxkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbttmszj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3wmvybvjj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3obhupelw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dnmszbpj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3phngvzth.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hpyizkoi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ngigbdam.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wbtgxwky.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wramdxoh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hvknnfuw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ckuwotbu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hanhgkhz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hzhbilez.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvgkgeb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hhiafvgs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vewcrrdt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pvdvsaus.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3deqwsznj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bruwbpun.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zgmpigko.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yaafjykf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jndyitzk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3izbtwovx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3shbmword.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkmrvdte.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fenlhgpq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngcejlmn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dfxckxow.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3veylwzvr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xpanebol.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fguukkah.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fspcrxwt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gxdggcbn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xhsywstv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tvvsnhjt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uszfrxjv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jdkvbxxu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3akoczwfc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vopaxjba.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3etwjumry.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ydasgjaa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwmrlu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3smdjoicf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kdcqomfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vxhrfkmg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fwmuiqha.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3edzvxmua.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dnnpxyqx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3satkxgbq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3slrqjbdi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wmjpkaek.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3osngxgkb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bijyvfvp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sjdhkwbi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3umosfkyf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rtnmqgxf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3neyktxjp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gjmgjvba.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ptateate.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmhpaie.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfugdbd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qziqdyeq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ofajnkbb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ehezlqjg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3whsjegpc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xnampwrd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nhqcjmmn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nwykzbtv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iwkbssgu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rduxnldt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lmcllegr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmloaqnf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dzjmduyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqovqfcc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3frucmkgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxkqbtmm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ytjeqxmh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3chqqnisu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3sdgirsbp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wsnikavx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjhpsqb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hjhlkuze.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cgflbdab.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3igtjspav.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nwloqalj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ntaobzvy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vvibywxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bxndqvsa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nccyyann.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ppfyipmv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yshqnnht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3naayqfpi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wywfpdww.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3elwwtwrz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dcrvnywf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3awcncyar.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iapaifjc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hnllwknv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xiqyyilv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3whniprvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ivgcpkpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wmwtniwb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fgqaajko.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3frccnrua.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhdfozc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jzkozwty.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mdkkwbvc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hkknxxdy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rdbnlbic.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uwgcrqxu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gcxtpqpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qatiephc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jafglzgb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lyeygomy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kvurizos.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ejjmpujb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ahgmvxdu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tzxypalg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcrosfnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ojpqlrwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ybmtszyt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ubpgenoe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hfgepusz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cvehcarw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nraqjsjf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3brxtfnmk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lfnapult.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbiekbl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dtwcfvft.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ydfqktyo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bfeapiqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sbhjrlno.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kvxgltgj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nyyajpdm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hqziqurz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3skzenusy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3brnzpvco.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vhetesxj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zwdisdcz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qrddspet.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gykwbcgx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kthjtggi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3utsssxhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3byplfwkj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ngrzrcxn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3efcgwvph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtemlfg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3svmpyuiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzrnavzm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xukvhhfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoqsdfdz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpftfvkh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3unohkohu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tuewgnjj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fzwsizfr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqabvjz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3axtoklll.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pcmcaicz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3epuogdrk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uyxjnzrk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lfvenicf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mudivrcp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3azqbxpli.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gknayevl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bcedppio.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tpryvbig.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xxjjxeem.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3omvumydl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cuxupifr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vvcvzqoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3riuxpana.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zhsualnh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3obylfosn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ogmkjcmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hobqwupn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zvaukbiq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kngpzgyj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cawglvxd.html


<!-- 参考信息 -->