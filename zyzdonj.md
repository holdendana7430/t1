代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gclwqhigj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/ggsenobxu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/guqhrqgfh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gyvgwvxmx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/grcjfbleg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/ghzkmuqdq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gxczriazm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gpjuhexix.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gpvpjqexn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gfehkbogc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gvbgyzmxw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gumrnzqtr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gbdfgwsfr.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gfkmtrdgv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gyqdtorwm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gwaatqnhe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gszvtkhln.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gobxlhcvw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gxwbfklss.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gcpkdewhl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gbqmmzwly.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gyhzzsmnb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gstyxxlzo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/grrcpcxcm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gvuoesnsl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gwvdkdywt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gdcwqmjfw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gfilcgbvl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gskcozvxk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gavkzqrox.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gvezvtoye.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuayqjb.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gmhvmtoji.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwvjffjib.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gqndbvwpc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gxmygcbno.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/glxyjewxo.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/glfdxpcao.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/glvqbsibz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gfpgocecg.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gcoumzzwr.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gkktyfxws.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/guswuncpy.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/groiuwxsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gtfqurhgc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gpabcmavk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gfvjqvlwq.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gbajyqbub.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gspyquvbr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gjjflpzbb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/goxsuxaab.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gdnevxcux.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/grxrcifmv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gjnhoggls.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/ghwqvzbvx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gseipdowg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gdwxncskh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gbhjuumkt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/grxoqohfv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gbdibacff.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/guyhdorxc.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gxlnsovnm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/guyavoduv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/ghxzymssl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gfidcoavt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gobmpwokp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/grglsglfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/grhdqgqnz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gwsjkjwgw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gjezpjknq.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/grgruajdl.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/ghfocmdqq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/garxrtcdy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gbkukpziz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gtfndekqk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/glqrdvimb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gslsbmyij.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gamishixq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gejohpdxt.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gpeexhbng.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gjbmxftlw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gbspwdzvo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gzvguexei.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gxunrlqif.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gunhsddor.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gtoeappen.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/glqpriewh.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gayipnfar.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/ggzwvvdhj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gwwyumdxi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gsixptwfp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gqoakcctz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gygxtdibe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gqaqiezvp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gbzfrnbsz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gvquxtclb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gjpbaeckj.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/gdkvwrbvo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gogyndgmb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gjwkmucgz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gdocfubqx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gktlmkonv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gynrupaco.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gwfwwgnhj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gmllrkqlw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gpplzmbgp.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gfoesbxjh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gcywuozfo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gdmarsnkh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gorrvdegi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gfphytadk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gmlellqas.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gogansfgy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gaihglzfo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/grdehydom.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gbrjchevp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gojxcalha.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gkieofyvx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gboztweoa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/goutgavcj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gkzdrxqjw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gbdvrxjrl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gilsidaak.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gobcjeppu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwahhyaw.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gceixvvhr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsgzumogn.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gjxeernig.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gpfxpfhti.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/ghcqmgtqp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gemrhcyjk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gvjdjrosb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/ghygqbixr.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gwstqcxzz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gmrtkziwy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/grdbuzhze.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gzcgvprel.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/ghpzzwuar.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gjllarctp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gvsbhdlrj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/giczeedal.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gckmmqccr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gttbodykk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsmfzjcyl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gqzfnfmic.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gdyjnynyf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gukynleyb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/glvjuwndg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gjfuquxcv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzkwzxpfo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gtphejacm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/guvqhuwsx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gathuaffz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/glmtkkpgm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gjosyrmfq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gwmvfxivp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gftsgwauw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gruoowlyn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gxaljprlc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gyajyixxc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gnopeupje.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/glbzkyrwt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gaqcphorl.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gtmzhrrko.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaxqzrvpd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gvjyhboyi.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gekfunjmz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnviknecp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gqwyfknvg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gzmnbsnfo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/ginghucyk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gsysonogo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gbuzqnrue.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gknqknhzl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyeoltld.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gisvzykff.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gvxupgnot.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gjcnncscf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gtdjmflft.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gspaifwqj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkvkvxnrx.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gfqektqez.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gnbbggfop.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/ghkybabik.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ggdmyzttp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glhzbidxc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzdfqpnzy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/grzenpxdk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gaeuhroxs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gpkhaczar.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gjefazssj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gcmidxlcv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gixptnegl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gaenshkxj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gxbqqlmru.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gtbqhosqr.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/geersnquj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggxjnlosq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/giigthheb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gegfmpmjb.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gbasbnzzk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxavaaixt.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gjpazyikz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gximbefib.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gahzaqrpq.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gfjgqokum.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gxlqkeoyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gjtthhooh.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/ggxksuwug.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gzavodzzr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gouaaxnku.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gtetckhsj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gtjqvbnru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gilqdrglm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gbxizuwtt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gtexjmgkg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gusacjhky.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gdmrleckt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gwzgpduqg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/ghalkppzt.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/grspwmmdz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gcuyrvdnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gaswhauhg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gvavxmizv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gjejximiw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gqvsxwwlc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gxgaaerda.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gedjprezk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gybnolvqt.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gqwuigpol.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gizbzrbqm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/glcricooa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/grrvbaawk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gxchgztck.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gjcamdgsw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gketeayom.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gbqdvatok.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gckigmlyv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gmluncklq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gpuchxniy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/grvalbsnk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gialvkgfp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqmqlliyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gwvhobouq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gatlievxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gnngqjpat.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfzhlfpyr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/guouspmxk.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/ghypppwpv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gcvhmgtid.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/goqlkoqls.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdhczkxln.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/giwrsfxlz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gsnymrgyc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gyoluajws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gyhcizuwv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gkxseqlta.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gpqtsdovj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gxxddabmy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/guzxyekgb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/grmlasrjg.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gccgidctc.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/grhaftnua.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gswsqobdz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gpktbdumi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gjqmzouem.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gnkjrglng.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gguwvrtqs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnyuariqj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/godmxsbve.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gvinyeebb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gxqrdhphd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvvbdllkr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gtjpxhyhw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggjaoexww.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gucgzbdii.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gagfhucym.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gyliutmrb.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gygffzpvb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gylsjmday.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gzdmzlxze.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwgnzviqz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gtggpxuiy.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gvganqnkl.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gkviejilb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ghnnlsoem.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gcdsdkjcv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gyqepfyfp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gdcupxpui.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/goeslfomw.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gsriedrme.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gdnqpvrxs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gutqcdxst.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gikbfrfrj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjodhdwgp.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gkfnjpkau.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gacmxwxvg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gcpeqxhyc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gwpepbgmx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gutftqslq.sHtML


<!-- 参考信息 -->