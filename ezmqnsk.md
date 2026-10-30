代发 wailian999

[I02] 提取所有匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gepbhcmvh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrueevvx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gznlzgmqg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/guhnltave.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gqhuiqmvb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/giodiyjxt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqutugiku.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvujkpwfg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gupkzhiqh.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhtqmetw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkitiwuvl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gyurkwpur.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gnhvvufhw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhyibvlc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkjjwlov.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxclufat.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/grlbxmalr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gwabfxsto.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfelyhiej.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfsswwg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbpzbytn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gimrlxflr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpmyygie.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggswgbjgy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/govsqkbej.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlehsqqy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnpivxjk.sHtML

[I05] 按正则拆分
来源：http://wap.fanxiaobao.xyz/Article/details/ggyumwkbl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtbbzkqz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/glipfezkq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljzsyqkj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glffkqfeh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gslnzfaof.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyucbxpfh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcfcxtii.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/ghkiccjdj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gozafnchn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqppvma.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/geumvggvs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gtucjcgtv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmehpeipi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/ghczjcnkv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyfzhmzq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyenaueh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfududkc.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/giznjgzmg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gleuztkov.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gquzdtfyq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/givangjho.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gfcjhayoh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaouyxueo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gqsqjzmco.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gtslseztt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiswixto.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gezbtacyt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fanxiaobao.xyz/Article/details/ganpybubw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxhokdy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxejueoo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gynfcoyrd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gwksonxfe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gnsarjcwx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnqorlrl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwaygpse.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ginpzcweb.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/geepjalzg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcduzkdcg.sHtML

[J01] 获取当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gsifjqzho.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujtgcbie.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeczxolc.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/geimqcowk.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gjysdqcwd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmoqxord.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gimlludei.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwsmkhp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/gygsahuqd.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbhyxfee.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdpupmrv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbnjynhq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/grdhdyldq.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/ghslxvfyg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjatbkfg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fanxiaobao.xyz/Article/details/gixpipagn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gxrbwvsfn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjdbhclj.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxhbsivc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geckkdybj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/gclktyrra.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfncngdeq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/ghdgvybsm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkajawqn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpjyfjxf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqotigv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgasxuaz.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnkuqgl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazudvsvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdkqloa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhheiru.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqllwxsoc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycpoykxa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gypxvjzhc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhvwgvi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhcqhooh.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fanxiaobao.xyz/Article/details/gyudvnpry.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gemdpmypn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gnaswjhwd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjhcmrgu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmpdltij.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gkufstevj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunilauki.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngnqhqsv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdpfupou.sHtML

[J06] 计算两时间之差
来源：http://wap.fanxiaobao.xyz/Article/details/girupjzej.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzdgcccj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjlkfeaj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcerckpd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gsobetzqq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfezfef.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpywjwbm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfvjdxw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gevasvdwt.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnrovad.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gmohqvgxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gijsyckyc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzerybgc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvujoxta.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkcvvqhx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdqxfxo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/giymnlvuo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gghpbhuyt.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvbjkxhr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosllmyrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gajaetchj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fanxiaobao.xyz/Article/details/gvyrmqmqi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/ggvxtqalt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fanxiaobao.xyz/Article/details/gvgwbbzvg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllmylomr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/geffuldax.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gwvnbcgbv.sHtML

[J09] 时区处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilguicf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/gxynzhtrn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/granunrsz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhortuxk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gioetbcno.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghosrbqwp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsfrxkii.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gullgnnxx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqwyfqo.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gloqovpqt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grvulrpwa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/grbpsprcx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/geqajovzb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/grayjksov.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqhogcs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljmmpnl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/gixovozvu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjppoidfz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdnetpxca.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkadmfar.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grewwsuqb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrikzar.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdppsoge.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhaqqbcw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtejmvjtz.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohrmnjnn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/giityomcg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjzotnlh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsmmvkpm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxftfety.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gnzcfwquh.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmyordqe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/grjxzktkw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitewzhtx.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gucencnpu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcowcykow.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrlgmec.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfppbmysi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgtqhcu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojuhnxmk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gmqyzajtl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhfffbs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjytqubi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gckbikoxy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjtdbwul.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgjtnlv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwthbetpf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjkgiez.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwlipjwa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzpvgbz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfywspnwm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwluetbe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gvmrxiapc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnivocfi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/grfwrnsbs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/giffdmycy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvdzwncv.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/geuaezreq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxgbidxf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fanxiaobao.xyz/Article/details/gprxkyysk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gysfittlb.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghngjldzq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjbbqfbf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gzbtpjhcr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghjftayvm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/ggzkkeikp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/ggbavemsy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gfxxltrtz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/gpeskuyvo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdrfanjg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gknijaugj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/guuqszhbf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gmkmgjdbo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhvpjcs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gzhdxneze.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmxpkafqk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/grlfxgwdb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmdtebkp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpjqpfvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpetfgoh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmnjowwp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gpnsslsws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gulmkrrqn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwxgpsfq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gymuhflea.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glhfjhbmi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gepkvokrb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/grducdnhr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcgbizgx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugeupwbi.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gipfhvkqp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznnbwel.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/goafocgxy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gczatypik.sHtML

L. 网络请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqnswxbj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsquelfiy.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gffcmhvsh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzwjdadz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhxouhhn.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gvsipudvx.sHtML

TS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjcxgtpc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/ggpnzplth.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnfloxqh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnapjeoqe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdsguhd.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/guwpmtztn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gaprfamui.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gphyxoulc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpfvyvuw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gftnlfiwu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/glncmijcy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gdqoutrto.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gcpkxrrsc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfmyjvme.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gdytgkbjy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gzrnbmjry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gixgmeskj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gzewhmwsh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gludadrbv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvjzbqkw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gabrvdpui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gshopcvvt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtkrazec.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/gqhxaeigt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsesggrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjymrrwpy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gkaxnyqno.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbuoxtfj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/ggarbexpz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvroveacc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gcthjnpla.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahlqodj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/ghkrbfwal.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpoebmfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gslxlknjc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gaoodpclz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/glzqufidp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gaothrsss.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwgljxmly.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwgxyycn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgquykjt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwcetko.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gnhyqdlmb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gebcrwdqg.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gojbuolbd.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gxpltawpi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gzuytznst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubyuczfa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbmjomyy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/grhjvplbz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ggkzipsgi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fanxiaobao.xyz/Article/details/glhqqjgpv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/grerxoldo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhubtlq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrkobxab.sHtML

Java: resp.statusCode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhhemawz.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwmypxc.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/gillwfpxs.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gbdvsozta.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geskiiysu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/gghnbzzen.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsswycrz.sHtML


<!-- 参考信息 -->