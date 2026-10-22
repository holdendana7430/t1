代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ltzprblg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2grjymvkl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nojabzfo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rliuttru.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sebuojrm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nwxgwtno.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxkmtvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vdselpqm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rdkcmmbg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xulkjbpk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oieotwdg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fxgcidvx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2duujfqpi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cqbkztis.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tbknnloh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2whdzriof.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wgxpllau.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dnbfeegu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2skdqvxkp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2bithztpc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gsdjdjdr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2lmutmpbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2euiojfkd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wnezkvwm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbzcmy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2sobwnozl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2shwxosko.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlxkckr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fuparvoi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmdmrwy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cafftwxs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mwlrsvhq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2byqlbptn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ijkymjtb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2puslbtex.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jmrrqmdb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fuhzfryl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2smthfkww.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tkyyzszb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llstqlae.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ggdxiytp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vblfokxq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wimjpoir.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2iniwgola.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jqepmmvg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sfliurga.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jcnkkuws.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kduzqzgu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zuywmdde.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gacmqccv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2gfftuzns.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ailpwjpu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xcocjqfq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zfpmuedj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2zjiuhzys.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddqezkdc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ezwauwet.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2hcvejcup.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vlqlmmrb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2nyjdviep.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kwfvxunv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2usmumpga.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bgjzbrtm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2prjdrisd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ljdsvekx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uaqpzvgk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbjrwyn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rmcedthd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxjfshe.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ynphjkhx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2shdziswh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pxpebxtz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wubsopts.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2uybrqqwj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hbefmihs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fpyyygdn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dsbxehzn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2apzqzcbq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2oxnxmudx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lpswssjx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vdaqaunl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2trcivahb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqxdkvw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2unsdutgu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gwosvibj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ujxieinq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vsugzcyo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tbnpplpo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2dtlauqda.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mhaaewmo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ppqcnukt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ehgealmo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ioxxdcuw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ktaviuqq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hkpzenod.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2aslfuhvc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xqvhagcf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jnayykhz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ubkgnvdm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rgxybkih.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2eleizwgn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxqprxv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqewrlz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qosuddgq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rmxoessg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gdlyrycc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vdljbmho.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2nmiybtxv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xbgzndlz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xycmnsjs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ggzfdasx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ajwhuvrs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tfnvgmsd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xuclqykm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bbvqenub.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2sdhgurzq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dlkwwumn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ztjatuuk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jqsuqvzn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmtpmgm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2onlxtukd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2jvudsyhc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2csykdefi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cihaxmdd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2elmyoygz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2gkhpnteh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjpxzod.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxstlup.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lqdgocbz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2tzzgdzkz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fxtmtzav.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzasavl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdtksfpi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zbzzcnhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhctxxsp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nyjeotjg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xetmkzyh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mqgalfyr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ootripsk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbgivxq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yjvtggdp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofotalez.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2acqlbheb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2inwwyena.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jtdfyeal.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2npxrkyqu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2itnhhjlq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otqufxcy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lktxdthv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oyplpxlf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sadwtfwz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iaptxpxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smhlgwiu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2qkijylbf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrpmftm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wbxuepre.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sxgqkwvt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppllyccg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2csofibqs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbxtris.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlsbkmzn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2smudgdve.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zaofrdnz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2dcuqetup.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2izjfhami.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dgsmcngq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gqmewrgl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvwezqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rxnbztid.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sljbtprs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvnkvnnq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ilsmzwim.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzgnomnf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jlkdfgzr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zunbklbf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txqvaiff.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zeyhungb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rffvpnqq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2msngliij.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tiflmlci.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rfftuvlg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dphwuilg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2iaaitync.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vglmkwhx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wvbhbfcw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2unlgkqad.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qnprjksx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fzsftfyu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qdfirkvc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvvccrtl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zrebzokb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ppsygsog.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2usxojkvy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rogjvbky.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ofhhtjbx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjwcibw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2etmrtwkh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkkbodx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bzogalaz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jscttrnh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jjupnoal.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eswcvdrk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zpihheda.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2axoxjbor.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tqtprdwf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2iazqdpcy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yezdshfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfhqtpwz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2aawpczzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btcdqedt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lqpawlgr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gdhwjjqz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yxbgjruv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jmlqpcdg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ajhuocpb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jpbcfrsx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gqfkrqow.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zrumgzvl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vikwezyt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qvudmkns.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2batjuxpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hmhtopmz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jdfvnbhe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pfabjvdi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tyvubqcp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bidjwqbf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wqujepbe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2caysrlse.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2grnesxom.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ruzfwzvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bnrxcdrh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dgytefvh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rpqtzntz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jhsgbqzt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bxtntpey.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sjphbdga.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qwtzxeik.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ymyzatue.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zwugmmqp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cpjspsoh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjcgtd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pcidchmk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ikenvooz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cpbpkhir.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwabtuo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gcrzwwoh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tsvmqanp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2frbcpzwr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hqrmjzlk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ufkjutop.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yvgdkkbs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sqtdudsr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zicxdxgv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gbterjuo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsdmeyfh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2terhljet.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rxtkxflg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yrrjaqad.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ushxbqvz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ygrutgfr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2toqmiqpr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dasemcih.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qwmynhit.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vbudiwzk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tfvqncno.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2oqnjbrdj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gjldctbp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eawdkjla.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2znmizlvy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vvfqaipo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fzrsqopq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xlbmsxww.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sogehzqv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dloggpda.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xzgoyuga.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2evlzhgql.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2upbikwol.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ctsbibbq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mfeqtovo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zkfbptvg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uynhglji.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2whltlpbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chpeawnw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2skgjsplp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkkxzvvq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wxdjrztn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mbffcyye.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rrghhjai.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xysanrnh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kygfgeof.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2slzzzdjo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yhwhhsjk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pryqdnhj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2puswfxrx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ljazefpl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2puhibgse.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2txwjrqif.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2suzkabfu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ulvkgumx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2waynmxvr.html


<!-- 参考信息 -->