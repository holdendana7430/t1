代发 wailian999

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqewlsln.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpealeksc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gebcnpibd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gibkxjzwo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdvjqgzq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gevcrsatf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqktexmcd.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gitvjvqee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbxpwzmtm.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/guktkqbse.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohaxqjvt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqthxiys.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwzjpzmw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgblodiy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbaxwrdm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gegvkhzoq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfdcfhko.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gahcukqgg.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrglcqat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcwhjiy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/glwnymrcm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvkpypp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjgzkptu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gkleroufy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gyvznafik.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdekonfai.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdimuxzyp.sHtML

[I05] 按正则拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gdqspbyuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvomqdxst.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhttbhgr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqdlygu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzgzujtj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gwcjmqdqc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsapyutzb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgdvuavd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxngeeaj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghggoaacl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzftfiwu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxyykydr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmzcqcyz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gvadmnlsa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gnlmexsrg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtfhiayr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhczrxgq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylxlolu.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpqpvynu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpusnez.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/grwamprdn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/gedralhhl.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/ggsoxtyfu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvdsomks.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfecwycl.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkctadq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvypzib.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grltigqhq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/gawgricfp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjytvnx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/ghetwbygh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnfkmgc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gqhicorlt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqgnzpta.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmqpnkzd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdntynenm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyofiicn.sHtML

J. 日期与时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuogdnhj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhawjtvp.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gsnmrhqck.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnynqmpwb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/geanqoafs.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkelqfmqg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gupohubii.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gythkylss.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gufiliilq.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/gizvuvmyz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/gswifxehb.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/guuqgkqom.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrpbbxce.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvrmzktq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gcaqzgtxu.sHtML

TS:   d.toISOString()
来源：http://3g.fanxiaobao.xyz/Article/details/gfrazapux.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gbpdkbadb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvlqbzob.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gunufbzud.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fanxiaobao.xyz/Article/details/gwwztwrco.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gooahviks.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnugllgvf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fanxiaobao.xyz/Article/details/grikvwcrx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsbmtqqf.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcsbqsds.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphqhizo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvypfyol.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gqwtuswoi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/gaczkersx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gwasbithe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/giancbrff.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gzcbfdfde.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gdhjuecei.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjkmddcm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimuxpvn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/guanvuygf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gibyxhprd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gampaunhu.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwslbeiq.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjitqqoqo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflkezups.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgehtwiw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqetqhgj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqzhrrsb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fanxiaobao.xyz/Article/details/goxrxklmc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gsmsjurdz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcskvrswp.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gxbgxriwz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszzmvsl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnvfjgmy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfragcyuy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fanxiaobao.xyz/Article/details/gfckmoxxm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/ghdsaiezj.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fanxiaobao.xyz/Article/details/gpuwamsgj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gnvgdbqeu.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/girayesuc.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/geigpijrw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzxzoskk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fanxiaobao.xyz/Article/details/gerditeev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/giwurvned.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmmjlrhi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymsmriln.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqqhsun.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlzxtdys.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnehdubf.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbhlvpyl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjytakcoy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgbeilri.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkkqlzce.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fanxiaobao.xyz/Article/details/glvpizkww.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fanxiaobao.xyz/Article/details/gbzbalxdl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/gdmyqrytg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gvltgsvkb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmntiqpn.sHtML

[J09] 时区处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghrwypcvs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/grgjhshzy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzeifivg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrgwhrlm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsudxvio.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gexsentgj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpepccss.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gonalifwi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/glavxtwfq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/glfyrliab.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/grozywdqb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggacyulgy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlunnvrm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvbzxxub.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdkmfjga.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/giwciulqj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/guyxkiefj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznudbth.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gupbhhgmr.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanedmgf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpexzep.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihyeaym.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gvchbqvon.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gyctkamty.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxrxkzrn.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjntyiqnn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkjinzbn.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbtdxmjnx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gveuqscdo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giazanqhv.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwsxmgf.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzffbbxi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxleevo.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwexmvvtd.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeboqyfu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrkfmnr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwbklxs.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmolbmne.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlstvxbn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsugvtxh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaunolrs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkodcguxn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugfwkvbd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevkbmqny.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxmhjend.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/glqgbciam.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzsdgxar.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fanxiaobao.xyz/Article/details/gyhsujdfe.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsafgwzs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gymwqrrfe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkkbjrim.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgrleyws.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvvitcsx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gufjndvbg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotkdbwng.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggommagqf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxnfteb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/givcjtrzs.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/giafgqdgp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gswkawtzf.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gclpwlqkx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvcdzkvv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbttcpqw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzgjoasq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/guzancxdz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlbbcgb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fanxiaobao.xyz/Article/details/giqbvorwz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gohncfoyx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxcattlmg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gclzbnjxj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzprpnon.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gmndwoahs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gsvlcdzbs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqyupxmr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjqwyabj.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gflnmuvse.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibdiclal.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gulfxvanx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gqywsgdwa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxflgygk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcsaborh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmiegfe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gclgovyrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grocafeee.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgxhighp.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gavuzfjuc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyjodygf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgrzviiv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbippvn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbjzndzo.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhrvupg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuebfohu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkezitxf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmxnzmnfa.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyktiizh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvlwxmiey.sHtML

[L01] 发送 GET 请求
来源：http://wap.fanxiaobao.xyz/Article/details/ggfhexlyr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/goeipxfkp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiuazlb.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gqpvnpeyy.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grktphozf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpurbazxn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwlxhfhe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/gkqeytauh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkpqqcsq.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpqopjfdw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gychgvxza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbtquox.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gwzljlodr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gabqmymlp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnkvwwnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gojejnmoa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpwcdxgh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gbwqkkhzb.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gcjefjslr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fanxiaobao.xyz/Article/details/gdnlheqtf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexspkqzh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/ghogairvq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gffljgzro.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gqganttdj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkapxtgjy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gfdrokszp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gvnqshsqe.sHtML

[L04] 设置超时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbndhomw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/gqktrordz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gacwfngad.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gsphedwca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqaejow.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/glxgzfszo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwhadmfq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprxjrztd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/grrggfnef.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/gexpmhkoh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqomzuro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gucjbsmzv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntxjnyrb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gjsfwohol.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcvpjzkm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaehlzrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqynogzov.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqggjynn.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gaektlcdt.sHtML

Py:   resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gxaxxexwv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdyndvmj.sHtML

JS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/goblwhwnt.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/ginpzfepp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gdirmdohx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemduhzo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxjledx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxydszpi.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmvyajoj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbmrjlqi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gatsspfem.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gabldaqjw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeyjyuos.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/goatuztoy.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gszlojduc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/ginqsxofe.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/ggvheloci.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjtnwpvo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqaplyjw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuyankef.sHtML


<!-- 参考信息 -->