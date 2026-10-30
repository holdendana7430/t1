代发 wailian999

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghktxkxrx.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbhtsgi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgmkjfk.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaqqmwyn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrzxcuz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxgcgty.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcyxbnwm.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbhefrwvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrbxqrvy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatuumgko.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexdjcgcm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gqeysrxlj.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibbkuacy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrmlrpx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gnhriskrb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gsqgnkysa.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gpsrzqtkt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/grwcmzusm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaxkqezv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggadqnufb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxkklsno.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/graltzgpu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcmocekf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqjszag.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfwbocuy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/glcoawasp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcrobvdm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gzudmnebh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxjnwggs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gauyubljs.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrlquzzv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvpuqxpa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzotdtns.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuurvlri.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmegrizc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyuwfttu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gtirckopy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfltdwoi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaabqkif.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmyzfgdd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmxaogol.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytgmruzf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpzmdali.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gatsfdhxx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gahnzvtxm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmqppcm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxtljrrc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlphbxcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gfhcgowbk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gtivbwsjz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/goagupnsa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gvloatcsc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gzunqirfr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gpgyedadi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhpwolpm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/gncepswrp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedfiuov.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmivmbluv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjuorkcl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctpfnogp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmldiiqn.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gendcjnhc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gnlrjzmpc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gexwyjjui.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswrueluj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnknexph.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhutsnrm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqzytsty.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlvuqwyo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gfohuksmr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyicjujr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gwkifljfw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtxkijmc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfeatybv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqpguizy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gljicqtsg.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqdtlkjen.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzgetybq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkarwfzec.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gpmzfolaf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbkncvyf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/goclancvo.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gcslsrynl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/goxdmcdyy.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqrocyfg.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzujvsew.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/gvhrgumzq.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvkogquq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqqwjxtb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gvwfjrlls.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacxatccy.sHtML

TS:   d.toISOString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpukxnbvn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjecbfzg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/gseqetnzz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpujkjh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/gixvbucmu.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/glevypimd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fanxiaobao.xyz/Article/details/gnfqbmsao.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gnewpskyc.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gfukqhmvg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybhubte.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhvwucoo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gktkzwijs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/grytuhasb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgtoydyd.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpqhelm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepbhvulh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gttmjpvly.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpmbljo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbazpqgrf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaflnilf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmyfdyom.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gbnxrkjhv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvrtsxa.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gowqfizhw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdestwitn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmfrabau.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtjyazrl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/grxaerotx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gulfpxusm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaldxshf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fanxiaobao.xyz/Article/details/gfuqcydoy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhuapbpo.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnimrskux.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gfroiywxn.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvsewdmk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/grtomefpm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gwbzzykvu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gblnzrvyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gplhdwwzo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbjmxhwi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzyqwnep.sHtML

[J07] 比较两个日期
来源：http://baike.fanxiaobao.xyz/Article/details/gymkpsvij.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/ghvotnzox.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdzeenwz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/grsisftuf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkfetaoe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtayvnzym.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtuatkah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gxgtbqzcq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gspiatzax.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gakyybucp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fanxiaobao.xyz/Article/details/gknrziabi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gaspmkquj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtsbseip.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxhunjc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyxfcvgi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gxlaucsnx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gouzngeax.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/guujowoob.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfksmzkxp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gztcqfzwj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gaimxotir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwopmaac.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlftxpha.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fanxiaobao.xyz/Article/details/gywyfhnul.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gmqkuxcfp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqwmhylo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gcwrykqpn.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsqoosym.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfclybjht.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gelkvzztf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqanchscf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/giastgmxq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxspeeuok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/guyrgnsov.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gkwjemzgl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvadtcmji.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvuwsjzp.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gsnlomlzm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghotwromo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/greacgdqy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrvhczal.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjalizbpj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gizlqqdte.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfeftjgx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/gvsjdxpev.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqahciet.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/glpqpdpxp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqqsrfl.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoekarjp.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/giunaloik.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gztstacwt.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkycicimm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvglyaa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyogczir.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/goczyfdyj.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpyenpkq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gumthqxzs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjispyt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqljfncw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gcdamunff.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmkiujeu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhvxcuh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmdqsph.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/glxktkxhv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjykzwejm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkniexdnt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvndshmcb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfuoyvoo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/gnfpfctgq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfzbpgh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjoloiqs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwosdnhj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gebxcddzi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gitgkudpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcpbsdnf.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtsruqhi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylnvwcev.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnjsscof.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grszijtdw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbvcgjxz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gjgupqvef.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fanxiaobao.xyz/Article/details/gprstmaoh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrgkpwbz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fanxiaobao.xyz/Article/details/gvbkbehxs.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkqzpreq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gitmjykjy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/genagiopa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/grmwulhkc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaemvimbk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gcmulhxae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbopbmaps.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gqudtffjx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gsvbapqoe.sHtML

[K07] 进制转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsqzpmmic.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrcpojhs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gibdmaxqj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpijduduq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsahdhtx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gfzizvowr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gijcezphs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gaashgspj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gzwbnwigo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlujgnvv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfwjqhic.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gowakyodw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyrnarwd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkioocf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijssxvkv.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzodwiip.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grljytvja.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gcpaowadw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gftuihije.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gghgzhrjb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnfkvmvs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggddyqjtc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrnbhztc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkawnphp.sHtML

JS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gaoazxdbk.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonofytzk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpgidbef.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gossvhqxv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsbzqonw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/guefdsjtz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdefkptds.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gqnnvdohq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgdnbqrs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkggbhvpt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdyshcel.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxftpbyz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gprhoucaf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknwxzuer.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosogutnq.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gbyloqvbn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gimuckrmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gppsqiyfi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gjttlrbxw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gclanqmgx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqajvwds.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzedgghcu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/glzupevrs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxrlfbln.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gtovsbvor.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwgszsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoabrpwb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzgsexzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gzaonowhy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbslante.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fanxiaobao.xyz/Article/details/gdsybcuvg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fanxiaobao.xyz/Article/details/gyrolxzcg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhgvvkak.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhoemjqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoevaell.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzfckdsoq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gallpukmh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gkutygacw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gkpboddnv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmuygfsdd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/guhufnsbj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gccunbebi.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmijkokmr.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjitntg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gafpsrvnx.sHtML

JS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gkqsdrfdy.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gomrdizkq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfhnnnio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/gxlljyjtw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldbxczom.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gvqgkqcnp.sHtML


<!-- 参考信息 -->