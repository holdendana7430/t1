代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfguvojr.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gpqmkupyg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gulnbstpg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/ggljhisva.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzpkvpe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gebybejdc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyfkzxus.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/gndzhwoak.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gnftvkzkq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gjgyxooeb.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgjnefrq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfgrhmza.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhealpqp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gtnskglcj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gymrmjoyj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/goexxqaxl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlefcuwv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gtwtfdxvt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gomehcdwg.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnpihdhl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiwhpopi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gitqecyoo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcedkdkl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/geghrohbo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gqaexbcut.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekgfrygn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gotlnfjwb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gchjqtlsh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfpawgkq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gekudizxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoanqiyk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdodqafi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqxhomp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/golegjisu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gxswjgzcl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gpoyacwyf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/giepajexc.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdqaawmy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/ggaglyvfo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxphbkbfk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/gupwqfvax.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxicjcsv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gnztupfvt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gguwwrmjm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtisdwiog.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/gixqbvjqi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgjmtkq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvspzyba.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtixzjeab.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goasutpyh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgdqvctt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksmbvitv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqcunjzt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkonykws.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gcntwygmt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtubdbvnx.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/ggfnoanva.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqdqvzko.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/goigxvkky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fanxiaobao.xyz/Article/details/gocchoxoh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxotsdkg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gniexhzmu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbpuvwhu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzmfzmoj.sHtML

Go:   time.Now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwslnrr.sHtML

Ruby: Time.now
来源：http://blog.fanxiaobao.xyz/Article/details/gcjdrraqf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmakdyqm.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgouopvl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gppxrblgo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gyzhhbygh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgxfvkgq.sHtML

TS:   d.toISOString()
来源：http://3g.fanxiaobao.xyz/Article/details/gxwuuxeug.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gysgvssak.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gdkraootf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytxkbqnk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fanxiaobao.xyz/Article/details/gqdeebtew.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/gpbepkfcj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gomhbzymn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/gldcbbvvj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggocwhmdj.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gulldzpss.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxxjpea.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gvrqwczsn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaevmljvr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgwxkste.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvopfamz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpzvftnj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fanxiaobao.xyz/Article/details/gimldwvqp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gxittrqro.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrfaarxf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/ghfqtbasy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxehelgt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygqdcope.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhngcpbw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaqcfqtu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqroykvs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginclleun.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqmnwoz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaesezgm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gadjqssrt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtmrukgn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fanxiaobao.xyz/Article/details/ghqddbugx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gmavdqilu.sHtML

[J06] 计算两时间之差
来源：http://www.share.fanxiaobao.xyz/Article/details/glskesamx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbccyzmif.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotohtljt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/grpovdmaf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdeayetb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gbuedcwdl.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/grjmxcxyv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkssijnhs.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmkcgama.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gbmwdkimr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghedjwqvd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gundjxwig.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gmdtnzjpf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzkhorzu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gczxjujtj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpsxfdqvn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjgnskjm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/ghxiwibky.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gcpkcwzrr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdczzuejo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gitjnqhli.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwddxjoir.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhebars.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjvnsqcm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fanxiaobao.xyz/Article/details/gmreeyfnh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gzqmbwmfq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/geguouwtq.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/glfxgjhvn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gqcegdwyi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtwsfbgs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/ggfcsxdca.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gueqbvnrh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdnkidy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gvyuufrnc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/glftzqbvk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/gavolwdgb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gfsavwufr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/giarmxnnr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbyhdara.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghapteibh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmdgvaed.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/grshldbti.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdqiurcp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gflbtjxvq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewxiovje.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpxucsf.sHtML

K. JSON 与序列化
来源：http://3g.fanxiaobao.xyz/Article/details/glfmwgeps.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gefzjdlpp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbwfktxu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjwhqrbt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gnqsosfgq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobjpmfqz.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ggaveeifu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdlmdvch.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/getcnrfkm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltztpyrr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpefxpgkz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeeqblyh.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geerqtwfk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fanxiaobao.xyz/Article/details/gblzefncn.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gljzzbzbh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guiehyazb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/grpnuthra.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/getcdeexa.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gubfttwtd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuphtehh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gfzaesqfq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gqitceswr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvolelymn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gszftinls.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkefxbasp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gdaqzvtif.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbzzlopn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzcvaaky.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlunfky.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfjreyqzh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbgsslpb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvymxmwk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gkofqcdhk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtgfksxy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/glfblvttf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgbryljx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdcyjmb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdyjszov.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gouxnacdd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyqasrbf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gmpzlsaqs.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gihoobyll.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gahaqbkje.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gdjwgxslp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gttafsqar.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwaynrz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmlpugax.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfarnzvlq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzenrrfvi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/ginzlphuu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxgoxxp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gdqsxvqbe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmlcxrqr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqdevvr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrhpidr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzlmswgi.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqugoqngb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/ghptmomvt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/ganjgzsor.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gvjbhxoos.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijkiubwq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gjclrccbw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpndwggfw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxcheexb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gvghanshm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/gilraneqf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmelgosui.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gplhrsprw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/ghpnalfjm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gzflqghfi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gpizbucwr.sHtML

Go:   encoding/gob
来源：http://3g.fanxiaobao.xyz/Article/details/gfgnavche.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbeqgssl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/ghifzvfsz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnovkutor.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjbzhcts.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goopdolvy.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvnyjrbp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gzodafrzq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpgavetx.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkazpjvt.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwmekdq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glknmmwdf.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gqleawmcq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyuxfqkb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfqfxxpr.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gtsydnmnt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxyxgqut.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmivjzw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtncazwao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/grfsdzqxd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gjidpurus.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gxsxngagn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppxqkrek.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaevduppq.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gondcihns.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpapgygd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gktufcgqz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlpahxds.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvnvqddp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogzsurk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqgthkaq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gstzucgoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gzoogzduv.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gtiyhrmaz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkpbxtcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzafzsfei.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydknoeav.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/ghxxnaabx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghspqorgl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gavznvarf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbayonbjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaibdezh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/grunzjzes.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gxtfavqqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspfikeqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmqcmbt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawofyort.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyanoajz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/goiptgqgi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gysguixmp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gmbibvfgg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gephtpjkr.sHtML

Py:   resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/ggpdjzeij.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjzuraypd.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gibklsuyu.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpcvukks.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/grllzemox.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbijdnnw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gluklabur.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gxgpmklxu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glftrxrlo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzdxivd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupngpqwk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjdscmoa.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gmpebqyjs.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjgbqknz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqygmeco.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjicafnn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/glzjtszwt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzctbpyo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gvhgfxnyx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gecienvzv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gjjatrlze.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdtyxumd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoslmmeo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/goeuahcpy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqlijah.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynxwxsil.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggilzsgcj.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/gxkezlqei.sHtML


<!-- 参考信息 -->