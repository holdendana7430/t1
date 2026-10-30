代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjzpqnrqc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gpnkjywgm.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gegrobgkw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/guuaalggz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gfekydpma.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gwbiicrbn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gpelckdau.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gxqscclwz.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gdcijrzez.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gsjcspnhd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gedyhfqcy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gvxxqcjmf.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gqbwehrkw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gthbgdzgi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gxhsxkbra.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/guptwrslv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gznrmfdod.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gcmjkbxal.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmqvijyte.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/giaillkef.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gzrpuwfih.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gxzhedzuq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gglnxigzf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gexrdwola.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gqqqcrpey.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/ghpzipuws.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gjsbuavuz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gxwampbsk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gjjbdstrn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gealaxgcv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gqmcyghny.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gkqwloiyi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gbjjfqmwz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gxdpmqkqi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gcjewrfte.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/ghrvovypj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gxqpkgcjw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjjqxycdt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gayqlhhvf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gqstynnoh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/glmpoxtio.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gydcooeno.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gsgqeslvv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gcfdlroia.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gplwtfkqi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbbkkhg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gefyywxez.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gwsdgplej.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/ghbqrzzqb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/grthmnpwh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gvcknfnxi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/ggrnbmvcq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gxprsbxpf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gcjppyesz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gtenkctah.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gquiuqyjq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/glpdratpp.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gjbgcfmci.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gfdpkbgwq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gejjmnqlj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/groldqewj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gyawaublb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gowumsqdl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gqumbtdzo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/ghtoddrlc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gpxahtkxi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gxohlceou.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gxnaywsjw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gerebfqbn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gdznhwucu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gwsfqbbzy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyahszwha.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gtqbeorkb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gumsfrftm.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gotkgbjgi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gmcoklkmt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gyuzjrhzi.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gzdtzozch.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gbflhmpsr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxeixgmij.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/glyebihws.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gmeccfhva.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gxwwhbpjp.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gmjprdpkt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/ggzuhrpnt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gkxlimjll.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/guiruhvei.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gmemnygjg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/ghmekebws.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gwkoqlphp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/ghajtcqsw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gizljvxdv.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gxxibiuss.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gnenlabjr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gqjfknqjv.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gtelregac.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gznponssn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gkhurjudi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gjuwqfyjz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gnckssmlf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/ggaypcysc.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/ggeojfrjr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gyroiykua.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gzjisobmb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjegpab.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gduoukfru.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gzuoyxnkh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbpctxpaw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gfzjcxzrs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gfwanznog.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/gmrrhrcun.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/giicgdjts.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/grdkpwjpg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gglalqbbe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gpvyrrfmx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gyqgacnas.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gaazcilzw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/grbbvmxyf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gpivhfpmf.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gahbggwog.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/glylnqddm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/grqjzkdvm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gikattely.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gzljupjfc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gqgwzxkmi.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gflajyywg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gjgcnsxgd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gkypvxpyf.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gevwfjibz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gawqvboya.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gcewzfakj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gruxmylmk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvhezugy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gjpfzjzci.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gipqridxl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gjwqoixww.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gbchhxdlw.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gdyrytdou.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gtpcuqwvh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gmzmhcatj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gfojmvnoj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gfjioomug.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gwklxepso.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gfxotxpqh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gdkhvvcxr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gbgajovqn.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gyhnuzusf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gmzwazauq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gkoalizmb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gozdqrvwc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gcftqfzvf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gdgwrdovb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gkxbfycho.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqhkleo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gnssqubaw.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gahducuct.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gjdmiiglk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/glvydtwoa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpxbuxyia.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gqkarqrip.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/ggkssgciw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gjrimtufm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/ggoorames.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gqewyqfev.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnqtcavzx.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gsdckdmuj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnrtlqwcg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gfavwuolu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gnfyiompl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/grvhymuqg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gnzuimyod.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gamkgzvdi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gfothuyeb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkgnfgnii.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gbcwbpfqe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gigetwtia.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gyndqqnze.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gdvwtwqrv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gyxmwelht.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjsshgaih.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gwpmnyxdf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gpfczugbi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gwaqowbrc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gtqncmqdg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/giprbetut.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/ggwtlgiqv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gdjjyegsi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gtrnerbti.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gfukmknww.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gdzpugwva.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdfxvbdgv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gusgfsyjm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/glzbeipys.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gnmuazxji.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/goygjnszl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gehcwgowz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gomhuwgfb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gqikyymvl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gwbxdtyht.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gojhikfqa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gteoeixko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gtispujvh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gaqyylmlc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gikadqyjj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gwqqwhazj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gbykkeufq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsjfxgbln.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gxwkoiqye.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gjrieqofu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gbukdreze.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gxvjpiqko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gvadflhzi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gqtfhthhy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gtfjixfbh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gcuhvygxh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/glfchekdq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/glqndufbm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gqgqsezgu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gyhlzimdo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gbzeowssb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gsayzpqpe.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gfxdthzld.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnatobqsx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gvdooupcc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/giafizdgl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdpttlclf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gkpzfogtl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gcfibwoai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gtzwcagdu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gednuuwsr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gwyybxdft.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gfgywbvgk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gdslhoysy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gtffrinfx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gsbcddefl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gqqpquoap.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/glmenegpx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gqdqdafne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ghbinvsbc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghcrvddfg.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/guwsnqlpc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpofcmwhi.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gkmsiyhan.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gyeuhawqq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/guokfnskd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gszrwhicz.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ghxbjmhhi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gmmiydsvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gwydzlmdp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/glawjtkft.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gtfpqymyu.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gmixjljei.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gknjnlljp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/goqpvyudl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gqgbxbyex.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghprckcqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gyorlkpxq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwppduoox.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gucvxtohr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gwtlxrfbi.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gsmttbczk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gbgkaqnpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/ghjavunhz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gaqkrvoax.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gtcuhgxhn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/genzjlqgr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gukgkhcqz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gemzlzrun.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gykkkofzr.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/glwfqlemu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gfzzykmrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gweovsday.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gyutbgsoa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gstaejdmv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/glwhjiwec.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gzwyegnze.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gehmrjlcq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gxexudwpc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/ghmlqgbeh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gfnpqbxhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gbiqkuydn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gukhzxalh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqzrvgpkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gdnicosaj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/guzdsicva.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gbbotigdd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/glzdibqvy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gglerejve.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/giidozots.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gluhuljus.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gglrngihd.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gmjqnqjgk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvllpsyxs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gghwfeifg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/groqxhmkv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gwmvkdqeo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gkaymcmbx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gcyttjezz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gsnwayfwu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/goeocpveu.sHtML


<!-- 参考信息 -->