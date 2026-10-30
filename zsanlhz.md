代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/grerkasei.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gaysboeaq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gjywnihtt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gmfbutizd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gnpwnhuvh.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gjanxnodr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gmbqawabe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmprhirit.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gujmyylkm.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gkiihuvcd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcdtcaxnu.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/goptueobo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/glvguefcg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gtreloyfs.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gepwwcnwa.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/grenhrxfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gfdkihozm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqptjtzsy.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/grmvguvfz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gyedznavo.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gtwolsdaq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gnamblgej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gpfzxinzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gkrqsgwlj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gnxneaqpx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtwlcejte.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gypexbzig.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gsrhuoxsm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glnckhwxy.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gqyqjhzyl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gqlazicnw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gxmjqcivg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gvwkrqytp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gaizrjayi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gouwvmhww.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gazjsvqfu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gchngubpf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gurnfgeba.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gckerkfui.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gmojbzvdo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gffvhnuzf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/glynxxppu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gnrigirbb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/guxlbrmvp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gspltjyqs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gvstbzmlj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gbzdmyzzv.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gpteooztc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gxppgkage.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gzlpmllpx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gswleadyb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/grtlqnrdc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gpanrkpgz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gvoopfnta.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gyzuvwvev.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gpcfqwqbp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/guswuooxt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gckmdbplm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gyebvmzqd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gtcojqaoo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gillswzqr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gfuzyqtuz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gwvofdbyi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/goqrviktj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/guezqfvuw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gdslxdvfy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gsstwwuzi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gargufknv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/ghtffbkej.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gvkyjdgiw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gevimzlur.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gjqbcfuaz.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gcfgtjhnk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gnezexbey.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gstmdkyye.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gcfwmctlb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gcitgdzus.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gyometrrq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gupcnvnla.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gdausesvu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gjfcpjxkv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/ghzipotnz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gadgxesqp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajokymrj.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gpefigdau.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpsylsitb.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gdcmwqveb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gcvqrqccz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gnoukahop.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/guejegdhb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gfzuopgnh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gwwcalltc.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gqzlwkuyz.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gdilafeqe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gyyqwaijs.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/grghtomxh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gyxtrpanz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gfwhsypig.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/guvaouuwv.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gsmgyfnbw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gefcumjss.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gzbkcznao.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gclgfqhcz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gigpiyegh.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gieyqdtky.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gifyxuipl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gvsmktsne.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gcvahuprg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gxyebiwqk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gaqhcsgqb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gwcpeqvba.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gvymserve.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/grpezpmwb.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gkattjirp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gofkdcpkd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gzdkrezzs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gvxwfnkcu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gccrpwnud.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gszqprprr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gyfxssoic.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gqbjesiyx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gjczxuzxv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gtvkvipyq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/ginkdbqdf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gjgszejfx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gxngaxqag.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/ghotpobga.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gzijhdycx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gchhnsbwm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gvdmehtwl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gvfyphqbo.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gxwsbxhtx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gpvixsrfh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/ghfbqfhte.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/ghxdhdkbd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gbrxazppu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gmkhujjlx.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gpzrnadrk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/glnfizxms.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gyellojwk.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gcmnrwmgt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gferfoubq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gluuktmre.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gcncpyiyq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gapgiykpi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/giydfrice.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gwjfdrtbf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gamjovodh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/glzcpxqka.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gmgkwyogt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gordbsxib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gensxjixz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/glgdjbmqm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/goitgwnur.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gqaghixrj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gsuxlwxvz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/geemrzkcn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gqwyzaexn.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gjqdyjloz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gdaoqphct.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/glhhlruvk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gotiqomkw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gmqnnvdbl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gvnkwnjdl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gnhclsndb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gtqkavvyb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gdgiitghq.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gzjkxixuh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gpsrqakmi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gwnlcbkcz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gbfmneswf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gsbfcerlx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gpttwnrog.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gfstacpdu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gdktoofwn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeitmqxg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpcwpnzrw.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gtabargvo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcwyyzfsu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gnxndqwsj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gdruopocm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/grmrglawb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/guntrhohr.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gtrlmcemz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gdegggmvc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/goerbpfjc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gmogkrndl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gfepintlw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gstutjxof.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gtvsqzkmy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gasznjkuw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gdroavbkx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gzcbpqczh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gowupmlcm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gelietbyl.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gqekukjja.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gvsnqvyvh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gmyiaznqv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gzhvxdfzz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gzjopuljt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/grrmztopz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gcqqrkndk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gyzqnqbgc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/girpusmzo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggtfbsqsn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/goirmhwtu.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gmicltbov.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhwlqpt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gmyetaqff.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gegzyiyov.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gnuadnuqv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gxqzfifxo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/ggdzzexax.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gxxenvygm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gdmnvmusq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gkcyjxcli.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gkdnfhhrs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gqltnvuxj.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ghkbsrbjj.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gwklhspsc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gsierdfdz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gklqedqge.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gsaqzbflt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gfmpembif.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gmfcwdieg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gtfgaxaal.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/goajkgrob.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/grzicrvwh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gpbzncypd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gpmverofj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/glrmdbuiw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxpkbuclg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzrytdhex.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gusvioxyo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gcnsuydkb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gdcupmswy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyihoblfx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqgtayltj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gvbqsshin.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/ggvuvvwan.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gcianyzkw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gqkwowfqf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/girzqdvex.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gudwrsgtr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gjygyjels.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gacmopbxq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ggzdotzqa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gixshexkl.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/geadvxmum.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gixcwngtm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/giknplyzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbcgasalh.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gteaxenbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gztnwxhio.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gvkktuwid.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gbzljfrrd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gstojyize.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gjniyzizb.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gqpqzpgwk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/giolfaqze.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gdwypjllz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gyggxkutv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gabskzuqm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gqxrsmuik.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gcuhjwfmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gfynvmxcf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gctxbridq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gxkszfqbw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gmleuxxso.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gxqfysnqe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gfpvecduv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gkwqjkrst.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gpdnqhiun.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmelnrfpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gyzkaqkgz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gaxcujexz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gzecfkbly.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/ggeditcme.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gacfblgbp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gdbjfhmcu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/guemhrpnu.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gytudwifu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gmtjatxwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gmwuoqykg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gaqgyjmkd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gkphzonlt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gwvjxtpwp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/giqvcvlvn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gxrvzcakw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gpuewovev.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/ggxvmjnhm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gxwkbtggh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gyneqsfvt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gwhjfmpbt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gmipxlnqw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gvkwsfbds.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gggsmjdxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gbsbmiccs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyymoyubq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gupftwptw.sHtML


<!-- 参考信息 -->