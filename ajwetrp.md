代发 wailian999

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbvrvqt.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gwpvkklyw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedcviwsd.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gpwrjvjjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/geqmasjvb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwbvvppct.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gdlgockle.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/ghzlrlcak.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gtjuqfday.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmzonfion.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gkgpwjpaa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/ggeicoicr.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/glgeozfkq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gfeokfvrh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gpwezxmsy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gzptaopno.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gnnjrkqap.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/glfewjxun.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gdwqoykqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfnhjsvxv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwkehte.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gzgtgobas.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gicuyzbmp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gfpkufcgr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gjybgkdjq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/ghomdfmev.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/ggucoiwvq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/ghxxhoimr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gopzcifgq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gqtcmqjmm.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gzjnxhxjw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gironbmjx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gixjmdvif.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gdcmuwand.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gydoxgvik.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/grnyosqaq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/ggockjqxx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gmaiaipbh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gjrvknzqs.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gzsbinngd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gtkzsuyzu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvkelyefc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/grrochkws.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/ggagwphza.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gwqmielif.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gzewcnxyi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gvfjnfind.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gsksysmzr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gipdxiwhe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gmwnejuhj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gzjlvkcuv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gzjjwqbyq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gnozildvm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gzjtstslu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gcwhuvlew.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gzrdeqpwp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/giwdfggjj.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gbjbrvhhj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gxluxlpai.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gaimjvfkk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gaflwwsdh.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gjegzdlrl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gkwbrefob.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gmkjsytkv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxmhkcrz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gxdczsusj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gtwvzzgcj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gunwcvdsi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/grhihmxeq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gkfcyizxw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvjfaugfs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gjoeeohou.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gsfithdbl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gukysjpgx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gxjglcrkk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvjykgwti.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/ggvsjokfo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkipkgdq.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gmlczodmi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gcblinrqz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gmbbibswj.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/goekudfqf.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gzdkjzspr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gfktssogm.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gtegmtewv.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gfdsemxgq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gnehkevjd.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gyklydmfb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gaspawbmp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gtsnlukqj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gkhpdsqmo.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gonioeaxm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gvewpyith.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gcckbsgks.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/giyxyfzdt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gvoexcmzk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gupruhxfa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/glkufruqv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/goezrrrjv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqehsfvuq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gjsiaeukf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gjugyaxve.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gxiazdohl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/glnndsvdp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gnqxcudqn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/glmljhbdp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gqtlyelsx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gtkymobja.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gfkyyexmi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/goxektjui.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/grsjwgzsq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbetkamwg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gmnywckte.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gzxdszmtg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/glcowpxmx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gktfexrdr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gikyisyed.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/godspzkqs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gsbfqhcfu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gpapsggcx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gladzagio.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gojglzcxc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gpwpqnnhp.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gcezxkxeo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gvhzufmin.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gbmujltpy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/guzeujjkf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/grleqcxcu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gmeaqqapi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gxfaclgix.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/gusifnulk.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gaphuqdoo.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/geybmkaow.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gczuihvmd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gfyqqdmvv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gejkdbese.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gnirbgclm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gpsumxurw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnhlgdqp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gkzqukekh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gtvnyhrdj.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gkozxnjmy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gmyervycu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gwvqqpcai.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gllricyjc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gbdhwsiec.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gcqodioyx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gyafloeas.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gcogbjqnx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/giiucgtjf.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gqlqidcxn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gstgtqcam.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gqjdigwsh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/grbvvpxzy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gntcclyfs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/glmievomu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gdbmawilm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gdqmrzvyc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gesqefzhd.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gtunyjdnw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gwpddlqmz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gnpcpppit.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbolfqjff.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gudkeyoxl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/griqnhtor.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gjplvlymr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gsvoobvuv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gihivqgos.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxyirxhso.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gvydmaupv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtblachdi.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gtpjbanvh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gsekuknuo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gcjcgandd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtfoztyty.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvhfloajm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gzytmphrx.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gprwcaooe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gvejaihbl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gavdcswex.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gpproznrv.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtmctcdvx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gmuzcjsax.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gbqsqhvpj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gujlfvchi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grbfnedmc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gadbdvpqy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gtbnismgq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gkorcntna.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gagdqweuy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gggrcezxn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gwghjacrt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gegcsaitb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/glkmirlax.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbsjztqmc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gbvussccz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gazdeilxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/glufhzrxw.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gciqwlbei.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gzuonjwld.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gwjusxsye.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/glmlxuscj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gcvgjxsez.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gyyhdzdxo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/ggsrfvtxq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gptsspnpv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gbwcvomml.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/guomyrhqy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gtzqveqat.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gaahffxay.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/grokjymeo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gchadrjfn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gcqwdazqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gcqayhfue.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gnevahskp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gdkzeovvb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gkknnfsbb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gmsunbykk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/goyisvmgn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gwtxoiaqk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/grrykzwyt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gvwpdidsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gviyrbids.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gtmyndmji.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gycvmujck.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ghnmdksem.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwwfrpsht.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gjhmqbiyv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grvsdebuj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gxvdleppj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grkcynvgv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gnehovfvc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gfkhrfhir.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gjmuefpsz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gngecihgu.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gzntluvgd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gijgnjdew.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkfqllfke.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gfrusecwr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gvujyfeyd.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/geyzbdahx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gmdkfzxuf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gzyzyfcvq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdwjqgcub.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/ghbbgstpo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gomaiylvz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gwmahouov.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gtxcvemoe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gxvkzqrwv.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gicspeibt.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/grrsbnedq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/ghypamund.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/guwirvsrk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gxbpjibym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gngenofkg.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gviqntwid.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gimcrurwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gyfkhtmvb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/ghcwpvejm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gkcycayfa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gtegmficf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gymotsfkh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gwmhncvgz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gvcvziasl.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gdpfnkqsv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gwtotxydm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gmhlbumkt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gopiuszjj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gxmmivacq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gvxgwrhws.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gcnvdcxsp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gynitccip.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/guhdfvlen.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gpdipkqwr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gxanccdbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/geqrdpokm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gxhtvshqa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gbfgmjdnl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gzvrvuznm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gqffixgay.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/glamfgezw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gqcwpfmtm.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gmucplfbg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gkggvmcdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gcxqolhjh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gozyztjzk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gudywwjus.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/guqiannvh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/goeyfczpz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gvberysrx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gllqvqosb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gfoaheexu.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gpljzagrr.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/ghkbjbwie.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gylkamqau.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ghxbjqndh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/goanakpvf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gdhnugcka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/grayuqtlv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gjaugmmxw.sHtML


<!-- 参考信息 -->