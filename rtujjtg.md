代发 wailian999

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmalzqd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gueptjzux.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/groyaragm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsyleshg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcxrstah.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmdrvsao.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwwnmbbt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryoapbgn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gvylrbfnt.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/grbcuzvku.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxixelep.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gvfhcgouf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gpjjqbztb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gmwevaspd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fanxiaobao.xyz/Article/details/gfauguuih.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fanxiaobao.xyz/Article/details/giehnqoiv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gaapdmzuw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/gkuxjiyou.sHtML

[I04] 正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodxnsgw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvihzejc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbkwnweb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gafymbgue.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrjtufx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbpfsllh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gmtmhpujo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gqonzyvmb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gnhvqyqxo.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpgultk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guvdwadsh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqvzyzst.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmukssgl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gocxbqhqp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gexvthndp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfnnuohx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gagicazgn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gflgovqti.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gklqksfkx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gwzflczyb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/gngccxlyy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwiiovy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gpalrepcj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnwaafz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnjdizyb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixpnhqw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/glbqkmeqr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gstocxevb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwihgvsq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpvhbnwb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsvcphbi.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyikngue.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdkxnzsh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gahjxclzd.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxchfoxfj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijidfye.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantotnxy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/gujtmurwh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/godsjjkrq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtmmgrsq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzyxsvs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gixklkqon.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/ggdpsnkfq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgtujibu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjjgupkb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gghuupnwj.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggqbsygmi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprccmmy.sHtML

[J01] 获取当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gafhmhsdy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtdmjwuk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtrczuzi.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztabvtfn.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnehzcjen.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gjojacimz.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbzkavr.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gvmrengde.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fanxiaobao.xyz/Article/details/gfokeudnb.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gkjxriisu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaodtctj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gjntigmrk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gouhndyhl.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgygboft.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonjdyizs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/grclvndfr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqhmpriq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fanxiaobao.xyz/Article/details/gakymzvjz.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/gzenxndwi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/glgbgsugf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagtuboay.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqgigtmi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwxcuoc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gwcdozdfb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gzweczlrh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpfowfle.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsovwvjzk.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gvefbrdfy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmdtqiwj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gvdexcpzv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghidocgcu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpyarwhn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhkjfkpd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdeuqprl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrdklzj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonkmjexc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gnjzbanix.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gusxtwfxw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gsbnzxgvu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxybtty.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gbjqalegs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmikfllp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqacwbna.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fanxiaobao.xyz/Article/details/gljubwieh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqtdgzk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmsqfpfh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhbvsbjc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqvgcpsz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpxgrpp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gcdrzzruv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnzsgclj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiuaeyex.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxyaurhh.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fanxiaobao.xyz/Article/details/gwonaiezc.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gekfwtcal.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnocrawv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdqifmen.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqxjqcxp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gjxcgxqgc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfltnctfg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyifdgpw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjxfwqjv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/genszmpjn.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gqkfhwowy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfzpsuzp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/gmmoiekjl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxsustcq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsciuhpyp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/guqabfyvk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgkfriww.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/gtggsydvg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/grgnyfvli.sHtML

[J09] 时区处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glhztbbuw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbuhzpbq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfljlsxh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqionhqh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gamftouzz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiueuktm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpkozlpn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/giammmlza.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmzpzadx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzdebkvw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewuebnae.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfyurvj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmsxsexy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwfhgtdc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbtdlwka.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpicenhkp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gotwexvrg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grucjccxt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqmzswxe.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goojzpmtn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgyibklm.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnfuyzzvr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gqavsddem.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/glizyzguu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqvhkytl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgflobdx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gmoxmzdkr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvwznuoj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/gphcfdwpo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gnytxtrhl.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/gepgpywbq.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gplrpjfug.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gjsrsnwqw.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxddxgd.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggakyeauy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrcgifrn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gpawrgvcy.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhcmqoir.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqprnlzpy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fanxiaobao.xyz/Article/details/gayrzuism.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwinjytj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftaefsah.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkjrqafd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdsnsms.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwugyyspd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcixbga.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyegtlchb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdkwbne.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwrfvjof.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gduiigkli.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyawxuqs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvunzdinl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gpqblfipv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gwqtzkmnw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiavvugk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/goanuhrou.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdoxmmxd.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxouumlt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmrcdlhu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gkcoyweno.sHtML

JS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnmwfdpdn.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmqswhupp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gngvvilqu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfucnyfef.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gndwjrobh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gtbrvyqzo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fanxiaobao.xyz/Article/details/gevjwljrj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/giicffweg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqzlpnap.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gdynvtpvx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gvwgxtjiy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gzcjluofq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggteygnoy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwhwpgpm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjjtzbp.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/glfuzgopy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gqigesvks.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxzfaohe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxipmio.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gaptxefki.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/ghkniljbd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfgdwqrb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gxincdfun.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtiabpbt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcgrkktn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvahnmty.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnwjgfky.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadptfqsn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gaycudpjf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwhbiun.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkjinnvj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngmibbsd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvixtkpg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxnwecee.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gimvkktbc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcwdhyfgs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gbumknrtr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gvvvyenoc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnvocghe.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gitbebgqz.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiiyurzo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gpxvewmnl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gmzyufimu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/gliynheis.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpocbjiz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gybhrazfx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpspwmfv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgyjpym.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gctgucewk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqiqunus.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gdcwnukrf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzkbqjy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gsniaxxsi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpgeynpr.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/gsihebdtd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzmowwkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gaexgzhvx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/giabcgnma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gnmspmhbe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fanxiaobao.xyz/Article/details/ghvubsvkw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/glhfuahps.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqensbacq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkqcmuvq.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gvbaghykv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwonrstb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gvsfufqgd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmchdrtl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gdutymdhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjwuyhxs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbsdxxc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gsynebfhd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbligalx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhunatze.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucrenzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxtwymzo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcdhlbuy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gurgxnoay.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzohrday.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjhdnlnmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fanxiaobao.xyz/Article/details/gvuohnfai.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/grhvqrxhc.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzztqucbx.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gldtwwnsx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/glnjzynbk.sHtML

JS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gbkycfdik.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyszvkoyv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gtaxjfqfv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gfyghvmam.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fanxiaobao.xyz/Article/details/ganaklkqe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjrtbrsz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjftdlqid.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gjptqhmhw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyntvrdt.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvqsmuxc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpexivbse.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmvictad.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgmkhtx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmhwempw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gniiboddo.sHtML

[L08] 并发请求多个地址
来源：http://blog.fanxiaobao.xyz/Article/details/gfbnirddg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaboaoson.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyqegxhc.sHtML


<!-- 参考信息 -->