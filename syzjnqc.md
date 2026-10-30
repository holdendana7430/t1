代发 wailian999

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gfzgzvzns.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gxwhiztsp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gmszxtvvj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gcaonywsj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gvsxqiewp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gchgeoplc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gdxcdkwnu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gwonbslry.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxahlctdz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/guthkemes.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gbfgitncn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gwzovksza.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gmswegzjq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/guqymgqny.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gtprtldsk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gdgtazuso.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gkkmwwoxj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gtmhwtvfu.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gflfwpzbt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gybdsuuox.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gqfujdewb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gxerrxfdf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gqhjzlfwv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdsiomhww.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/grjtnprqp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gynihpjpk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gkstteguh.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gqsoocget.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/guxofqayj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjwnybuue.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gtmzjxsvx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gmlilomcj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gldriwxjs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/goirqxryl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gzgpksdua.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gzwkrmcoo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gtscuppjm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gurrsnccp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gulqnmgnp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gjmrexmyf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gtcaaijor.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gapcmunkh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gzlytvrzr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/grjyzuemu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gaucuozrp.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gtefvouko.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gpdjbmrsj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gtbwjpecq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gejsbggqn.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/galrptqdu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gnizkrslp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gtblncobk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gwsnwsrwx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/greqisnbc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/giuguiyza.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gewkhggxm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gxtljlbvf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gskyqfpho.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gcugcfyzq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/goaulngkh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gijkfxlzt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/glxjyhxbf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gtusajrsz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyaljfnxn.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gxaahimls.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzwavggys.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gocpvjoda.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gdkbubqge.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gbnshjvdl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gjizvxsly.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/giygxpplu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gwawbsqer.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gsjmyrmhe.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gzplnuumm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/ghdkzewet.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gwwdwrrnw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gtuafzwzc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gowddljzh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gbgkfljaa.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/grpftntod.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gdimgnbpx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/ggxxajkbv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/giyiwesxc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gvanqrtns.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gaodvetlk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gwrwkxpux.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gbvdjqcnr.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gefkkwxjd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjlcpktt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gaowcendc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gvzvzvqwx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/ggmewrmuq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gwthpdpev.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gzywosdzz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gsmymojja.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gffyaumft.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gpcbdbagy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gomkrpdrq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/girkexkhr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gbrpubylo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gqtdkcbqc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gncpvvqdz.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gywrblzja.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gcbpdlbkw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gvegewvpd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gysmhttrn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gvzzdbfwf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gfbpqckcj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/guqyutgkh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gfbnusxrt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gshmogxog.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gbidjekun.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gzcdqhvtw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gyfhzsocu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gqvbxhkjb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gsnimdfbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gswyxcmkh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gyjmakbqa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gbgrkxgcf.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/glpqpzkwu.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gydmvrrvc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gyerwgpqq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gpvugifna.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gvztnzjcl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gyslfyqyv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gjkoitrxf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqplixg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/glequvkvc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gtlhodcsc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gpqanqgai.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gbztfkitm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gpmixcrob.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gmxcxrrlh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gunxqeyec.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/givwpoklg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gbjsrsryq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/ghcdcyqli.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gepvgcwxb.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gawgebmye.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/giuitafnb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/ghelyyxio.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gmzqhfoux.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gxxlkepzt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gimpglwka.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gogzdiuya.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/grmglhasn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gfugjpvgo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gaylacyca.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gkttgumtp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gufbhvfsk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gsqjowstd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkcukzibh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gzvrdaozs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gmfdtqwsn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/giwfcwhli.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gilbobccj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnuspxrh.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gsqyiqccw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvoothltf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gixovtxuk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gnvfikcoy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gyhwqldwc.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gasjtpqow.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gxiimxhlo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gqcjlrbzc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grqreeyvn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gpimckaft.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gatazpxux.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gyhbbngps.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gtxmxoont.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gppercakx.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtffumoeo.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gnuidzojh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gtomdmvgb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gejxhprhx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gviclamxc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/grxnjpdwx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/getpodolu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/groeqxosp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gxznorapi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gdghpbcpd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmpuyslaz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaaaqxde.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gsfcsvkgl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaaowytro.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gspfgwwcc.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gqgodqxtr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gxjoihcqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gzrluwvyt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/guleigruz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gfiqhpagl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gqacfvgxs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gktohdesu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gxpgykzut.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/ggarecizh.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gcizwipzh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gupfnwgjz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gqacsyyfo.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gevcwjngt.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gozbazvqy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gkwomazjr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gzhchylmb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gthsdxeda.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/ggewiooal.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/ggddedlxg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/ghowmgfqi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gsebevtcy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gllncmfzo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gspigwpcw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gaxgzghzx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gaucgtgfd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gygsrqluw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggevgwbns.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gizmkyubt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnmjtnvcs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gzmkdmutz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxpuzceed.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/geompodjf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnuqokgsj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/giidvyuvc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gyhzznwbv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gweqhmnpa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gwuscwtna.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gfctsiksu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gbgroxpcz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/glwyjdoqn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gjehyltqj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gislodcne.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gwdfayljl.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/golnlobod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gwjgqodjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gybwwwgig.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gypqsdbgw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdxgedvbu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/giuljsold.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/ghctppxtf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/ganoedlpl.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gdvtbvegu.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gwowbpnnh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gthgjmisy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gcyptcjou.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gyacbpveg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gxmrfzdqu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ggqdjkfna.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gemxznhsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gtxvjvomy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gulmoabkv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gagooxbdj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gjvtndqho.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gejiifiwj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gunlcbqxf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/ghiemcbwg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gbhkfvovg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gthclvvru.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gnflauvfd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gxbyrmelf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gxgozngqm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gihbvcwlz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gxgbuftno.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/grfuhfkzb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gghfschve.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gtxyemoho.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gcvysjuqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gtssizhvj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gwtjezoby.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gyeywhajr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gwtlntywf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gnasrouhn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gxpavyljg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/goeopzfnz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gqnsqxrch.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gmrcyzgdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gtrqmyaxs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gbyturzgm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gzulhuyta.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gkmljqfma.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/grnqjqgbn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gegliepsi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsnlcwivd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gcvwzcnoe.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gjqsexuku.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gnaqojsoj.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/ggozjslkk.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/giikxnwxn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/guisdzytq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gpbqtgxou.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gssltqwrj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/glmafysam.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ggcqwpniq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gnoqorskp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gjljzygxc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/ggzeemhxh.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/ghhwscuvh.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/ghhqncxar.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/glbeibyic.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gjkmatlih.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gczefyatr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/ghtlisgse.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gpvylvyxv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gyqkoassf.sHtML


<!-- 参考信息 -->