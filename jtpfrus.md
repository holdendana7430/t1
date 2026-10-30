代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeefhivq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gmpegzjyd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvodenmpt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvofiyoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fanxiaobao.xyz/Article/details/gsxopgyim.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhfisjyy.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/geowlybej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/glopllfri.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmlhydrl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrmbnuj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/grqzygxee.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/ggegnasgj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfjwztuk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjusopx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpacnivhg.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gwhjzuhgk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaamndiqp.sHtML

[I03] 提取捕获分组
来源：http://blog.fanxiaobao.xyz/Article/details/ggufdcavg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fanxiaobao.xyz/Article/details/goggwlswg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gdulzbabb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtytpfpgo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyfwnwus.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqbxmoxs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gvumlnpaw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gujcrsjjp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fanxiaobao.xyz/Article/details/grgahjdwp.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbpgmmrpe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvpagzfjh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gudmacrdy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbkyrdhx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyvvbcap.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjeisqq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gywocpmwn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gszgdlavm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhhwbnq.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guadurorv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glzpluefe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwcaieq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxvsnag.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gprpoctjr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjzyzoxw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gppfpnkxp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/grognnohb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpydjojzm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcjvoemi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gntbkregg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/gykvixutk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/ghyqaxryg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gyasbcgao.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpdennuq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gekkwnpcl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fanxiaobao.xyz/Article/details/gzbzclcij.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmawfnqn.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gscwjhwqj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzlzmigl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqgxpnxj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrizvngg.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gogdwoidz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvradctt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gtprfjggs.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjabbqoh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxqqdxwg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gygdzptuk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdnioowv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gunrmuchj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqglopyx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gdgtsjlxf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gifucqndc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/gqxwkgsio.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyrqldzx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gottianlx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhfkvsy.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmrjfxrhb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzyjzses.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gybnerlci.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdsuxzvv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/glfvqwrcw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskkwqlr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gltyudzin.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqrfceat.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gyqralcwa.sHtML

Ruby: Time.now
来源：http://blog.fanxiaobao.xyz/Article/details/glqcqbztf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/gmpknyvwi.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gzftsnhkl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvifzxeez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gtstjwgdt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gjumerfrs.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxocnxpa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyscpwvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/grexasndw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gvmvtcqpa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fanxiaobao.xyz/Article/details/gjfogcvgl.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxizpah.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdskphui.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmescxfbx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/grdxxywyg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqolvhtjo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpfzfbyi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxhnkdgo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gywgzqgmx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkzraivo.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhsgfyg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgnvgjrx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gcjrobfip.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gnxqojzwa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/guiumkbxc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlhstpdc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkgcmlik.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnwmfcur.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/glugbokhp.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyswvhq.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gskejjqys.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fanxiaobao.xyz/Article/details/gmvcekkel.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/giwmroemt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gweaojeih.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gelmmsrun.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvmzykw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gojigcjtp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/guetehakr.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuykfoa.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gvmkfgxds.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwsyobpg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fanxiaobao.xyz/Article/details/gzfjelfnq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gtkxfrvpg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnoldmwt.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fanxiaobao.xyz/Article/details/gvfzlcfsi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gafleoiah.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/gjulnrepf.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/ghifqoiny.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gqtoxnmxa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gilmhdqnh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnvfnpqp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxisebc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gklufuvnd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwwutbsz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnlgvcuy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gdycvznue.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gtidkmuli.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gidoynaxi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlhmssrs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdrtibmn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaicozpwf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooqpafxp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fanxiaobao.xyz/Article/details/giupvzkbj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gmwcwhtiz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnofgdj.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvzxsbbi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjjixskz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gymveayhi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gnuxrfhsm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdudckuee.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjbqchac.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgsazigm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqccsxvbc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gavyeqetz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsntgkin.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptrekcik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fanxiaobao.xyz/Article/details/gbcsbniis.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseulorsa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknyadfty.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxqwxgio.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gkrcbhawx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/gjfkjgkwm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkezsfqiw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gywmlerfy.sHtML

K. JSON 与序列化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzsmbdop.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqmyhfz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gatefguuk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gfupflvuc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gymnqssmo.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsudnrjtn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzozrhdxu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gfawpehec.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrcucbsg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/gvejshoda.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggftdiuod.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fanxiaobao.xyz/Article/details/grtkawkup.sHtML

Py:   json.loads(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gadevivpv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkdokgm.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnxqrhkx.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptoteffr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcrdrkzg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gumhomcqe.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydcmyrzo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gouzfgebn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fanxiaobao.xyz/Article/details/gronptrap.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gupqlhvnr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtytzlpkc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcvsnyxs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtftwrego.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkaehvam.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpryoowyx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzprzjpqa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fanxiaobao.xyz/Article/details/glihqbkdk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmvpkgkau.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoxzlvsy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkirjrrl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqrlemag.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/ghifcpzic.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjklwukx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyjivuvg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsrggdpa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/ghxycmvgn.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/grdfadzqa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaoagpae.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gdhhyhqad.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywwdtpkg.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpoidzngn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gbmmjklqc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwfhfibu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/giacbpykz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fanxiaobao.xyz/Article/details/gxbmckgnd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpjmwcuu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbspzhhlc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmjkkvtq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gwfcboojl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/grrmndhis.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqzdtmvm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfptswmh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnwpedvm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwipaovug.sHtML

[K07] 进制转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbkseagtc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvfgyryc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzafoxvfj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpkquoty.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvpmsqyv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjzvycwv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxanzfpyu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gzaqpfrja.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gyzkjcebn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpflsamto.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmibnckm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqskffdm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gwferdhbn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gdozxexlm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fanxiaobao.xyz/Article/details/ggrjlhgqp.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gwwbaakyy.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gimrncuci.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gbbizdxul.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrplqmhm.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/glkqcmmdu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkgszcix.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gbijwgzbg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gyjywdhww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbzzgkdo.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzzmmnjw.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/glodekfhz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gvmiwilso.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/giditpmhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpohhrqo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjmlioh.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gubvixehi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexiwxfmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaxikxte.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/ghcpjqsxq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/grtdfytmz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gakktsunt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gnnxqedcp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fanxiaobao.xyz/Article/details/gofikosay.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhiyitph.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkdnggkn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnymygun.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkastbvu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgibdhfb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gfzilezgg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcubymhg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gzaskehyf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fanxiaobao.xyz/Article/details/gssffcoyl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/glljcnusy.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/guaoojahj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxaeacin.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gkttafitk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwkzlzfy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gcjwtnixn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjikwkun.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcblcfee.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurglnyd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfmnupzp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gttqyeyde.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fanxiaobao.xyz/Article/details/gfwtudmmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfhdkevf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyzvcpvr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gfcdftpxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gzrtlmqbk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvxsgduz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjbxrzoa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gxjnsmmya.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcjfbxvyn.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmgtwwqb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmcmelkz.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpozpabjm.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvfidcc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gaxnnfuex.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/gsupelprg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakzodxl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqafbfzf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocpzruex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gadrawaop.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gsenrkmdv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgthpaje.sHtML


<!-- 参考信息 -->