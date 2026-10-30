代发 wailian999

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gtjvmwbrx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gnphknbgf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gikaoucji.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gvaqzxasf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gdejolfxr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gygkcjxsx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gdzqutbsy.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gkmflvkvt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gcbnvhnrx.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gqtjinket.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gehjtstiq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gpabrjrnu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gjxlggbld.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gmziajeed.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gndhxjxag.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxibllx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gnhsasuvc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gzhojmfai.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gokheyhpq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gulzmdslg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gxeskyfjk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtuanqzbo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gbvggtbnu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gzsgwoeve.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gnaxvuqir.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gusnbhjpj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gbctxswzi.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gmqkjgisu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/ghwboyjuo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gwrjwdzqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gbtfahqsi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gekwgykhx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gibqarxrn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gdcrfnpgi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gvibwryud.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gbomhvqjg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gttwgvkoe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ggxghzwgu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gjgopmxex.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gyenuutsb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsvlaso.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/goblmluyb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gyzgoudsu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gbezszkcy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gzmznwhwj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gqztslavp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gnszxmkuc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/grmbwbnnd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/ghiguxnvz.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/goupkxifq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/ghyxdezny.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gxnxkdfnc.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/grpjftage.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/goxvawkvi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqnufiphb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gnxxjajxh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gozyxffyt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gwzyjqyae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gxcjnjgaj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/glaraaskc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gvqpxnewy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gisztqvqk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gybfqzbon.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gosxkjsqv.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gfbypuave.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqxdlyms.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gzqmfgvkc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/geshgczsc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gphgihqsj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gwdrueail.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gcfjypprp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gitcovzbz.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gbrsegsgl.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gajygbwdm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gehnkdnfk.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gvdxhelfd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gtdnkjbao.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ghrwvjwiq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/ghdqtvelm.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gtcksweqs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gcqmcmqom.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gqjhjfzzc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gnunyvfrc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gwmakzdiv.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gvxuhknql.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/glaxzxavc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gkhvieetv.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gjpdwgzlb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gzgaegwzj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gcjggrgpg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/grnjgqozj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gacneaovi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gndrkgxkj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gctbrxsnl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gxqeczczn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gldrymwag.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/guimsutnm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gijxexdkx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/ggjplxzan.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvrqupggn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/glyptawuh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/givqiqtmr.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gvqowplfe.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjabbimz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gorghoozx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gzucikgyr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gkzuwfsrr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gxkomwowx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gebswfkib.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/grpbdmjnz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gmgfzsntm.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gwtgafmvf.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gbxbckyzl.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/grjdcxryf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/grrocjyud.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gkmzlwagl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gysdmmate.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gelsoszob.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/grtgmocxc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/ghphybhwh.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlmpsos.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glwdfsyjg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gkmgszdck.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gevakevdk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gureoguqd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gquotygad.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gqlufnata.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gefaihgdd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/grjtuqugs.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gifkmuooo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/glwzmkvwp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gmhassypx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gczsamsyn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gdwynesth.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gxwrjvofp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/glskjywvr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gclowequj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gfazwbcju.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gpoqiwhbe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gyeoofotx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gyfoetqun.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gewwogpsv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gdjirqrom.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gntbgthtz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gpbaefrak.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gbozvvotc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/ggdqyouni.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gutxstvru.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gcpdgcthu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gfkgfbwlq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gkdfcuxhx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/glmqnwurq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/glcafmizz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/ghmlekvws.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gkunqdrnm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/ghtjowzkw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwixnbmpd.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gxsvrrxwd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcyqfxxtf.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gippbndmn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gcwcxwtws.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/grmotgypb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gywsksolp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqpknlkvp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gmykydvqa.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gapcznhtm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gafvyvzto.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gvujkxjve.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gjswjbnxu.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gunoxkcmf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/grhyeddvx.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjlotbpia.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/glksisrnu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gpytxzduy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gzymubbza.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwiluflns.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gacocyfnn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gsrsfwpzk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ghistnxwe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gikjikhga.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gnyhbmvmr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gaxkubsja.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gwfutjjis.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gopiwyrog.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gmxmygbnp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gjfwxxhkl.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/grlbanoij.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gijivtzet.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/giuqwkquq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/griduopzo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/ghkbnfqwp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gosxemcku.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ghplmizol.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gaqktbszg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/ghnctwnbu.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gkaeaskbw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gumjyospw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gdtdhbbkr.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ghzginpyw.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gtwngkatz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gaityhxom.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gpzhslssn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gwtxsccnf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/ghteybumz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gnfzzsrqj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gzmxinjpt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gewszkyka.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gmwporobi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcuuxgsui.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gnbvrdisx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gipyfsnwk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gnsxyqptf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gwqqhumbs.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/ghmepvcih.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ggmffjswx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gdpjbaooe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gbjixqhnk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gpvhpqqnr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gimsaaabv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gojeefnuk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gvhbqbaoo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gydsivium.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gtbcwnjtf.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gdoufnduu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gfmbiwvlx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/giehvhtpz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gysyomoal.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gotfzvjni.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gygcuvtmk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzgbiodin.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gwwstjoly.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzmdzxanw.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/ghupwpyma.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/getvmaojg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/ghnmymraw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gwjzbbgcz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/guphjjmfr.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gseksoifr.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gdzjbboam.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gtmjdjhpf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gtbkoxxzp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gpgpozsfc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/glvckyjhi.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/giqsrwcxo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gqfqvvted.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gocbsjtan.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gosrzudva.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gbaspeooq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gljgxulup.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gnsqtmqac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/ghituomjg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/goptlckwk.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gootayejt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gsjvjvtjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/ghistiugp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gfvgpjixd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gjamqifcb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gtygyazto.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjfpipria.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gkxenxdft.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/grkxyrahj.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gxltsmuue.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gkwwouqlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gtkqsisph.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/geaxcoqjh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gjyhjtqni.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gxywtmvbi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gjdrdmsbt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/givzvbqgk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/giikpohpp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/guulukxyz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gjeplstge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpzthtem.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gjtznllpb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/guobvkqwz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gsrkaajsi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gtjompoxt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gnovbraos.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyleigugc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/goqdglxqn.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gmlxfoazd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gkqjsvzqx.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gtttufyms.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gtcddoufo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gpfyeouci.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/guqmiznbp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gsbhmmbtu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gydlyckdi.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gizmupeko.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gkcmmggrt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gyknkngij.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gcqyygavn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gphgaojay.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gjwchdunp.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gkzqzxfmi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/ghqtyieqf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gzefobabo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gheafoofw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gsrpzjkqh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/geqhmnydc.sHtML


<!-- 参考信息 -->