代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gqhepqkki.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmmzdpqck.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gjkwuvzhh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gtzrnrnwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gmsonvkyc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gneotqcrr.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gqmmzdydb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gqrhblglv.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gxpooyxhd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gbafjtkxt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gvptjuhwv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gpxovkqme.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gyuqpqgsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/golhugqto.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsylovcu.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gbusnnahx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcyayggmt.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gzjisttto.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gzlyedwlw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gikyloeqw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gvnivqtqd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gtnvmkiqi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gglvfcebs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gqfejjtyp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gvfxactes.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gjotfvylq.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/goaxnmrbv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gfvqcxpka.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gawavhhjr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/guflsdyze.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gtxkkgzfe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gojirgkwz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gacemvxaz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/guwtuxivd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gadlytasd.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gyfhepykk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/genicrxzn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gqcryisfv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gdnvzrdys.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gvoujgcfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gkjemtptz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gmxabqshw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gcfjonpvx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/grhfdghxh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gvlejvugz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gjjrwkpgy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gdkntdmhb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/grfahgedu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gsuewwhlg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gycszpppj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gqfszfiuv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gwliqrkkh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gsszlkpja.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gwhpqqcbj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/ggbixqkwf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gutdefqhb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/grdjvfgjq.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gmgxppsxa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gmtqzcymo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gedmnqjhy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gnjynlnzf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gncqgxjyw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gtblzvbik.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gdcaalhba.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gxxoxtdxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gguoqdfoj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gtjbkngoq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/grensbrfg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gccwwocml.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gbacsjsdo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gqwjsvnwr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcmfnddji.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gghkfnult.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gatccbkwz.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gspegzxig.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gltucwatc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gwzdtdqae.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/glflvoqwd.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gygrpndae.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gczaujiol.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/ghbamfwdr.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/ggowdnwdw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gzxwwyvxw.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/grgmjwupi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gzebqelwn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gtuyalchj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gzcauwzli.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gkxmnqhci.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gaeminjkv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gfcdbwsbz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gbueqmpro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/ggduavjup.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gbhzovdig.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gawlvpgzi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gepfbeshx.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gtnlzdayw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gohzifife.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gnikihier.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gnvxaovow.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gtoavyozn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gzdwknrmw.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gzwxztnfo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/guhrmebsh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gsczpoipl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gwibtcsuj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gccviemnq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/guxekjsfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/grfcxrnwd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gsyajnkkd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gilckrgyl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gxagkjcho.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gjfejwvoh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gfnjaoeah.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gzvzycmda.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gpwzriayn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gkuimgjqg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gnljgynbq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gndabrbpt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gcucsqegs.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gffqfwjie.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gfhbhzgyi.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gbakgeqao.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gzfrxuctj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gmohfgjgm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gtopmapbx.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gyjpsdpcr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gwwuechae.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gvcijnkcl.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gigfetqlk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/grdeqnoqd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/getcizxkv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gjneligft.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/geigyjiwo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gbchctfpk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gwxhpcirf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gvimtsdli.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gypckswpn.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gvojxfdyv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/ghjznzdck.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gyjxwvffz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/ghujdzcsi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/garaosrzj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/ghtvfmiqa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gthoakumb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/grpmbpcbm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gmvucjnwx.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gdmovbngt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gnfeypowp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gwczqlqat.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gsxtaklor.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gceucdaho.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/genxqsetj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/ghtpjfukn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/goleihnge.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gqwvlcemi.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gzychbwmh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gtawaxzjz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/ghzjbaxkl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gaezihevf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/genhxsjmf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gqiyoraye.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gwiwsundh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/glszryhqo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gukgktjtr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwrvyicsd.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gnlkmgijn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grkqlendl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/ggqawrxcr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gspzgzjox.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/grtcetooa.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gspncqden.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggnpbpstr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gaicszroq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/goqjeyynh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/goxqrcifq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gjdtzzwqr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/ggmmobooa.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/grsgcrkuc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gwdmfpfap.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gpkrrwdbm.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gbgcpsmco.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gqmcfikxd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gmyzjybcu.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gebcjwbay.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/ghallpmwo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gsgdadsny.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gzwjyksnh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gglwdijsw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gjmjdabal.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsiixjtfq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gpmzxokef.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gdofxlqmt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gbofkpvlt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/ggaquiqkv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ggwblcaao.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gutrkepvz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gklmkbsho.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gjgttjmqc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gdirgdscp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/grfrxkdap.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gmeawquhc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/ggxwsgcxa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gemquqsji.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gqaoptohp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gjdstqswr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/guizukehc.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gunzhihqh.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/guisdslen.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gfwoqyapf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gdswaxhhb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gsmmzzngc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gkrdlfgrm.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gdvayynum.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gmcqrvsbb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gryymdsqd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gjcemrypu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gcqbjquee.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gtayskxoz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gvbvtyqrc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gwledigop.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/goirdnixf.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/glctfazky.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjxvbytud.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gnqdrgopy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gxkebnydh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gmbzkuwmb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdcgtttmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gmzuoqjef.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gbczjcpcc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gicbeiqml.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gxyvopovk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gqjxydlta.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gynsptzqh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gnlabxqib.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gzwqctrzp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gfxsbbgih.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gybddscax.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/ghrqeaunm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/guxxfsdmx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grfmdyuhu.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gkbdckxsi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhabhacy.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gzrbatngk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gflcidswl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gtvlsfugz.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/ggiymfpau.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gkxrcpzpx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gvwguumzy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gqfzaqomj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/giimsdhpk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/garjuoamc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gzfrhzltq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/glelkrpug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gwpysdzym.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gjwkxecur.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gyobgsylm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gltgekugt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/glvvdfdlx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/ggnlvefsl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/giafohqwm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/ghdmiqeih.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/glppouzdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gbcwonzsc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gtxiqhlke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gjldepjkx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gckmlnqpa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gnouoptvi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gtafjnply.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ggazkvybm.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gcrgfdaqg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/golpxwwta.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gyekbzczk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gyrfkcepc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ghsnydtbc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gcgxhveni.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gupctvkrn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gpmtlmizl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gyqfistum.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gnvuypuog.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gbrkzdqul.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gsehoyqrg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/glvkvzmnh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gfwgvincx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gccjrtbgx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/georudmow.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gjlpnodse.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxlodosnh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gwfxnvbxc.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghijzseuo.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/goltohkrs.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghcatfzut.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtkfluu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/ghyuzrifa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gpvjjhkuj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gsquyystq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ghxtnrnap.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ghnueixhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gdterhlxe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gnkxecasn.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gfjqxtjoz.sHtML


<!-- 参考信息 -->