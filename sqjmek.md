代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iaezohrd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fommzqlr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qaltwqpq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xkzifybf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2shkbwsst.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2iqzjeyyb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tloelpom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zxhcximy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wylpjbpr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ygnyvike.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2evqpsaco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vkeotdlq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nfpwrxet.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2crcaaokp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2nucgakcp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jgamcdxl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xaslyizo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mguigzae.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zmwckmef.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2yrsxmgbb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2kwqudsnp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ridcobjo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zyrlzjbu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2cqbkmhzx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bpwhgmzs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lboxjfre.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkepduwu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2soqzdcui.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nxehtdpy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rtgvalyx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2iyylxdif.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vhrdqbss.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2luqjqqzi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2lmnzizxv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uxvvsrdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkqtwcvs.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ekyuamhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzgcolkl.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nynepiud.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wpbucsiy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2opsqbvmf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tpuugzlm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sjxqxywf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uejuehmb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2gdzizthy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2tjbefzpc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mbpgxxrl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ijtpyfop.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ghaarzvu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2flovzxwk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2whhymhtc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hmoqhgox.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2sllboyib.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2uqhpdxcr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2stcmwyyw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2nzlwwhqe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2gxylrnhq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dixladkw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2inuoujmz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wuzkuifj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mixwyrsq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yutmyhgt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lytciube.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xducbopj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gotdhzza.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dnkcmkyw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ulioahhw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2nvbqqzdg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ifpdgsjr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ssqzjdem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ayvibcjo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qrssywic.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xdvqkerx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vcpjmtnu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hthjreip.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kcwgrhxa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2omipypvl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eeaeuljn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dykesqyp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tmpedefk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gocnwhei.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nnqwecxm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjbycd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2txlghgnq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xbvqdsyz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vtwnvpal.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2dxopalcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2eapqhvbf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2omtpagse.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xfpptiyo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2tkcukqce.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nprqqiqj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nzmsbjof.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nloqnmhe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2visaoxhc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tadnifzq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dlrnnscr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvlwklc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqzxdcbf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wkmqozcx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dlrkysct.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nlmwjgnb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rdagijze.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2xkzcgcig.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2awmbybrc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2zlrukgcf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qltocybz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vhhwbheo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ophrjucy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jaevdpib.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgdhzhyu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2atazhbku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2lomozjja.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2cniotqqw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jpomysbr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2yfowqzek.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2xiadntkh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2sbekcrax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsudwf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2simcxmqa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2abbmfrra.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ssyhueto.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vojrwvnq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ldnesmbm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ubymcvsd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rendmkad.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bnbdcwfo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2myiljvho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfaxhnfl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2edyvjzeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgpmljjc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wbjyilfg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jydwjlll.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hdxxztzs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jdcrrkxk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkplymbq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qluxnbmr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2unpjwezc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zwppmiyt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avhhjcnl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bbxvhdcv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2nkiegtrn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uytqbjiw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dequazcc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rblcepbe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2amsjsoyy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iocdhxxu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kitxtdql.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ilitznnk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wuulyxox.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2duyjaigs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kqgxdjmp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkihgpco.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aissnouu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2bviepfbq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zgxkzjtg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bbdacecr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2thbmkxoz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lshvxmnj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bierlgiw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2oautjqms.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vfmkyygs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gjwoebsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gewwwheb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqpjwfa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sogjsgkd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ostvaydm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2cgxfptpg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bhkxtjde.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nrdrudfn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zygbhpql.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwcrgthi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jfgzypwe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yxmxbtpu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2niqsoeao.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2frtliztj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2goihjjoa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hduvtoyu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2getsgiwk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cnvunoxu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gpgxlsrs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nzcgggus.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2irueawtt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pcpnlsao.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2thdolrcz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gsnnynbv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrbmcrp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vfbrhmei.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2chlcentw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vsuzyxuq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2buegbyqq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2amkghsbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vytsbzaf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zasanubz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hajtkgcx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2isaomufk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2voysutdl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2geoquwoz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fcjmcuyz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zcptpxbr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pfjnjubo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwadywwj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gukdqmic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvurmnae.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jkawgziv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hakpsdkh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qhbsdeon.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uqcbffaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cljfsbkj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pgeiptbk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yyacvszd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2aantxqxm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tussqrud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2liauberl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dajieabl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqofcj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zhnrvsxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jyrwahtg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hdgswmmg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bzokiouo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xqlesuhd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hrzuhlxm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lgsdnnyr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqibmxcr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hogihnfj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cwqpddik.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkogiajr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2etiwuqod.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2icoequgd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hzqheqlc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ycmlzmcp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rrsrjaha.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fcfgwbgj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2chjbmqad.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xpjjspxu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qshoikhx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bcdkhqal.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yldcqemh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hhgxgjtq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qxemyiao.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrcegqp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ctlyhvrs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2eepmpuhy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2smkbbgco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfvkzxol.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gcfvhecl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sjtrgkrq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tpzkngys.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2efwdzqag.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kubjgjrt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctsyadsn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bgcrdtbj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wxaltrxm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2slbaspod.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vxhoivli.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cqnfxyzk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wcazilcq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkiacnh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dhbcvbts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2eotbbuwv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2munsbflj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2knnongbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uqcgaqdd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2thgrnvxu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mpasqsmi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxltxl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2icgmktjc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2npchzhcd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2crtqkpyq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2elqjozxg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2qxbyumwo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yuxnkpjx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ahrgyhxe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2muqwimkb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jnsqqwuh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2iqnmkbqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bgpoyiuc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xaoijzcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsqzbsoy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2heqpwbjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvcphdmx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bfqcpkam.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cgpoqcpo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gdbiuwdx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgehraw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hbepzvep.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2takxomaj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uuxwrhwq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ebkbmnnj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nqdhlofc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aalvcudw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nebycrlu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jorzxqsu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gxftyuku.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iqkkrhnz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nknrwssg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qkfiziad.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jlplejxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gardfotk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ychcriog.html


<!-- 参考信息 -->