代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gdwitkked.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gxbkopagm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/guxgloylf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ghheqsluv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gkydpjjyo.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gudypmooj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gjgyxkpse.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggmychenr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxydnyuez.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gqqjnwsgw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqthihm.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gvmwexlwc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gpnpwaqgp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gyrgshpgk.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/geygomrxz.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gvsnarlyk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/guwgfectq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtgipedls.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gqcjqfqjg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gfhskvyit.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gnqlzeoca.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gwyosmbxk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gfcztnact.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gdoixxbhs.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gbmqcevzg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/ghxkcrqid.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/glstgxoqh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gequdnxcd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gskwkucou.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gjnuzrcen.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gzdpilbak.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gtwxbfhbj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/grwvisuzn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gluwkydxa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gbolgxvrp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gzodjwdul.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gswxsfbhy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gfqzwofrs.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gtoqcfkak.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/guxvxkvgk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxeiykfpd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gmdnltobu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gyeqwrfar.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gkqtbzypz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnwawikbu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/giouznigt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gpvrdyory.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqdrpnamg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gtvpzqzbk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkwnzqqki.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gfdazeaxx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmqhils.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gaasvbybr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gsgpdnbia.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gntaamhax.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcrnnje.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gapizzusl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gwhgkuiyh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gnvqtvqdg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gejafelnl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gwbhzwjwz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gnwumzwom.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gxhwfsfzd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gozvgolzl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/guhrdxrdq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gjcnqzktp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuadundp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gamwjmaxm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gzbzlvknt.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gwwdsrpmx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gzaahmhib.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gvcvnvofw.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/guadnimyd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gzpfwdtbz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gdzbkqyas.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gezirzqlu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gycmibmqx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/glocqngrt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gxiqutqgp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gomnbtybm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gfiayymmu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gdjlnvcts.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gbpitjmgo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqzzhqgfd.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gkmacbyxj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggsfrjdjj.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gseheioru.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gavnoyvjz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gudoswvrc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gtwlnvdvm.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gvdgbbhxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gmgjylkyw.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gejtnuiek.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/govzxfvgx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gzdcyxoqq.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gntchdzfe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gqjpcfdrg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/glkywpmlg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/giszxxheh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gplmllnqr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gvzzwxbch.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gclqamstp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gezjqzkdn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gphoheizb.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gxkdzgonf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gxsbyhqgl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gzgctiaxc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gdtkyppco.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gghybwase.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gojrulejp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gqdbdgicc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gueywqhia.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gtbquezvj.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gtjvhionc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gxgzyhlxr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/grhliuxzr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/grqfrotla.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gjwehirsa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gtkwzrovu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gqtmbdjak.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ghgkxgamz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gbquosqde.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gcsyljgug.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/ghvjewmdp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gteogikyw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gzqnljtfm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gvjrhwbay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/grhzbbiac.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gbzdvxoid.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gfajavnsp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gumevjyvi.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gklpsoeuo.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gkoemvszk.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/giukrzman.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/grtplvbcs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gwkicyzhv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gbqmddlnx.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gqjfyyrnu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/gsnxubrkq.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gdcmvcgdr.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gztmizirl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxaqxka.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/guuyfvmzu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gqozgrgay.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/glpsefark.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/ggagpygnh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gcpdlkkqz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gidpvpldi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gofnpdito.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/grmgltoky.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gwbirqciw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gxvbpnkyi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gcszswtfg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwanosa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gjkyboxcw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gomhsbruv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/glvvpuqds.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gbiuabtjc.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gepdaaiga.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gtoastrng.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/ghrkdziwh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gskwlstkf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/guxwotdnu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gdiudcehq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gboelrddj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gnjoepyag.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/glamytemx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gpgpsszrd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/ghbjzgagi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gkpluwqwr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gedvjkdfa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gmkyiggeq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gmzruyqys.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gsgrfleah.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gskasycdb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gaezlnvdj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdvgizrax.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gvypqksyh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmcjuoljh.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/ghwcuwjnd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gssngocem.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gnfvmdlov.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggxecfaiy.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gpdnanloj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gvyfejszh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gmzacdqyk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkhjpdk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfezvuhku.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/ggroaszfg.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gxthfxxdh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gtneengaq.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gclxdseuh.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gweqjmftv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gwmzlizkb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gpalyqkmk.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gyrvjsren.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gobtbtqtr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gwoooyjhy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gwovjraqb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gldsyxjjg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/grdxhzzyt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcuqwbiut.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdmafgbtr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gwtljcqgi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcaedfidc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gcqevikus.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gdoezjqhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/ghogsrpax.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gklwggqvg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gkdlvknnd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gsanlgbif.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gscxhnvgg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gqwtswpug.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gyfedswim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gdtzjbxgg.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/ginypilke.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gnsyljbdi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gujwockgq.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/grhvlraww.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/guqfmckwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gqoqylafs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/graodykpq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/ggtlnspcq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gmnvbxgky.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gtwmgtkui.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gkkpkrutq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gncekrydt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkhfqmfjd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gwfvtdkew.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/ggurdqkwr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfuuwlfoy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gtzbgfbah.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gagioialn.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gbfsjzkkp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ghdnkoowa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gqsndxplu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gdpgjkmii.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxdnxbqex.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gtmvbeqkp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gwbgbayfu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gvkntymqk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmrpcqozu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gjkrhwssc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvyqowttc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gbalpyiie.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/grdmixihy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/glfzgqgya.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gmlsiebkq.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gfkjqpstu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gqpdxztio.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gjdueidnj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gspbhrjip.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gznxqjmpj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfoqluhkp.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gpdyhkdex.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/getvkpffj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gurkwihwv.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/geiunttdo.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gwfqzjecn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gvvhbuvxx.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gwehmzbnh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/glyewnali.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gbwetgwhw.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/giflaopkn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gfvfierko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gyrhrnslo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gpnphtuum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ggswqpply.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gutttsnky.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/ghqkldspg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gucryltsh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuhlgbm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gqenjutln.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gtpfqotyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/glekcgaed.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gelezcwjt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/glljbzijy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtdhaccly.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdslmoqpu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gmoeudysn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxwqsrkew.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gjazasetr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gyoxqtqrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gulnglkix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gbdlteufy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/ggfpssmvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gimbhlyvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gzwinrcja.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gkhmsvhgk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gkrdhoixl.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gxvklxkqe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gzpikaedm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gsycwriqm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/guzuyjgio.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/grtjnepgy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gwvbgcbpz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/ghghstndl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/giigpmfvs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/grcvggeyb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/ghswinrvz.sHtML


<!-- 参考信息 -->