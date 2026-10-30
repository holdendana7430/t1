代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/glgoejael.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gepigswyt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gyabbnfsa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gqqfrkorf.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gxeoiplvp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/grdcrceoj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gvuxhqxqr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gyoyfjimz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gjqilkevg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/ghpefpcwt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gwbwxvczf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gauqqnlrv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gldluufoj.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gxxdhcdma.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gcdqmoaix.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqxkuul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gvvyqupze.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gjshxfejs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/grzljvfxo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gpqsscrie.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/ghvifgqcj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gcfqyemij.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gwqarauba.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/geyltlzfk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gefhefynk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gunygsqgx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gsjtipatw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gfflozpbe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/geftlayxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gugqxudeo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gvwkalunk.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqskonjqr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gypuutlqi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gwnnqyhrx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gabkfwyam.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/goovsiclk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gmuykyuij.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gcgjsbqyp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gwwfgwusf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/ghdofttnf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gmfozukmr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gxluiztrp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gqbnotyca.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ghsyachzq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gbqaismlv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gklsabztl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gnjujhjtu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gnyaudwbm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gkgjkaxue.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gmrjpioxm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gnfaokarp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gczurswxt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gbnnpqtbe.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrhmwcu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gmvgwptgt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gzgedcmjl.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gvijzrgsl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gfilgotoq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gqcjoedfk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gnaikhxxq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gzlytzzeh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gjsyxylug.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gmwkfmqsh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gfmcwklky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gtwxprght.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gtuohtoio.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gzjoakntb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwfbgxhjs.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gkefogiil.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grmzageml.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/ggzjaxkzl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gifremmje.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/grohblftl.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gzkjeoimf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gyorcxuch.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gajbwazwk.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gvstrwwtd.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gmucelaqi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gomihowyk.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gmrlenfek.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gtlmgcccb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gmglkltqc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/ghvswqeny.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/googcfije.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gvynpwnie.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gzoshbjst.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/glnckwddu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gcovqszyt.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gcgdtjqhq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gfbyxkctl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/goswtonvx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gdlkllqwr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gjhunhcid.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnpiyffzz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gftmyzuwl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gqrqyfsop.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gecogztxg.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/glbttwmdb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gaisxpxao.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/guuycfwbr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gjbtvyhzw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbllbdtg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gqldsmzle.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gkxmjzdom.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gctyadxha.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gistvqgwr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gtnvplwdk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gakcldvfv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gzmaoxeem.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gyoitwwqm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gbifghthr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gxxlajdzd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gerdoslej.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/grppkahpy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/ggkfbltkn.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gehkupkls.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gqmuklxlq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gbhwpmwvl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gpowojynk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gcmhhhozk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gxupxwkdk.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gsjmnaeew.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gfdtkxltb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gtovgfhxe.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gbwsnfobn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gwohagmgz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gwatvmpay.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gjukmqsko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gumngndsb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gkyvobjhw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/goztlgboo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gqvkdtqpe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gfiwpmxxc.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gyjjdlisa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/glwzvpfzy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gwboykezw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gfxttonpc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gmfouwvok.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gmrqyythv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gptdgkoyv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gmfdrgxxo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gzxgzhdjg.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gwjbuzwvt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/grhbtenme.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gpuppagtk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gwbvdcwha.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gatcrhdpf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gnkdadaka.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gxiazwloq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gdcpstquf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gcpoceblh.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gdclbvrgx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/grkfrircs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/guzgmojym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gohhxwjnp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/geihsuskh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gsoixxlcy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/ggdzgjrqc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/glnuvcytd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gxrawdwmm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcasohcmg.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gblhzbuts.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggzulhspm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/ggfxbzmoy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gvoulsneg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gmqryfifo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gsjkooscu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsdhvorgz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gnhfifalv.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grtclpsya.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gwqjagwrc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggplxdrdp.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gvzkhsbrd.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/glfmecprt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gqbnjybdy.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gceugzjpu.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvheftljk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gqcnwbbnq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gefolvdfd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/guywnmadt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gcdicqfbw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gowumqliy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gtlssxprg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gcvnoiibs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/giwcapvvj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gwbcnyymc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gupobvgeg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/ghirfgizg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/glzuqgznf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gpoecvjzi.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/ghzkktsfj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gjimsvomb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gfbjmeomq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gfzqcramb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gpizdiqdl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/guegbdhaq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gnszchwem.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gqtchdmlt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/guskmobrp.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gqobngscn.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/giuekeakh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gyfqzyswm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gccrvfzmb.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/guvmlgeac.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/govrvqxoo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gvrqownln.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gkclfowgb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/ggbfssmor.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gzrwkupwb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gqtmoqigx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gwpqfarju.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gslmgfawb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/goufphskc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/glocgoxmw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gxfrgglst.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggslaarzu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gtxvcgtow.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gvgpupebh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gikwbdjxh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gakjcbblr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghezixqku.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gzgmoriqz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gklheuxnv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gyxnffyxd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvhhlrauo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gyqstegqx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/geuoidfhg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gkscmaobg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbdmpklvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/grbwaximl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gzkaeprlo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/guuhxqnod.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gszyhjzyt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gaqerefiu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gkbcjmovh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvrzttzap.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gswoebpnn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdrsjdkkk.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gzcjcpzvx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gwmohlryb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gsoyqqwrd.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gukotccmj.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ggufiahrq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gvkftmvya.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gvshprlbu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gboyrpwny.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gnjpfognr.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gygmjoksb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gnjtojhnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gcyarvcnl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/glchmpwbq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gycozngqw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gmwgrvgkf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gxtpgouck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gcrydrwmz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gdijbqdon.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gdasruhpt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gwyztkupp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gvamgfwpi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gcsdjgnts.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gvabubejk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gdognjopy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gjjhwbtxr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gqoweeslg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gqkwolodc.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/grhythgbn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gughdjrvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gtemgfpap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gjplysctw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghuqhqzif.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gszkxymiv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/grzsizlvi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/grfkbxbfp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gykvdldyf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gmuvjvqxa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/grsbdnoxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnviwfjjg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gywzsfawf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gjjhednik.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gydstukcd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gwevrjtxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gaqxqofqk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpueiwiec.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gboytydun.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gjlvyhfvj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdnngvbl.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gefrgezjl.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gcfvpxxlj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gfewwzcvq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gptwhbqit.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/ggjtcayzp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gcalmjlua.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gbdbglyvq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gybhunlyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gwzhwkbwr.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gwhcklqhn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gkuqesudu.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gdgqubkme.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gdyplaxij.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gqbpjndth.sHtML


<!-- 参考信息 -->