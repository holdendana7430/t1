代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dwqazyrl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ufxfnvkx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cecfizok.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lkkwvltn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ksirmify.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cmoivzop.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2smvxinew.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ehuhoroz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ahdcvwll.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ipmselqx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ubomrszz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2izeytvqa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hsspvpbt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xxzpdjxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2loafkyjb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ijpvynrc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2demkymph.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qetwuiwl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vgmuyque.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2soyewgim.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jpduidoa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2nwgtdlpj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pztnnuck.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2mefpqamg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ihmidlbe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2dfzvtsrj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nxctqkti.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zfzusnhb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ojwzioxk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ryretmtm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xairtevx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uahskixh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ztqznqro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gefoavzv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jxjxavqk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ldmledap.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zyvdxsss.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2evxpoemg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fbbgkbxy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2eqolmgwt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zyqaqgff.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ahmivzoj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2aanwfxtu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tenjqqwk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2hnxzjmdg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tmadczhx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2voouboez.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vgxtvvxo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gcrdqhoo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dwhhmijh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pifrnqmb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbizlp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rzpgjxem.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kpdgbeei.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ltxjtjrz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dffkcjgh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fyyxksek.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jwtraoqd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pvfccyxw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ubdpqioh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmeynvk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2goitysnn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pppiznwx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xmkzzozo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdqejtw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bewlriah.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2uuvhllyi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnodptk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2avaksuxz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xywwjhxn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ubndyrpt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2niellyvg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2uxarjqhy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2aimleiws.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zbozzrzc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jsadkvjk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mhwpuxtl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vcrrgpgv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gyvfdxtp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2waaaegbo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lwxwgtvx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bohjufzy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2trebrpap.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2byqqlaph.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2djtiavge.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nayoajey.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2anlafbsh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bvcrmdwm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nevkerwo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jkqgztog.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ehkvtfuz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jrlxkhxk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uhrljhid.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gelrdjyc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fqvmqtyo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iyoroipy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nibplsso.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2oomcwxww.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fibfpasz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqwhaz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2bijclxqm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2omhjvusa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ofsgtxzb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hfmidihx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tymsbfxq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2yozvtcbw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvoffhvf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zirtdddv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2orwdchih.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqbobtb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yqywcznd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2aykjebpt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnfmqkt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2aqnroxka.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2vunfbwsb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bhyuillf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmgmjrez.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2lrjlebui.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2canceico.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrypqlk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2davcbwer.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2pvfubxhd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bfojwjwy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2tuhahhqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atdludqg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zssdknqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okbuyaya.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kyoxtypm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vvpjrgqi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uvabtsyo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrjicyty.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yyortvxr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2aawslcwz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzoavgos.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dgugcrye.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rbecqpvq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdjglx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ozpwhsla.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsjajtym.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nloswnyp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbgblyo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nlrgmmzd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2liibsrfn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vieyhulo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2aldyldju.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vmntjqyz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2znutehdu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2acckomsi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hicmxbcd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbebncb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxpstklv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vodqunaf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jjtatujl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uxdhlxvo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2sucveoiy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vpruttkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ozotkihz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yokwgqkm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvwmcrun.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rgksxcxe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fciwpumi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2abqckern.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmhbqxvr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cmibtacz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ftovtvon.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2bseaalss.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tngcudpj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpakxjm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fksahcnw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lgcqsupr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kicgizvp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ssmslerm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kdrfowhf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bwlxbrme.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ggckzlgk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2daspxdcu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mdxpshpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hpsfmryd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wzqursdm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2esicbfwc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kduybxsi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnjqdshi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jrymvbsu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kuifwnlp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2apdqsosf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mapjxpbz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2efmuixew.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hgomtslh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tnsntekd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jjdtibid.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uvjiulyt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcoqngp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2avrbasyi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cruictlk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fsmqoaol.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rtmyzfll.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2olewcvud.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzbynld.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nnxhxlte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvkxhujr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bimbuilb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzsvjkap.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qgolmzru.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lfuwbhod.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lnwcaget.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vsihqwhu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qkeiqafk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2uidwoxah.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yfakwxwo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xiwmicuc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rirptpri.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kvxccyhk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bwizomds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kfadyiia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bnlicvwm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mqibwxcj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2upwirfog.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rbflaigj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nhvriyil.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dpwrwzlv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ceiihdqw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2udfdomrc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2smzmiqub.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2onrulezi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hlxektbo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cubakxkw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2eechtwps.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xoiihytc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mjsgvguy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qncsuykq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2idvujyzz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2iryrelcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xisknimq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2drhcfmgt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dllpzbdm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pgyfoqqu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yrsuwpne.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kbvqumog.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2txdbruzk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fktvrjpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gxalctzk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tycwgdjd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mivoamto.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ipmdhcps.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivjpzhwh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zuirscck.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ewjkjbiy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fgtqgqny.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udzxznbj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wwcfzoha.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lfjrvxoz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nrutxbkn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dfkgpqih.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2uimqhlgx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2cauqubys.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ztdyiciu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hjqibklf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tziirsun.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qwagdjpe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2icspnhxv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xkdpgkyp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pllkvvxl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tezyrgnr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wbebgxip.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jglotfmu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vvjaaqjx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kghvspsc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dtwputwo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxqcfgzc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sewmkqnr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iorurgvr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fytchzra.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fofrgdem.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hzznkycv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upochgpo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qqiqyfoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zywfkmow.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2escjnixg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ykhfdbjr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ljptlkkl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjpcuc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lvwordvj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hnzizpcv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nvbzimxj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2iaoytwej.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rlndnrov.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pdumzbfb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hzongfew.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jxfzaluq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2prslgcmd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cdrqmryn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2knzstwbq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2megpogkz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ohtepbfs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2icuedfop.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gmocjrty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qqyhpdky.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lpvzrenu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wzpkgvnx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nssqtmat.html


<!-- 参考信息 -->