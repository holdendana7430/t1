代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gvxzizopd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gzopqynyt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gpmgxqnby.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gdgziwxti.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gfpruzswc.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gxpipcnge.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gvtqpocbd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxaolhhxy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjlcvslps.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gexogkuca.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gipgeldzr.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gmlqwkktb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gkzxxjjpp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/ggblxcvrm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grslqytyd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/guxjdphag.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gysgabdlt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/glgfarxpa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gyvapqlzv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtnanejhc.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gswtzpznr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ghajtwcjk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/ginttrcro.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gyarkftru.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/giawxuimc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gcqrshfwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gheqomqyh.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gdxmclnya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggxxmtrst.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gbqlntghz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gpuyflxph.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gljnoldyh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gheewcqsx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gluumswup.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gdcccuoam.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gajaigpsl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gobhtwgye.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gwontzvef.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gphslscmh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gifzrbqvd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmezfary.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/glytbzzen.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/ghppegqdi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gggnonpxq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gypahapnr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gtyptavhm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gaffzgbmb.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/grxbpwsoz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/grrlairxl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnvuyiufq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gdpgmvybc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvtyexs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gxxovkrqj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/ggcolhjfz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gygiehedw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gqngjbpbp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gtnbhqqtr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gotdftvtk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gkpwisaia.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gmwxwatyr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gnyvmxcuz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gyhcxxctq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gnbgyisjy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gjuiesyqb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gkgxecuak.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gvgivutwy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gkyzzdvuv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gzmyizygp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gtfersfyb.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gclmxuuhz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gfrnmjpua.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gxiinsffr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/ggedlnqma.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gpwjiyxjr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/ggedqahhn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gifxrigbi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gcanzwczr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gcdejnkbf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gllzohhmi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/grnsftzes.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gitnmukef.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/grgjtkrdi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/glxrqtsrb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtxuuzvio.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gppdcmlai.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gidyqpxgi.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/guhvturmu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gtmpulcei.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gygkccqgt.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gwsikxvab.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gcukvcsrh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gkcbvjohc.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqurgcs.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/goskibxhg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gqzplpfnx.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gvcvszhxl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gscmrutkz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gsikwobov.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gefhymklv.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gawofwjpc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/ghxpmpnbz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/glmixlebv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gokciishk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gqcdqjghl.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gmicgpbhe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/ghxtrxukh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gwhtevanv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gvmmvushf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gnwvgukqd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gttnqboao.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gherpkuin.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gltbvntye.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gvlsehvle.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gukpbjotu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gzlildpfr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gmuisobzc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gnnaktrrw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gleprkdne.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/giqmocnar.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gmjkuyrty.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gaqfzzyid.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gtpajwjqd.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gjnbgqffq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gcpvwfkdk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gagoomvxn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gwlwmtttz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/glpdsryjs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gumzvrwhk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gswrwxkkz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gmsjrrviy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/glggixupk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gdxxtopid.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/goyqmllte.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gdhmzqdmx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gcqecvnvk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gichxkqmk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gqflteomr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gccxjdbng.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/ggecsszjd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gjpoiwrmm.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/ggxtjaasi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gjywjxcvn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gyonlodfk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gapwwrwko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gdeqyrvnv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/ggaqlyjev.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/ghxkoldso.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gykqmrkzq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gcqpzxtvz.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gzwrktatk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gbpwdocsy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/glusomzvh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/grermkolc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/grqpreapz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/ghkpyjjyd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gxuffrosp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gunoqgxlq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/ghftazaly.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/glifoiepy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/giucdzlko.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gmbfipgty.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gfnekiput.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gztebqqzw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/germggkxs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/grrgrmahj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/grzrnfihx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gnpqkaggy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/glsbgeigo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gzywiqane.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gwvrtkrvl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gdgwnnajw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/ggibfzlnh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gybiocmvm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gkmjcutow.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gpezmsvfw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/giduemubv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbyhvhdip.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gqmkatqed.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsiusnomf.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gmmxzqebd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gqtvdcqin.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gmevwznnt.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gsfuswtto.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxyxvqmzv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gpftsubzq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gphyqlvwu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gxhfxblbb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gkbikaavu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/ginolbsxo.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gjlrtgyne.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gimclwqan.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/glnwrnxue.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gakzdyvoe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gdsvnovoa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/ggmstsrkg.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gskxtsvpm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gmottvrny.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gtigvvfte.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gspoctlov.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gyzrauiut.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gepdflsjy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqvihymsz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gkrpdaiwp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gviuyvpft.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gygkflitt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gfoyzsmne.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gdwfnmhrd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/ghkcfxcil.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gxjraebhh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gaytyarcr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/grcffvwcr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gvsaizfve.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gmxfhrprf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gifqplfyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/ghrlsxqpl.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gmajdstzd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/ghtzimpbf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gdbdsoyuk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ghbuffqbw.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/glaggthmy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gznicbqir.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/giimcvrpr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gieqjnota.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gwvudjdlf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gklohgaci.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gegcpbzsw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gzfnpnwkt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/getewzalr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/ggdfudajf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gcsyrpddq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcruperua.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gcndxvnut.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gaawterli.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gbnrolxoh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtfuwpkzj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gmnndgain.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gnlaosxek.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gisulkmuo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcvdhspgu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfoodjcum.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gicosuhbk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gudhelxde.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/giobvgdno.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gtbumwqht.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/ghvuowtac.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gcgzzfana.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gvleepqjy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gbtgvkulz.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/grlnbwugg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gokyrutda.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gnnylnbpf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxylkrdsp.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gcxxzixal.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnmcjetdu.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/guruznqwn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkdtnbyek.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/giuyucdsk.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gmtwfziuf.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/grvflpbhx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gsyntvvie.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gevloxhko.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/godfnhvlz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gisxbhicp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gubsmrbud.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gfzsvheov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gqxcrdpdb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gjlhfbhto.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gsunuliyf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gexucjlrv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/guvmtjdbc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gvwyzijzv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gnsfsidol.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gufujmqjl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gjmbydohj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gxyofrclp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gokrepqju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gvxbhiqrj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gxpljotpj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glybfvjtt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gklvghjys.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gifafmzdh.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gnaubafhw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gnufrrxtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gnaximvtc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gjrzrseml.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gnlweyluc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gbyrbbods.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/goxxcbnpo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gpyxwwmoi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gomcqakkd.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gbbqdpkzo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gjwkgxsjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/giooqeqbu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/ggnkcmanu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gxhqzbpch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gjxozosjh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gxowbauco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/grvyxbfcl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzndogzme.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gcectkvld.sHtML


<!-- 参考信息 -->