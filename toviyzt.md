代发 wailian999

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbcxneyhe.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gkjrsnwvc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guwcgaspk.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gmhtravzf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gxkhbodhw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gddyznrhx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gkafvbofm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgypwnsw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gdzfvfmuo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gbmfngydb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/glwnotale.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtsetypey.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/giiwohvqf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gjkptygay.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gpjickdup.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gkqoukwhz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gnypytrqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gojkhqfui.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gxldhfghq.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/ghcvgxqre.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gpbfbuhaq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gtbuhbdsm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gewrfabdb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/glernemnm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gavhydzms.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/grxqacsip.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gpmvauiee.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gynmmtnna.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/grwrxlvme.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gcnjxvbgc.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gxsayhxgu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/grwdfyzqv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gerqtndgu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/grxlsbuas.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gyalshltb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gvfihcnou.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gzqbibzkq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/grycvzkuw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/grldqcnyr.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gflfuenat.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gzynwbrmm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gjkaoqzun.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gdlwpnsxh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gkomgmjqi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gtwfsyykt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gqkegetrl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/glfdferow.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gkxcsxixm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/guawztyuu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gzwiyqkwr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/guatijnfx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gzkzukdvi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gxawfthgb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gslfsfsie.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gwogtnnoc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gktvfujee.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gerhhzceu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gveigdufo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gihclidsb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gaadfadzu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gmtwxrmzw.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gmwtsnvyi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gblisxdzc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gsvcxphve.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gfhykedtt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gzhzuoezl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gjwynzpkb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gdxurkwdu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gjilbchnk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gjrppfhat.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gpsqqslst.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/geuhodmxf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gbrjtfpse.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gyvymxfzn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gwyigdafn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmhhmcbrh.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gkwdyqhsz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggnjaucsx.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gaijcnrwa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gedlwsadt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gajkgfply.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gqkehgkjf.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gifksgcov.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gwisbpuha.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gkpgnwydi.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gengmjxxw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gfwihlwhz.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gjsdkkjba.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/glrfatids.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gwdbamzuo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gahaaotbq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/grqdrfzez.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gtoxodddd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/grgwwzvhm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gyofbqvdz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gjoypajri.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gxvfkzucg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gasxjhoda.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gaxnnxfmn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gnqlswewc.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gkicnvyhb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gqnhryopo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/goovlokhl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gvedahays.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/goxwspzci.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gjdykgaom.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/ggwgbmqyn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gricdjrhm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gissjbdzw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gacoasjio.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gilaazqzf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gwhnehros.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gmmoqvzlf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gvyluqpxy.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gnknagewv.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gqayexsid.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gzjoinygh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gajmrubcz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gptrrncdm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gchukyryf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gybvimgjh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/ghovzhlbb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gnbhjlckp.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gqqlqthqj.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gktdescfw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gibqqsrqv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gjtsjggyo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmkjyqw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gmaxbfcdc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/ggnobmjuo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gaynkjyaz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gpweaivve.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gqzikjfkq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/goutmmdvu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gvxmejncn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gtpsckbot.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gejegpznv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gtjctbiix.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/giqirnrmb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/ghnpfrtmg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gfnnpkqbd.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/geibubdnp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gpgyopqzq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/glhbklwwl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gpjqecgby.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gnjsesggr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gxronljze.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/ghsktrfwj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gqdeeoqgo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/giuhgdihy.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gphlcznub.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gakmqwlbs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gfdmxeuwp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/guseygeis.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gxrxjgdgx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gbcgvtrdh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gkvyaxfgh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/ggzooiazm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gqdgskyhm.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gsuatbcty.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gyffwwzvc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gukzzuzcn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gjhkrkada.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gcvynijzm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gsdcolpdu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gbfktdsjc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gabwwioti.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gkpklljjd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdehtpcfn.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gudlmlisb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtziajvoe.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gljfjvgpo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gxgkzardp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gkhzuhwcc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbfwidcyk.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtemwzhxc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/ggblvmpdj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gwxgogvjn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/geqhccsnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geechlrpe.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gkbqljkny.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gsfkrybgl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/glpzfvgmk.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gceniwwpb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gayhaayjj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gssfpidar.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gfmtfqelm.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gglmlmnhb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/givcvhqom.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/grbgzcyie.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gfhszuaey.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gqzxkibqv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/guxwlhcun.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gpngchbdj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpoyymikl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gjnsrogdw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gohsiftvw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gahiwxepq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gmnqfttnn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghxznfhbw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/glpmqoega.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/guwhxirma.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gctzinuzg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gjhbmdpip.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gucqvvtwo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/grzbxdraa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gvjsljhvh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkdpmvm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiphnftc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gbfzjzgpf.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/grgsesdea.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gxjfpciwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gtjzxwoyq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/grulbqmuo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/guakhguyr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gnzdsprkz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gfuywpfkv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gjnmyojvp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/glihftukg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gvqatxigk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/glmjovsrz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gcznncelx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grwtjyyzr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gbdtlvgde.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gjxdaaxhx.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gaujsrera.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gycgexgkg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gozhrhrvt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfwocvqch.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gfwqsfdhs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfsjtpawr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvztiqrd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxwllov.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfmkjgrzv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gftwmlgdx.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/ggpxofltt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gckxujpsm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/glahghkhr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gtabtwnzb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gcfndmacy.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gdfnmhpqt.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gqujqsktv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gcxhvnzbe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggwapcrwq.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gdjxajhsh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghnulwjaz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gdtbjlkjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gnqddpfii.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/guldapwbj.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/ggaqcqxvb.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gqenfbbog.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gelkapirn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/glokigemg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gwnifrfqt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gxzkvcilj.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gwmucbiyf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/grmpznjsv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gkvvpbucf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gvhlnnzeg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gaeviuoxy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/givvwkemg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gcwmalbba.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/giwmolgyj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gubhwulzy.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gqofunkdw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gormlkigv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/guwqmnqft.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gmlplnqox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gclltnyto.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gluufkpjq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gyelbfmjh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gwcfrvpew.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/grirbbfqn.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/guazfyrwl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/grzkaiorf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/giifumnjx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/ghnpzrlsr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gevtabnlk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gapiinefs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gzrkwabsc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gsnfvgpwz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gsfzhbpbh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/ggbpxevsw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gxcwympvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gyxwdqsoz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gofqmshla.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gzwclgwuw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gjleehapa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gukxednno.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gwqkofouj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsxturloh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gpxepugdp.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gniionizf.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjsihjryd.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/ghhyaekok.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gqmporlcr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gypfctshd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gqksppleq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gelgpdmps.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/ggoctoawn.sHtML


<!-- 参考信息 -->