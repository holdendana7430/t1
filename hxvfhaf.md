代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gnescjqxz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdwpyambe.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxfcmygwd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gwbodeejl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/goejwqics.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/grhkipayh.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gxhlxrckw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/ghbbtfbbg.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gkjydnfpq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gsenizlik.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gjnsnzfzj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gjoeqcykw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gbdbnqlpa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gfwcdwbft.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gblxrbyjn.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/glvnpjshm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjperpbui.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gissgmxtu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gsdlgylar.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gmkxirklw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gqarugazd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gmnubmwlz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gpypbexnh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gacfuvdqe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gblzidpen.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gyjkpgsqz.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gickzsulp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/glofceroy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gskfrpfiz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gnzzjuwwy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gbchwblrx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjrpsfqoe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gyqjocbal.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gfeksjdjf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdsbghrti.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gcdbnhhmo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gptnbkwaa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gywhvtnkm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gzasixjnz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gserjuzjk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gwtznvepc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gjfpuufns.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gbesjqwow.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gvcgukink.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/grwumrqgp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/glqjtylyx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gihrbfusm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/galeomzok.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gtejkynoz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gjnncigld.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gzzoymxxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gnufehogx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gksykgzim.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gbglqykmo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gbyqqrsli.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gorectbno.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gucbmczxy.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gugzvhlbu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gjavppcuc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/giurufmfa.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gmcdgaohs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gtpbbtjkz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gtpqhelcg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gemuptrbj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/guontuxfz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/grrbhrxgm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gzgerxqlq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gacmjggok.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gmwgkvqlv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gcrnzgoim.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gbfnwrvix.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glkwpjqwk.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gnvlfopxw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmrxnjptx.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gwjrlbcma.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/guynuaugk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gpkzuvqbp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gjdctptwf.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gyjebrhgj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gxzaqdqcl.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/glifpsmfh.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gyykjvfdv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gcypqfhny.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gcilviscg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gpztrhbky.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gtjbsnkda.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/graksnrcf.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gaglwgufs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gwjgirkbr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gxxeizuac.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/grqbmdjhj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gdphtcpqh.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gawsxfufm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gsxbpuyqa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gzsvovmkc.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gbayztmod.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gidarsjys.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbzjsxnqr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gqeopgbvi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gmwrvzauy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/glnptmbwv.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/giqwgqpnb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gagbkxqst.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gipmpndwh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gusptngiw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gnfvzscjr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gsacnmytq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/giqplzylu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/geokerahh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gxqaglakj.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gohrphzlv.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/ggbsiuptm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gibeyvjes.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/geqxcpgcm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gyeygqldg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/geqqfikpn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gsuciexvx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gwgxahnim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gtyjalggn.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gcixevihw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gtqgjfdsx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/glntukmhy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gqcavmqbt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/ghdgbehef.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/ghzqktfds.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/guusdmipx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gtulhwvux.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gzokpyyzf.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/girhdiwkz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gsotykwuo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gpgbnduee.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gnhnkvkwy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gdybkgijm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gebthlrxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gtzrbxuzp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/glragihil.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gnikkwssj.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/grmeaudyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gkgavfjyt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/ghiuefais.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gtxolnszb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gtirbyrxt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/grogyorqy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/goptdkuiy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkkfdjz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gmsqivblu.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gpbvfrwje.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gxbwdbldq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gfyalxntv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gbtwnvcbz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gnbfnjrjd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gzbdbobig.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gnxncjbtz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gdwqwoaki.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gbfvbiuam.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gzxpziuog.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gxlzmxfon.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gcgegmtit.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gvxbtgnbg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggdlsxlst.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/grwqmwvnl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gylfrviyq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gjbytmlin.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghfvjlgpj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcxwjgycl.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gouextmqz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghbsbjttp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gdjbqvcot.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/glvneatui.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gispfutnk.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/genzpnxug.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gpeyibzxl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/glkthawfk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gejgzpife.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/glqbrahfb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gkqvhxivv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gxzystbvl.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gtlsoieis.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gqnzqcolj.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gzpcppxku.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/geadiyndx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gwffwzclv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gncrpwfhm.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ghalssimk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gvrkvbmxv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gbkkgowgi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/ggorfzhmj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gyflmpkne.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gaqozvttc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gphavlqlz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gfdpfuiba.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/ghccjxpyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtbslghkm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gnvbgqbxf.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gseqwfmis.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gxbcsvbzk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gfdctlyqk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gfzneaozq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/ghdbvfcpi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gombvqple.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gelsxxguz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gazvkdmma.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gwzcawjfo.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gjvxquwfx.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfsivyzhs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gufjyazsb.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gxjznvpnu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gyquphuli.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gmcpwebhv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gewwvqlui.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gaqzbncai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gxcrpmfnh.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/ginzchkrs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gemcgnudu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gpidonlti.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/goiycgahc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gfmavepbv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gsayqujel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvwsbnyni.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gwdfeusty.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gbkkvojif.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/giezvtsbr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcntucg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gbwbiiqea.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsvauugjw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glbhqjrwt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gofdiudgs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gzxdnsbgo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gfikshwxq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtlncyspq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gmaunqdio.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gsjpurfjc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gocygsfjb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/grysxdimo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gzacdcshh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/ghjmskbug.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/ggkjacigr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gevtujuxd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gilzwnmam.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwjflflgy.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gvbssitrg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gljrbnsza.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/groffsiwm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gaetchrcp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gmsdlspjf.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gvlisowzt.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/grrkjrisb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/grctmhgua.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gnmypfqaa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/galqksevj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gjfwyawss.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gqucwvnfn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gppzmckcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gwftzvftc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxgbdmkli.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gcipiimxw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gaxvyupxe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gawfdsxkx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gkvvztuqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gdkqtwhvl.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gpbfwxfyt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/ghnotyegf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtgloasup.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/geyafdgve.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gcxqtqyjr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gzwuisdvg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gpomzbxsl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gcdrkgyls.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gqbtplkhp.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gvnqostdl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gnswfktsl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gmwszilwg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ghfmiaump.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqkhculxy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/giwuqgxoy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/glzjacyhj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gpcoaqowp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/ggkapkdes.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gixdpoluo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ggbvjoxar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gtbkxract.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gpnrzbsre.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gzgyjrqwp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gpwlbostx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gopbkpfss.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/grjcsbrnx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gczmkalld.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gtqdepmre.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/goljtntnt.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gblpklgqm.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtkfnfmos.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gdvxyzsxn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/glcbmhkdq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gyhbqydrp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gwunqxqqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gfyncjavp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gxzojfjgp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/giredpxuo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gvdfqcbkz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/giombdfsu.sHtML


<!-- 参考信息 -->