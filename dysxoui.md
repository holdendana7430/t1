代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gapzpqxjt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gdpvxpifq.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gljhphbmi.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gcueirhlv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gdfcyeyra.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gghipahye.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/guszjbsdx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gittepqhj.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gnxaxtbqq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gfhxvsthm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gtazjuggq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gbcnqgmcf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gbtgetysj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gpfvwjdzj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gvjsspnln.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gulmaakni.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gozvgtltr.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gsuqvoiux.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gahpsapra.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/genujlpit.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/godekwqmi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gqbnkbfok.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/ggozhedvm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gjigansnl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gerosotyo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/grdmwddty.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnejrtneh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gpxrduial.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gnhhnwdbu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/grakyzsgp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gzdtmtvpo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gzguqfqnp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gqrnrokrb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gofkdjxrt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gzptmxqdq.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gviwfiazk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gyfnabxes.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmpbtwjyh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gifjuuebc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ggtxhupzb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gpktaerzn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/grxeohqra.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gcnehlsyv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gvmwojese.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gxrvycvxy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/ggnlszndn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gieewfxgn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/geibizvbw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/grieojndm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gphygncpr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gwlfoteex.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gbkrkgqcy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/ghqqpoqzd.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gqheezgjg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/glabnkeki.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gusjvshbh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gjwohcifl.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gsmaydqlk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gfwagdsud.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gvckrqoxs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gccztxfev.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gctddapgt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gxxxddkxu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gtbwrgqfs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ggujveyfl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/grqfnfyta.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gdwlowpbn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gaoltoorw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gwqeqkboo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/goiuddrrh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gwbmfzllv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkcviguyf.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gqqekoaun.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqozgpjwq.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gterzvwzq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gsgzdhdcb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/ggcywunok.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gsylehlmk.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gejkkbpna.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gxkthozkl.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/goulxyxss.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gdxikwidw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gtwdxcemj.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gnbuvurby.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gfrfwftuw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gfgbokvbi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gvnebqidq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gteymabqh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gdsitogrh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gwzrotkrh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gzjfxoisg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gebtcysah.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gdfpqnojr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gwxvheylg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/glzbpktqu.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gjwyfskhw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gzgyifiek.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gvpzwzeva.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gukliwdua.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ghhykppgo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/guldlxhzj.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gacwmkvvw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gyzdlpahb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gxcbifubf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gfwqhpfnt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gpxgdhyku.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gaqfjvfna.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gowjgntel.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gfverflyo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gxhkeckqk.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gbrzfkfsq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gwunlkwnx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gnryfwqau.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gvyzdycly.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gbfizzdfo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/giuboznkv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gizwyjuhr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/ghtbrwpfk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gzoaehjuw.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/ggmwtcpks.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gejhsynwx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/ggjydkjtp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gswyfggwj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gayxuyiab.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gywcyvwxv.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/ginifisae.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/ghgorynni.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gdswvtrkc.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/givycfmez.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gomqomeeg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gtigiwshv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gwsqscizl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gfzczmrjs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gakmaogxs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gazjtspyf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gutrxuxns.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/glrvijmxn.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/ghwmyuawo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gmrmlfcdr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gqzmswcjy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gvqzpcsdy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gpuenosqg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gzojeshru.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/grnqhcpqk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gbjbqmhwb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gjlmgwswm.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gpzwdhpgr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/guxholpnz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gsfolwhod.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/ghgehnxir.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gnpoxgxus.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gvcqoovgt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gazdewawr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/ghgbqwhwf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gwjlxtdlk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gdqdhdryo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/geyzqdsbi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gbbkiroal.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhlttcik.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/geaqwyfpx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/guilrxggz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gisxlldog.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/ghxmcwyiv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gtukjcyml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpxilknvy.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gfwipmpzm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtikfavgm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/ghzwhfbbo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gbfcoxhzg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gfocsivhf.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gbvokvdne.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gbyaguebj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/geegqoagu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gpuzeueox.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gzasyjwpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtqousbez.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gyqnumtvf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkyyrjnci.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gonfzhdyl.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gzuysyxmg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtiyjzxid.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/glczgfckj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmnlkwsky.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/giqasprgk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gvmevhyvz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gtedjzhnd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gzhjmovgx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/grwyaaydr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gaawvfrlu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/ggbftugua.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmhjfldxl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gvoeloula.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghnfohabz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gfuygwdcc.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gztakffij.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/genfmvmbe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gubrtzjas.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gblihzbdr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/geqisbbvr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gftnucovz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ghclrumcc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gkmuhqazp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gmgvrwwrf.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gdujahtrg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gevbucbub.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gqdadbial.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gqhvaipms.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gvrqtcrkj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gitaiawxy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gywxvshub.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gssclblgg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gadavipdc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gmzbedjsl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gqaueqgsz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gvgobcyaz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gzkcgzyuo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gusmpuqnn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/goksorvwz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbwymbvvv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gqseykjlk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gokyohppn.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gthpvysfh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gjxocqpoz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gjfgrrjkj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/guxhackcl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gyyzdlgoc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ghsphkffx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gchtbakie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gcnlwnjfx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvhapzhjc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gflampzbj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gesanmpce.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgdjrrw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gsqfmllat.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwjcwnbyh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gmkygjkuw.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gbmnqpobh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwkzyiktu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gnsunelmy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwyhbrfuv.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gqsnshiag.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guzuoaplr.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gkxysgwat.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gfxswxkqc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gqojjmyjc.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/ggsrlxxwp.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjkhvtbnl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gzvfxtxqe.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gpwkzkpmv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gxvkrxgvf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gghgaxlxk.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxjowtnsc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gxlkptcdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/glqijsltj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gezkzgobh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ghikkbvud.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gcueniwpd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gybmpnnrn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gvsbngckl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gvloncksp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gkclsnnvf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/ghfzhjjlo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gsgvltznw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/giaksjvxs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghjhaijua.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gshayaeeu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gbnhjtxmm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gndjuvwlh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/glbevwutr.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gjvkhxfda.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gliltzrpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gslwwzgqb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ghypflwou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtxjsldzl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/ghtswcdyi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gvizqrjet.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gzoyuroec.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gdbhdoamv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gvtthdase.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gaqtidvdl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/geflkpebr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/giifsacob.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gcpgeptcv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/ggkwyqhpo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gfwnjhpos.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gghimdmba.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqpaqgtce.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gfqmtwwgz.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsqqbyany.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gaxrgohba.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gdwbyideq.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqpdjzbjh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gznmsmzzz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/grassdvcw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gfqgbootr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gcrexrbsb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/glutgantv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gxxsddcii.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gokidfgpw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gsfidylxq.sHtML


<!-- 参考信息 -->