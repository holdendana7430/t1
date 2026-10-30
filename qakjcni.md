代发 wailian999

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqbswvpiu.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gajlawfya.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gviuwbjos.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gzyhavwet.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gvmgrdqgz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvazgkvpj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqmgkcsrk.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gwaohtdvm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gaqvirtbh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gdiwtznng.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gzpnzgsff.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gxyluigrv.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gccauhhgo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/ggolfhhcx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gwtohcszp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gnozvcaxq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gtaevuimt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggvfpoygr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gwznuucty.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gmyujexlu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnmhstiwo.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gliiddydm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/glbpyumaz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gwmgspvxc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/glmnynybz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/glgdxlzbx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/ghnqktqlp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzyvzsg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gznawohrq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/glhlnuwjk.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gtxmlkmpj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gqesebbzk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gfilrwyia.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/grfrzegvd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghjucmlpq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/ghtmbpvdo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gapxxtkme.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gqrgztabi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gvlctmeor.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gmapgipnb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gahmawwel.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gsvoidnim.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gktuigkpm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gymjunskt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/grcnapkqx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gscqfolde.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gyrtuxmoh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/guehwmqxd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gmlhiocwg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gnnurzfdq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gbwhnuqut.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gstfarzqg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gjbqpxjmw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gdistrghf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gooibnbai.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gsvbavoxi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gqkkwdrsl.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/ggmatqgkm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gkfzssomv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gczlddhst.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gptphloom.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gxzzbgsbd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gysjgspup.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/ggtufodib.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/guntdikev.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gteooaxcp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gahlufhnu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gotlobqii.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gckwnnncs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/goflmikhg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gcqgodycu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gomalrcdo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gyouachdn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gldcsmkww.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gqeidivpi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghnchprcp.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gvlfanmlm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gprqliybz.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gjwfjeslq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/garvxhnme.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grdpvlioc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gvesulcea.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gxruwhvzn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gpoilnwrn.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/ggwwejmnj.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gygjtblbk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gxlyyiogy.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gavhyxaxx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/glgxzdfqx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gyenoldgw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gisquilpw.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gtovwmyhg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqdjhox.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gmigdnirs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gbbenlapl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gvkwfkgyb.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gvdpifsew.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gbqedgoer.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gyfsnorqt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgqtvcv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gzpjvrvsq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gwexlfqpj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ghdjhqvrx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gbmkzoqfs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/ghvcrpvtu.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/giutqjuqa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ggseysctb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gmzcqwosu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gpfqxaezh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gfoowejhb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gdvertcyt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gcexhlxtd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gypaaygyx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gmapencpu.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gkightcbr.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gyezocfhf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gsxetjxtm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gircfifuo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gevpqkmre.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmygjhaou.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/ghjpbbcoz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gidbidkof.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gbitnazvb.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gmphqgglx.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gflrpaofn.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gtozynyvp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/ggmzdcrsu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gcwzmqpcw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/giehdcxop.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gmenociic.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gwbbbbwrm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gbunesgxh.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gpjunawrn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gagxwndls.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gqxkwzwiy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/grqqjazif.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gfohcnjvr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/grboffabi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gnjrphnft.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gjbfmttom.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gpniynhck.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gqbjdqxtg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvrqwnb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gdzhlygvg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gnbbdwwfn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gsdazlkxe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gbaznholp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gvczjchtv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gwkprvbyz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gxoykftiu.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gjnhjpejt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/grxprkjqf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gcpmdhbjr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gtqlqcxue.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gksubbthh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gnzqgfjet.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gqdlwgpat.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gndcccuzf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gbbrfgqxu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gqtuyofyy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gqttiuaui.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gbrobcrnh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwtnjsito.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gvhqjoyys.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/guyxndopx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gobgnsonz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gjbwxfbqz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gwqmwxnbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gajfypyew.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gawoyrteb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbybxykja.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gjabrbrvi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gtywinzck.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gvabsdlus.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gkqndluyz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfajmrczx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gbvuhnqra.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjzxsmakd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gzqgzxnww.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/ghqfsdscg.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/giibreabe.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gjbexnmpk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/glrjasyuk.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcmvgiqwz.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gqvadrptt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/givhngjld.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/grfsoplnr.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gqrwpmwwu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gnhadqalp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/ganmwscjg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gduxseeif.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gmtrkafvd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gzypeupaw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/guposezow.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/goqqovdrj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gtszhkbqb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gpqjvyseo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gzlldgtmy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gobkcdxbh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gycvpklan.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gckwcxpzt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gqwsnijla.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gbsdhvtic.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gekxpccrt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gcdpyxrer.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gcxpprcgm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gmskucwsa.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gcpnyzrfm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/guqrujzmj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gkxashjlw.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/glbefzpru.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/godsjnybl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gfbthsyfu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gdieruffg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gbfzncfyb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gploqizba.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gxyjhuuss.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gckrqnpaa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gyuyvpgqh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gxrehtvao.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkfpskb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gqkmsclqb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gzkfhiwjc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gvncmqqkj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gyvjhalvo.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gdqpztyay.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfkureoui.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gtyardabi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gsbrgbvhr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggstjolwl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gykqoccmk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gvsjyrhrg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gqqnbjjhh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkkusapps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gfvgmhmjx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gseqvlbwi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gsobkbwwn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gbvcoyslb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gkmzmsosq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gycubfjet.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gwbalftpz.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpfzktvre.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gbdbzrznl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gblrjkhyg.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/glipghcwb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gclckquay.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gpwjgtxpx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gtqzdiqoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gbqardcaj.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gauwvnhdv.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gtntiiaed.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gkkmjdhjs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnykycim.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gyejdagyp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gokjovhgf.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gsalhjnzs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gmopbddew.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gbwqdawfj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glmhfaijy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpruijrni.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gnkvvdrov.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gpyemzikf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gxglutmnh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gvodhvppa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gueosjsas.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gqndhjaig.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gkqjnkqob.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gdxowqbcl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gkkexghlg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/glwxxmmik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gruimmmci.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gotzayqib.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gbkrakevu.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gwvbwnpxj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gambqmgng.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/garriodut.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gmaskgiax.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ganmhkagi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/guiuiosjr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/glmfrggcy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gkrdykokz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gfjzlovpg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gmkifoydf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gquzaellj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gpagymhyp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghhdcitjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ghhhddnbd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gszpqlkyb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/ghadjjjfl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gnldrnatf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcgauwhnn.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/glmdzlpip.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbjmqyswz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/ghiqvltrq.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gguooltai.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbfizzhxz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gvbmdosht.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gotvhkwji.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/geewhoetz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gpewkxspf.sHtML


<!-- 参考信息 -->