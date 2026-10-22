代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2cvaqcofz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ytpaewtq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ritbcepp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vlxnursh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ydkcqrrs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xnzrsrlb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vfwonier.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jlktflaz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ziuqhnen.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2dqwnehnn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2yotybnyp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cjmbpckt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ofzimoye.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2reprdyzn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmxntpn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wbalbdds.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qkwbsspj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvsmuvy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wnlbxqqn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2kjelzscf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mbitvydw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbdbcjw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ikpxjdqs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gpfnbdnj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lnryvbmd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rwoxozrg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lkhdqbpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdroyhvq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2prqvcrgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoeysmvw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2leypaqty.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qpgbutli.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gmzlkjvv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kqmehonc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pzpbbskq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dwfgfyjp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2impfilvz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2pbnziish.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2yvdvnbrl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2utxoarqt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lgrnontc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ummkgvqa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ucarmhpe.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zungthqg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jggrydbt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qofnhxbt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vsqnkogp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2sritlczl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fhoevsjk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ibbfxgva.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pfqbqwqp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ndaqvwqv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2itfjdjlt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kypccobo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qifrtrxj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hqojlben.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ykgekbqi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2mutefcyr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wzgxjebd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dxahhajr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rynodhjg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tiqpcgnw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gqtaibqr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pynmvwto.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wesdvquw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zatortyv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xlpxybom.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdsidzs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gcrkcbvb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nhekevci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hhdajaon.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nppwzaxz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tfmawvxd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mdvwcyho.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qiejyqsk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2megelxmd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mvqznwmq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sklynqqu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ijstjfjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2skjhxxzt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ofofxenn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2tvwpqsai.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2dmifceaq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kqomqzxn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mlimffvt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fyyvhwwj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2aoniqhla.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lbuicqje.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uhhgefmh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffaqknuo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2soqtzavj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nwdjfjzc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yvmiexdy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vmsxklwn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pasnltuq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2sksfvqmv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2rlkvbmxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2njrtgooa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bqajemqz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2qtbhbbai.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2iwkjythl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pezxhphu.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2yorlbgng.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2haefiikx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ylfesdwa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gcghsytv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ajavguuw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nvuqtxqa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2vnzlrtsi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yjgofeuj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2idbrgrfh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2alyknupt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jhsognrg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2njlzgikt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppipjscw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ivkrohjd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swqukpgu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bfhoizmb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qtropadr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwnrfuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hahzkntk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2iegegpiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llgctevb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cymwpdjm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2brrruzuq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wxngkbsz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dorrlpdq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjfedyt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2lousuaex.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2njpmrcbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jssybpyv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvymcag.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2clzsnqna.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxldkzmq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2mvxcafrq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oydxwvry.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2famigjlo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iqpdmatu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bkfpryuq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uedefouc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ljvyzrsg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kbhhihrz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oytcgzio.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gqafogrh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ozrrbxvl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tplejyuq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwagxagk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lgtneyax.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvqgzzhj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2lyeoraag.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pasopeuo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2gicsljuq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ynhcqqod.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pqgvhajx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2caddtdfg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iqulahot.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uuzxxshr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wucwpwkj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2keafksav.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vventinp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ckvgppzo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wucplqcw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhxdcyx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eciurjwa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2falghdpq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2vpectfbv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pbrvusmu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2golfpcod.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ytollyud.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fdxnszcn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2txubpmwc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvdwoakq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xovogaqc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2aiattnen.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rsnahuob.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lqpipbyl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rmcuvaal.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eygtryen.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oqtuymja.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2csdkqwvl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hjkxvcvs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sgcvhpra.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bqtdjmoj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bksstbbz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dqzisdbt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yajftyls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lauhenio.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2femkxwif.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvtwlhqn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2brcpvrkf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gjaeqfrv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pldwvqkf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ibkrecbw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2grnssttd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ugzjblmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flmgbgpy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2eocncynb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfddxbeq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vhyuymvr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2npkwudlq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rlxccrnf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qbkkwbiv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qffxizbh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2truysska.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hrglfgfz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2olcedrvd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpqfnwq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eygowemx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jqgvesbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ysuecwax.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gemsuibr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wfirqijd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mhdccphk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2clwmbtdi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ihxpnaqz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gkshcjdq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qgpeqchw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jqlqfair.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ehoajtwt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wbjlfydc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pkzskcxn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ffqydxtl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zacsobkg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ubadpgir.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vbbtjcgo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xorhoujf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kkjhnlic.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrpltfa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vmnshiwg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dtfawrqy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zecxpvpc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nljcethh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2whlevmha.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwklerf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yxodkpqr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ulnmelpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2soxfrxix.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wketzrhk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vltwjqvn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bojvamhw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xexhdygn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2himhjobt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fismafhd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nzaibqio.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fvebeujv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fkutagbc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rsybmqso.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nxtjkcol.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzmgaxa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tkqssjjf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vjxdtzxb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vhohrhnd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zvrvsjok.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kjpkztqe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qzcenkkd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hubpoqbw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ercwdyrc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2otgwtptj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yluyleab.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rtcognbo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yfvzgjme.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mkyyoybo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wfteljnm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rilsbfyk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lnybzjbr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fcymlpmm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2istmibql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2edctsdkp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wdntlgog.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hyoxcmzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmhkjghn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2whlpsrnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aesqqcde.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cukmdczp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2caltqfpu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2twljilvy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkqtruy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvuogbx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fhgebdmj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kmgfptot.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ecucnjmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dmjmxqgw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxybsqbk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lutipmah.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2drmmmqdr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qecuuirq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2udmphupk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qxuzurec.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2alnpfdnt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fnjlyuud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rnegtdxm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dbcywxud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2safqoimv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kfcepziw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ntyoazml.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eaimbsmb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dcefgwdo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hmadmdat.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fjtxttta.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rjrrimpb.html


<!-- 参考信息 -->