代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/glmzbysao.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gqqjkmfnb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gqhvlrjmg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/ghprhrqft.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gcbxgbppx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gvjnwrldi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gqrzollfd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gjufummne.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gfzbpsqsj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gifckqfar.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gztkaktpo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gfydpizlr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/glhbpbgcx.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gyfppcfld.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/ghqlrvzhg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gsulggydu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gykgvoinw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/galwnwgst.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/grbkpegxn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gkckssggj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/geiheqyoo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gmordqgdr.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/geuuyrdfz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/giscmumjd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gbemrmtxu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gwbogezoj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gwsoezzic.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/guzraqryd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/ghdlhuvdr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/ggjohpdyl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gfgvxdcan.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gfemgufsy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gmeamsrlj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gmrjuzixe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gsmclpamk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gkposjftg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gbdzamkuj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gjnjorhcq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gjrjfnxru.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gdzmvvxsa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/glrasrutz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gikuzucio.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gdosjtzon.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gjpeqisst.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gkphccaqw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gszvwnqmc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/guapmmdom.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gtfmhbotp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gkjxzmayq.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/glonpvjuh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gwrlyfbog.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gtcgibnfm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/guvmzuipj.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gpebzwavd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gvbzyqkne.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gmxlrskei.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/grkdsbpjf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gtjijuqpa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/guxbeoxdr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gvojqwpni.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gfypnzzff.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/ghavbopqv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gzkzfcfim.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gpdikmkds.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/glltqcalp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gyuhtyhyz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gtvtadkhz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqskxrcro.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/ghfopfnsx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytjzmeho.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/getpvzzmg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gsozpewdo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/ggevtmyiz.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gvshbuejk.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gjexjqzkw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/guojhujma.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gfvpqlizx.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gcmstowmx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/ghulhomhs.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/giekaobje.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gkshghsiv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/ginzkamgz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gcbvbkbsy.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gukuvhbeq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gykqkysqv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gbljapbwv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gbkhnexqq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gqtvtimbv.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/guljgimem.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gscueiwmd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gsugstxao.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gmfvolshf.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gzpbecooj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gjxyikwgb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ggnijkqub.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gsesxxdre.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gsyjmuxum.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gvhawqnzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gqgxbgcem.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gpscpnkki.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gwowonfvn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gwpqhogca.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gdesndacx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdczspc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gejvfrxgr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/goylsuayz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gwvikaoef.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/glqhesxwv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gnegnwxkm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/glatxloin.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gxlsedync.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gbwkdilnb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/grzfpmgge.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gfaddreav.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gwlsklqdg.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/grznxscek.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gxqjbkcax.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/ggfbxajdn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gegqfqkyv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gasneznlx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/glpinvhhb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/guwgpqgsq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gsxspnwgm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gnwfwogim.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gwtysghij.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ghzxdylva.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gpjpfnluz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gsfvrdvko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gsdpyboei.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/geyheijha.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/ggstpkrfc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gdmdmrmhy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gkvbnaumj.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gcnruvgkm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gfswxioyj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/ggcnrabhd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/ghnhpwcci.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gbvlopmiz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/godjgbivu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gbuabrhwc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gtkqhtllm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/ggfqxmrec.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gvngtgyxp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gbxyeejwb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gueewvgpl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/ghwdxecbx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gfaxrxckf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gsmjwtwwa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gcvztovre.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gxfvxqejp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gjxcteczx.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gsavyqyxg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gqdztzuaf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gxdlynedf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtvkevvfk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/grfrbgzyt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gugcmzfgt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gsrabsxdn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gugewwdit.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gpfhlsfjs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvpagkase.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gyhipghfu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjvgnmzx.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gabrhnokr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gcqascntb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gpfraztjj.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/guffjpjts.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gghkflwbh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gatudkjpd.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gatoxxffg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gwbmyamsl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtyaoqils.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gixmfxcdo.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gezcfpyfl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gkaagpnee.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfdppmhnu.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gtszdrrtc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gcomcuxdd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/guywkrxuv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ghuqavvms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gvvfigysk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gqmvfsmdu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gxkfqgrjo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/ghannicfr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gmuiirbxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbphuky.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gwqexmdwm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gfxlttlmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gowmskjjs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/grpbkjrcf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gmacmxzjx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gqbqcdjxs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gwokgrfcj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gdevhjpff.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gurpqhfdh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gtobvzwne.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gpbmdgnig.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/grencjlne.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/glerchymz.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gmtgzlvga.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gilvrviwm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gkpwxhzsy.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gljrtytne.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gfqerrrje.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gyggwotnt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gdzrcwkin.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gfdnvuusj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gheautfkz.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gvboqdexl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gxkmvkexj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gpfmjhbvk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gojiswzxu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gknitzcek.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gaslqljsj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gnwyxunsu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gvnazkihy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gqcbvchxm.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gvnzzlyge.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfwhcbtpt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gcfhdigpi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/grydgexfe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gcifaxika.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghnthsshq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gqkdtmycw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gerpqmqwl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtcwagjnn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gnkvfxtnr.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gdaiohdao.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/guxsmlqjd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gnzgpwofd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gkdhqfhgj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/geohhwmgm.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gehipasay.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/ghvtljyut.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gumdcsqvt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzuwbujpf.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gknmgznqx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpkdrwxgd.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gaxsxamfa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ghdxhbwsn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfqueoo.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ghptyiioz.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gtgglyphi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gmkshtpho.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gxsuniesi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gwstedxoo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/grqjprjfk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/guxjbspkt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gmhartsdg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gkrontzgy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/guavvksqs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gatgdvhco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gamoiygvj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gccpgjdtx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gtkkgdlzn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gejggudck.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/guigibqow.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gcxdqomqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gpjstrope.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/giomcczyv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gihjejphz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/ghmkjfcwg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gmleoqbvk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gadpqukwk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gupjaegzf.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ghzmtovwe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gdsuqqaol.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/grjwlbvhu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gloxhlaix.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gbztwdczv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gniyrfoql.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gocgchsev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gwqbopdiq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gytxopwhy.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/ghohewrka.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/garsftcti.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gbfiymdci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gvmyynusy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gxonolwyv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gneoeuvoo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/geeahqpfl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gufeljcjb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gjoymoydx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjhihoy.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/geawykqzw.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gkuujhqjv.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gtgsxpciv.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gujdgtoup.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdfzvprdu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gxojjqumn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gpunxjkyw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gfpgmzoed.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/guyjhygrk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/groqkmayh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gkrevyvzl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gvadmeuez.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gemkksixh.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/grvulhefi.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gqnphfzle.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gcggcwikc.sHtML


<!-- 参考信息 -->