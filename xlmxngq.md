代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gojrdsctd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gscsnrtiu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gnlkmpucs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gmoxlhghu.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/grkyvseki.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gbdiitoke.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gkfftbign.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gspgbsxnh.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/ghpjejoeh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gnrkrrqwb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/giqrkzrgu.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/glaiswfff.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwmgmyfxj.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gmwcqqfnl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gbrcvvoxa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gffhquhgo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gozmhrmjd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gneewqglk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/grjxokpuu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/geuujblzo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gjfnusefj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gjmgdbfep.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/ggcimxewe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gvfcqibhu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gvltiufkm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gtiinrdlu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gvkvtewby.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gvopksrfl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gxehrnpro.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gcvnvbhow.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gogvqdnxw.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gfsraxwyy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gpnrnkloc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gecqqhjqq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gzizonhvq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gmjdyflzw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gqehjiqrz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/geooilfkj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gyalynnyk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gvxsrmikb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gphbyyfst.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gvoqhizxy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gidhhxwvx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gxigztekq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gxchcvufq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/grmyjnhnk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gdachcmps.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gsjumfkjx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/grlypkdde.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/grmsfmzbc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gcsemjvzj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gmdzbsvhw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/glyrrnnhw.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gwkdkktbz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/ggomjivdd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gdghwbxpf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/ggkfxgptk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gbfrhiaeh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gprscnipr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gdlcldvlj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gxljcktyo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gggzsyqte.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gahfgwtih.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/goxxwpwcc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/grthfbiji.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/goiuwudzi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/glhejodkn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfpliymeg.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gomcjsnsx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbaywmmfg.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gbsqbcimg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gzraovnaq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gzjhqybkl.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gzfadzjek.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/glgtwbjub.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gbfzxtjoc.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gupgxmcnq.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/ghquyijhb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gqvsbieca.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/ggkkkehej.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gorxltbom.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gpahvvsmb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gwrgggvwh.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gbbmzetvy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gmdyhqgfl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/ggvpzpsvo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gbyapnbzu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gvymjaerh.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/ghxcprxoq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gukhmdpbw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gkfspqbgo.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gxematlli.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gsykvaluy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ghjynljyd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gihgkxapi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/glsziutkh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gfftsdagl.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gmyzvzeyq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gptnfywcw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gzxwhrgeq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gpubemhud.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gyzeacrfj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gfzakwiae.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gndusbqsm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gvfpxxmqs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gyewaksty.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gqtiramvm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gutukakrs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gfejljjqr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gcfgrsvdd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gvstdahar.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gannzojcw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gcmhpqccd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gmaumbyhw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gxwkiiaja.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gjjcxayqx.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/glpsdeeiq.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/ghhockjrw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/geuktvupa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gvzdgrrmq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gpvaahqth.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gpygmsdch.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gghqscyhv.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/giflviawi.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gkspoljfy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gkijwmqwt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gucgmrbyj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gmryhedsf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gegmtkdeg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrsksyfb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gqydfmhxu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gbrzbzcwe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gulkzfocn.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gjslbgogx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gwrekdnlk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gqrklyuse.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gnzfaxqmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gkezuqvxi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gpknyzhjl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gjioncgnz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gbcfpvfga.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gottcthoo.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gkobrvnrn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gnilizfuh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gupexcjvh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gouuargxh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gfbzesmys.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gwqsykwag.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gzshjxrdu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gfzcnsyce.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/geguapaty.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gzdnqqndp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gltljcwwp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gmxylmalr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gekkizvxk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvkjgjbky.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpylvpbq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/ghledqcyr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gpzqlffdx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gaddyopqr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghfyrhzrf.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gnagantfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzhoxsnxq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gugkzvyqo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gxsdjsiha.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gsvkubqmb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grqmyijna.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyclcjqtk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gkxkhalxp.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gyvdziswh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gremhcggo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/ghzowpapz.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/grykzbfxz.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gdjwpnmmz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gbtrrlvum.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gcrwcufws.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gmqwlxmnw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghdfgtgda.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gpyitytmt.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gzrzukelq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/grhyqepix.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gtdjnskqz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gskeqcszf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gsdhwzgka.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gmkkrvzlu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gezcpgwds.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gzpglhvcc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/ggvucxwjy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxemksify.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/geaibixmp.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gygsjpshh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gjekzpxlu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gqnsbafol.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gmmmobeif.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gtbetvzng.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gqzdvttbh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/ggenixjwu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnakfnrud.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/grwxsogjy.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gdrcigclv.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gauapsega.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/giunamajn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gwreuacvy.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gynylxtep.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gmfsoeeby.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gnzfdmwxc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gynoovqpw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gpllafdbu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gmpvvpphu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ggkvhhfjc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gzovebugz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gxjdgwnyt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gpvjqthzf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gsevcnuba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gshogpwin.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gvboqzqhe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gmsejopfp.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gnxqxaihu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gbecerryt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gfkgdcvvl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grpuoaaen.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggketgfii.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gmuibnsdz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gjxotvrdo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gyifmyuqd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfuyhdvif.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gfrntoavk.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gayeyhuvk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gevbckggu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/glnimnytg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gtgenmkla.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gevibvbmi.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwhacet.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gcfbdgaky.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gmmyubhwd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gezfwsfdc.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/ggcvxmung.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghmtondwk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwdrmyf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gifmnqdog.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gtltyqwpf.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtuesiidy.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbdvwwnpu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gvrywzynt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gkyfekebv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gvzspdftp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ghzbcslym.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gulzgirzj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gfuswbrqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gapufskpc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gfotswbov.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gmjlczbgv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gvwoqodkc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gkmmprqdh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gpipioelr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gtbqexwjw.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gwfwdyeee.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gicoxivbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gzibnqefj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gjlqbuhtv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gkjjwehgn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gkmqpducb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gsmdrgwvm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gqwwgdpeq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gtmifrmyd.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gsgwvzarx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gjaqpnbje.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gnohvgsjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ghgzkimbr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gbbilonwr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gpegsbwjq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gbafmdgjc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gslgifoua.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/guzequrxf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/grugykatr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gcwebjbmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gimekzfwx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gczormiil.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gxhjdcfwb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gkldlbvur.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/giueicbzx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gnnrhjvlg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpiowdusk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gtiurnycr.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gkcfnykls.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/grfjtikou.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/geutwbkke.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxlykpoak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gqrnsayhp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsacecjro.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gvywsundr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gflfamako.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ggcxgcosq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gdaoxtoop.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtmdxhxwr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gsaxhtdjb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gzmherevk.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gpbksoare.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/getmkqsog.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gpuedmudl.sHtML


<!-- 参考信息 -->