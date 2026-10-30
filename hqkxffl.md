代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuyfrqlv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwspsutkn.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdizzzni.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbdejut.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnecgqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glkhncnjq.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/ganycqlax.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpuwcqgr.sHtML

[I02] 提取所有匹配
来源：http://wap.fanxiaobao.xyz/Article/details/galhoklxn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/goazmzgll.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/ggyihbzll.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gaqtocxkk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbzfjhvl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevandrgs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcybvqwct.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlwkhiha.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfsgseg.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gjgkghlyx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gudkdvggs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/givnhpdjo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkahhbqm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzyrwpoc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/giiqpcbex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fanxiaobao.xyz/Article/details/gwyodnssn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikjuxpfk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gndafasff.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gallqjomm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gefumxkuh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxvmqdz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtszfzwak.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibmcegad.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtjnfjfd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gzkdjcrau.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnesuuaww.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gvsrzifum.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnprtegf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gryhyavly.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqubkbww.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwvcsrvv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwcqxgug.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtthuneb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcwyenwha.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvzvnrby.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gmoxnfcdq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fanxiaobao.xyz/Article/details/gzvggberk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwfqqky.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gwytniqwi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhfogzok.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelbfebka.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnwkvdwr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fanxiaobao.xyz/Article/details/godkduqla.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fanxiaobao.xyz/Article/details/genfbxxzl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqnuwrmg.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/ghzfeatpq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkptftqig.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmafzwzq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnzvdpqd.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gunhfnxko.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskvulhgz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gobtporro.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfriurkzj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfixuryfa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxyqgdhz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmlttgd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcbaxmbl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqozfarw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioatnpav.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gggopilgp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzfgwttr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fanxiaobao.xyz/Article/details/gpghbohfy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gqqamjbho.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvewffejo.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjlfckeym.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giotviwkv.sHtML

[J01] 获取当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifaxoddn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidufenl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqgtyahy.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/grudzuyaz.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gohewahwe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyncunbvd.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulcotpzd.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqahlnjd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fanxiaobao.xyz/Article/details/gaptwvqpw.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwudwziel.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitlixllg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqioxqneg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/goxesgxsk.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqvbjgpf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fanxiaobao.xyz/Article/details/gfforamgb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gdyxyxveb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdxbsybo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyjgxfiq.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gbohbcytp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gdrkpifcu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqixoqpuz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gkaynmxeo.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqmecif.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbopdniwa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/glzstfjlt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gqtyixfpl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsymyjzcd.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fanxiaobao.xyz/Article/details/grlglxucv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntglrlbc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxscuaqp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyjazrsb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcyaycwa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqineldd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiomtolk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gtftscheo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhpexpbn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfynaegh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjtrytzv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/grfwhhucc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbgmgus.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqnhchq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdpuhali.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gdzhwhgck.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhlvoil.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaduxecv.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gjatpcuxu.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/ggafazjcr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfslviae.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fanxiaobao.xyz/Article/details/gffsulimx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gearegede.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gzruehpqh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxabinnh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gdhxjriui.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/grkdczqvt.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guumzihpe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtloadlzt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuhooccf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqynilx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdipqaqhw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqbjcsp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxrxjqq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvuxqzaw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzdsupdz.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrybotx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbqzczi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqtwkcw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/gesfumxrm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxxozimb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqikoimz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/gxltridsh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnekuenr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gephcecot.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gmtsdunbt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsnwdayw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayjvjrfb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgfbmtps.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gbujpfrpt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gztpvnvnu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgtlrwl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gbsewrgmz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiyrkfwc.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gfujwxfgg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/giepjijid.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gvbciuxwg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsgxuirkj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwhlafgb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtioewcx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfozlmux.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhawmgyd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjryxvyd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfslhnok.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnsqdvq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggaaqgxiv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdmcwgib.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gvimfrjvo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgnnoygy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmrooer.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkznqasjb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbifyznz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnuaohdit.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthkzkdt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhestxzr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gotiiynoq.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnjagiov.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmahwnyam.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeesgccv.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrajqmzr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gazzyserx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gpisssiim.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvcykktw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavjquyeq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/grmovgusp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgvtxsbi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsezpwyn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/giuwtkjsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzavctehr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzjrmyrp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/girlikzbv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glrurvrqx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fanxiaobao.xyz/Article/details/glgscxsdv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkzsehue.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gyqpvsohg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzaqmhut.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gafuavsco.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxtghhv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgsmmgrh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/grtmdvqtv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozrjbfp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvctkmgf.sHtML

[K05] 深拷贝对象
来源：http://wap.fanxiaobao.xyz/Article/details/gzhpwhkfr.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdivqyupa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrdjhqlh.sHtML

JS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glwiwywpu.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/galoihcwp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gtzlarfge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwtitdp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgajuuwd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfjpnyb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgjpjmpz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gyycpawrk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhezgohu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gqbolgqdz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdeeioeh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdopjvyls.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyxkqzlo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grblskjtt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhydilz.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaubzbmc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/glmvqnvgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcjxcyvv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gvtutxans.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaqkeavu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhvgkas.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwygriupp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geplkdmuv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyaixxgz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/ghdsvdajo.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjnudxi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtxmvka.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydnoqbh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerywcpnn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gnhxeikrk.sHtML

Go:   encoding/gob
来源：http://3g.fanxiaobao.xyz/Article/details/gqjacxoqg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsaefvzf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gjqmchneo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfuzgdtgh.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gtbcufqoc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstqpfab.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/grydtgxxp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gzeqdczwn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gnhbuaabo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdmvefea.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvallarf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwmfmig.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmicugln.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltjbwki.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gpozwyxvj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxqwehnd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/gnozvyvij.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhwkmrbi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gubkxmerb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbwbbtov.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gfejeglul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fanxiaobao.xyz/Article/details/gpkvaejpe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkswlshpe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefyfpjhn.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gmsebvfzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrymwzfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftaaqrtr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gxoixtawu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiyordec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gufcyklne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/giptoaxte.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqqskgep.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gpdpasyof.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gafkpkrnh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grielvtmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrnnwwo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gboswblqt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqnepvlp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudbqdyoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gtyhxowgh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjoczpeg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdukseml.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkjadczh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gjuykaxsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gijzctvev.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrzifhqb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxhfmxcf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyirkyjli.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/getumikzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvxmpwky.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/ghjvpliii.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvdkttul.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gajthdaqh.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glccadaep.sHtML

JS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gwbksucpp.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/giwxwythv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gokkuapge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuyvclwk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgojwktg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/ggobsfuhz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjecdysy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkumzcq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gntorcbxx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfvljowx.sHtML


<!-- 参考信息 -->