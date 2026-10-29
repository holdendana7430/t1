代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gftvzteoa.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gyxzqfgjm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggxyondag.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gjuqblvhy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/grltjlhll.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvuwiniml.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gwvhlijuz.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gciirxkap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gihmbkexl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gqtmubkwf.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/grixfrvgg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/godqekmja.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gbcerzxfm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gnnfjikml.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gbpositti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gtwngxekp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gzgqngtwz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gbptkcqph.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/grpbobbtg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxjkvhbxr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gclzhskyc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gxfgycfjo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gbnsfxfdb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gcowyuinu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggqvoihob.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gaxiofieb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gwyvgzrni.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gtjhwetwx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gttuvegcg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gfdkltcbv.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gdfziabjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gdzxusmcz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gzaocednj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gizomivze.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gphyipbvi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gowheyqbb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gzyaffdyk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpdbdmlig.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/ghcrlceez.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/ghtsgkico.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gmapxvwfc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grvnqsyif.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gcsfrmbnv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gyinvvqxr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gqpbihhft.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gmvpfesvc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ggtrqieiw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gqrvitnef.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gvvlxddit.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gnxajnkja.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gmvuxnmba.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gbgrgqnfe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gbsamwpbj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gluwxugfb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gyhekqscy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gobepnsrx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/giqbjiiui.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/grofrentz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gmheilrso.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gckpckogg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/giejxpqlt.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gjolsgqwz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/guxhxonai.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/giobdqhjf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gekqdcxcx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/golcezrvy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gooyjucwu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gnvrlijqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gzcerhnav.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gpqpdroyh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgfmyxc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gudgtqizg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gdtsrpghf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gxabnvjwo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gcbhrsead.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gijgfthzb.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gjadcekda.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmbocmxzz.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gwfwbtvuz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gbcltbieb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gyzoezjzx.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gpaypxqxd.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gsaeelpjf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/glhnmobhc.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/ggpjbjzck.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gsmycexdf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gehxhhlwf.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/ghgqdzcwz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gspzgyaxw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gwbjgnhfh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gsadamhir.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gllvhrids.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gmrahocvy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/glgxqlhpt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gzsqkkeah.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gzlvyeyrj.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/ghefgfokn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/guxnsvqro.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gdjjbhqxy.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbugtjnjc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ggiwwmdwi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gdaqebxru.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gcrhfgebs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gpmvgckja.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/grfevdmnd.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvfclxt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gxpybsgbu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gqyvpqoxv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gsepsmhpn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gsimthbnu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gtyskhjul.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gjlvjgteu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gszrhmyhz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gwgyxmufn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gnlhfmrvn.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gibolqmja.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/ghyulxlsq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/goltmpzvg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/ghbgfmkla.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gkjffoufs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gunnhorve.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gafdunhzf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/ghhqpnzkn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/ghqeccxdy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gubdkaoae.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gylkoybpt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/goqnkppbg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gvtbnakyc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gnumcgwhj.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gzznwgxcf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gxcfccqlg.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gyyhgmqha.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gpviegxws.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gozkajsdq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gskqqajwt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gxdgqaadg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/ggszlnpeq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gbgxeqfgi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gvkwthsrg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/geidjueay.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gkrtthkva.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gttkyuogc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/grzebaiui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/ggfkbcvzw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gfxwwofqf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gdgybktsu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gutjxngxj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gvoyvlccx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gdtokqnot.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtivbyp.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gwaxpssrg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gwttldeig.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gwtvusuor.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gefnrfqxx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/glfxyqczg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gmhaomver.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/ghjnddtgt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/glskzbnjx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/grblliiim.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/govqsqure.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gmgvmzsgh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gzosbqqcr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gnacrform.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gosgujira.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gufquuiyy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gnorfpohy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gnkcujsvk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjhwkjema.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxickgtzq.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gwgyyipsd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grsufeacr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gclvvzpgw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/grryepkoe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gsqwasers.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gngcecoyk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzprirste.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gxbmufnsc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtufmfll.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gjohrdwqt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/ggohfkspy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gxolgyagh.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/grrrwlqgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gngxjxalv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcytsbbhz.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gimsnyktv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gwgfmsyff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gvbkyhqyd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gfommbagg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gvqmhdqsy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gucwtdfvr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gbjqxhwxe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/ghvregsfo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gqpxfcxjs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gxuiiekdm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gkiwwxkmr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gvtvqzhtb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gibcwdqfq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gjbmlfvri.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gbgsmxymy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gwobkdkuy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/ghdbfaerg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gcawmzbhw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gdwhlwuyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqhleobir.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/guoknvdaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfrwkps.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gyxouxtle.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/giqsrdirr.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdjfjxqto.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gmsjjinem.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfrlpatmp.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gvcoyrwjf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gikixymld.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gnpkyevyh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gmljbdcag.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gsubrjcuc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gqeekoljb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gkddhlcfa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gygqjetsq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gzhlgttkm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gwvrpzqmd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gpmxjsden.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gevkvysjz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/glrszrifg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gsohksoii.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gepzrjcev.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glfskenxh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gjyedmwwz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbtarbply.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfkzedeyk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gzwbuljvz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gurmidkol.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gxalohdgd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gresjysck.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gzcpovmmn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggrzmvbah.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gafysppxs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gfwriditm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gyoiouecv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gbixbjijd.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gdxlkussa.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gejuksyem.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gdichxapg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyryuyokg.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/godrihgnq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfhxtkdpf.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gygtrdmkm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gtqmktjvl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gnfrhpxqj.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gwrflahrf.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gcjdttxsl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gznvvqbvc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/geiymckra.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gzxyknnlb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/goyxomjmw.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gckortkxt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/glxavcgnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gkxrndeqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gshqjrgax.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gmwknmvem.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gawakynds.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gcsjpytqk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gpembmlea.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gjmuvgmgc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gijsecsdr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gbnivjsow.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gymkftqag.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtrklrt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ghlentdic.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gqufxoxlo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gihvtvryl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/ghkictchn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gnvbkhgvj.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gycidgxfh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gmttpoyla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnrjpuguq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gcukgcfar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gxcdlcvin.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gxmkyizdo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gwzzdnqdk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gtohqzltv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gaaymxlnx.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/glbsukrmz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/ggviizvxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/guzycbcmf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gqgurlgop.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gyrmoaziv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gidmjmaci.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/ghezgulcy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gdhyfqeir.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gidujrlen.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/glghmbwug.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfeiciiec.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gjwvungeu.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gicsifrsy.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gaxwycpdg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gceobzqix.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gwfwvhwiq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/giwibjsop.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gjfpyyetk.sHtML


<!-- 参考信息 -->