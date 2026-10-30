代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrcsyhlv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gwfyalbid.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfsdgdjc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fanxiaobao.xyz/Article/details/gapkzkqwe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqzsayca.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/gxrchimyn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtrvbzty.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpinhfbvi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmtncfrr.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqfhdmfi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/ggsexpobd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvfflkfw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/glvfcjnef.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fanxiaobao.xyz/Article/details/guqkgghde.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtevulray.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckwwwxg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwpqfeoi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcgpmaiy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gngsnqiwn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjnqafoa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/gykgnkmgr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gjqshpozi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gukjvwfqk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukroerib.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/guzuxluxn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpxszgvw.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesenjtkn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fanxiaobao.xyz/Article/details/guzsrzspk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gjbsmmaup.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmbryzcj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggixslcuw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gnogsoczn.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gttbpeipa.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/ghucgcreh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gktniugzb.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoupxqhc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gmspuamnc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gphjqqwjd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/geepdgbtq.sHtML

TS:   d.toISOString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytmdwrv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gztpesafq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlxkctem.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gjdzscbel.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fanxiaobao.xyz/Article/details/grtpfbqsk.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/guzshwcdw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fanxiaobao.xyz/Article/details/gzaahtvfx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geazcdphm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxantisw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gskafsehp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gvphmrrum.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/grwpshzvk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgdbahg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvmtkhev.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gqkqzbazg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzubdleh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/gugtasvng.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnltrpdpx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxshlzzh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjlqcwkc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyirvzayc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gomepxbxo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjezryol.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrtnxevc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnywkpnqr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fanxiaobao.xyz/Article/details/grbkohpjc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeiolija.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxjdlymy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadbjnide.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gikamnpme.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fanxiaobao.xyz/Article/details/geagowmya.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelmxyzyy.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gyotoiaei.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gkapmjxal.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/gbcvdhbuw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvqpxdgw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/gieqlgkon.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glshurmxe.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gzrvvkywd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkutvrkcy.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuxjsluk.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjkflhde.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvzypgv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganlfihig.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gwiekpkhb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylspipnh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbhfwtgv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucinpcua.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzelrkqk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbmkijjf.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gyayqsgwv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/ggilpmzlx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbutyblyf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiitisjy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/gmtzkvcft.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsygrbtoo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaqbukhd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlluvrcn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gekfvedxi.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gchwzdqee.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzloyrks.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvojsdqxf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvewfzsye.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvwsigm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvleuqif.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fanxiaobao.xyz/Article/details/gkfopsuaq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/glotfntqn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqrbwbvo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhgaflk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgwmcqqp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gbcatwfek.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyddqssrg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/grfphazbx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxbkyxrf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutgtpczp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdkbxqlp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gaensjime.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrgiaflb.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/goiajrjnf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubzypvx.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gempdooxo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gpudacyew.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxvonyko.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gqohfxwaq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimvgfxf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gbdxaeqar.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujuwwdwp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gralhrwvs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gackhlfys.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fanxiaobao.xyz/Article/details/gkiklisji.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnlcltwg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzuocejqp.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijzkqtit.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwrmkjmn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxnieku.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjvkhayq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/guirbhkuf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gheblhqhr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbgzrheu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszmkmijm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmatziuw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrpcdigt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgzezwkb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtujfbjay.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmeilltp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkfwznyr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgnkuyrw.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbqetxbg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzeqgtqq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwsqzbbg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfpyjkxz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gktqtiojs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gfrzooyav.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfibwiguk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgomqzbu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gxbojrsnp.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqabfatp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuzeagud.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fanxiaobao.xyz/Article/details/gzifqjcjp.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/girjvfwny.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/guccuqtsv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gailvnpon.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/gaaxzfcgx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/glybmfsph.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gzybdfdny.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutaokwv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckdnvlnm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/gievhosto.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhhqqzyl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtizkam.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshhzvxni.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/glynmibih.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gusfjmcyk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gskgmwhpn.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmiwpgec.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbozsqqs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gecljwqbg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/geaxpantz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprakldw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/glpwgxhki.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpgdjptz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpwupdx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/giqwkdxsr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/gbntuxtxo.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhlvwypg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgonoif.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjuqqnhx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gltmhlpnp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrhylze.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytbsqjkd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpdwqiew.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwznzxmu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxtwdszjo.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvrfquh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmcjpso.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/gslgwgjpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhscwjb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvllvvdp.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gudlzwjll.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gswedazcx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvvsxlic.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquchvpvx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/galbfwyfc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwzprpre.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glpnmffyp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gkchcgebo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fanxiaobao.xyz/Article/details/grghhdugq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gvprxwoku.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwtmddm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsojjgmol.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjqcvao.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvkjual.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gbjottbdl.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/gtlkmxdoj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/gzajhxxsb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gcckyljua.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gaggigvln.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfinsnrsu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdoosbfs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/glhajohtn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gbvtezmcj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoyicupp.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfqudqzn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiqlyixb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtkyaexg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gicyaqydg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyteabrte.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwnuwup.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/gloneuqrx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fanxiaobao.xyz/Article/details/giqamjqxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlsuzoh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkqwdxns.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkrbfpis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/guaeuphit.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcsldmbp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpuhpyxh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gosxqqyzw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhxmfll.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyptzieva.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gnmwbujma.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gcneqykrw.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gcruwpbxm.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkfsxya.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmnuhuut.sHtML

TS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifdisro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtmkmsrv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gyojmnxdt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisqftiap.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/glwhgcbxy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfrmqtjv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmsbnvxl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcfrslge.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcbutxtj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/geovizhdi.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitrvowqp.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gjuizjutw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvnxccqm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gwamkurfy.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gezhjxhhw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxtlutv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagdjrhh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeoratbf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ghwksqiqq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gyxlnehzf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvchjpux.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsniwiaty.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpxputfl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabzaozvs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqszbgfgt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gowmxzced.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzlaykvr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/glzlsemzk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gtawtzbff.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahhfdnx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvsuyrex.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/giekjzcaw.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gklrnuimh.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaiwflxh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaymhvlr.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmjclinhh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gtvbjnthv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlbmbipy.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpxddszc.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmiutzrf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzhsvwfz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/geegankfy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzbokcnp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/ggjtzxuua.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzxbhxlf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gnpavylrc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpruebxcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyxvtgc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gqirxxsgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gzahfbuvm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvvnwqvn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gqyzcxbzf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpxxemap.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gsvtaddah.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmoamwhs.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjixnnc.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gxiebpxmp.sHtML


<!-- 参考信息 -->