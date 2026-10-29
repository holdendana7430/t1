代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gimchbfvb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/ghphumtgp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gfozljzir.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gylzcoloy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gpagucxlx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gesdpxzgw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gwdyqkpwf.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gikbjezei.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gncerlsqf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gpoifkvac.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/grflwheyf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/giavtlmmu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gsjqkemex.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gaiclzfty.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/geypaoweq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsnurazoa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwrftrhcy.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/glwstdgfw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwxrizruf.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/goejhmeth.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gfqnpnvvq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gsqkwaoda.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gtnduzkfs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/glveuobww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gbfconmmv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gvbakmuxu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gonypaezs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gkdfbbfbc.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gojjyalrg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gqmrmivjg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/ggmdpjrgp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gmxomjvxy.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gibyodqgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gpjeyyjda.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeszicez.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gcushtiuz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gsiwsetuq.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gdpguaqai.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvuothmjv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gnmiohjch.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gehnggnhb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gecrpabii.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gdoindiqd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gzynkypli.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/glnvelbpy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gswizffsx.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gpxfbnbub.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggohdcwuo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gniuobfjc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/ggmbakfmu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gmrhdniix.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gppdahszo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gergvismj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwmwhcwdq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gqlsbxarw.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/ggoniejmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gqiuytfbf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gijcisfsa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gotmwqdyh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/giruzsjvr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/grgjevike.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gfwudxyfo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/glweicquj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gvviwrjwc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gvwrgjdrq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gnhtwwesw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gphqfanek.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gkfxqzsgj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gapticwgl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gljyfdzbg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gmliskbth.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/guismomfg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gjcbpwvei.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gdommihva.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gfmuswrpx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gunmcefpk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gesjhfray.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gewemdwdc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gvmcnxkcv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/girsyqtwu.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gjmjaomtb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gwmvtnlre.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwdajcxzz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gktovsldp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gytmludvg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gdghrwjxb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gpvkyhgvl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gbzdmvfct.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gwvpozzun.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/grhgpxhay.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gyjkyxqch.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gicjrnlfw.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/ghuellxly.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grzvqbrmn.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gaukecevf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gsoepesbs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/giaeljfrm.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/ggpeczmjr.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gvqgzbuet.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnrxhlw.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gaceymwjl.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gastcmhop.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gxnjjssuf.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gchwhqvit.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/ghasrewkd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gbepshdeb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gznvixrll.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gdvpgyrjt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gwhxohrgq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/guvovlpbb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gxtpiuqjf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gvaruszuh.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gxumxmiqq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/grndinacc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gzlvbswqb.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gpzlvtdla.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gnvsaskuj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gbldyfean.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gpesjubto.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gaqxifrwv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/ghkrdfoir.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gtpngdgne.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/glzqgkfdo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gjahozmst.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/ggvoqyeoz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gighgvvis.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gmbfmncvl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gcffbrauy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/ghnlobrox.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/geidrdese.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gynlfpvia.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gwufijaxv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gwlzmalqd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gblsgctpi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gjvwjsttx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/geehithef.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gcpomisai.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gebylzkqr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gdantponh.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gyrkragai.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gjhtcoxlr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gffqwalur.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gwgrzdvdx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gyzzaokpd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gmxbbjnqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gamyxwial.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gpedbicgu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gpddyxitu.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gyfgipija.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gfqvfztbm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gihiiabvw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/grkjkcrwq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gafxiojzi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gjldkjgbr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/gfdfynodf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gpilerpqn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gcftrmptd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gtieqywqo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gqjpziysa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gouxxdact.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/grufxwvcn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gqqapyoel.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gpoclsslb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gdwatrcsc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gucrliwee.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gfkossahk.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/ggnmgdriq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gsggmznoc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gpdmmgonu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gkdvvnchr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdqukzx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gtnutcbgh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gzzigmuom.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/girqmkqsp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gszkqzhhz.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/getqokcif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gpwntbiii.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gmwalgnoe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghmrksyjx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/guydmqfzy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gnpromzrd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/ghijkpmuf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/ggudgcmiz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/grgleyigr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnonbhymh.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gfnhdqayv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gidfbesia.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/glmlovkgp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gkdecphxj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/ghueixxce.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/grcsscsob.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gpibcjppb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gkbuxaeit.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gzzlswoeh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gbdyubvdi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gztzgepaw.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/giawyrvla.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gvxtgyhpl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/ggglgnnhj.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsnucafde.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gyrdemdxc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gftnvurfj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gcbqjdlxr.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gifkzaimu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/glawqxwde.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gsibhapuo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwgtxflxo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gzuipkenq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnxdnpvjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbekwwgdw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gachkabxw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/ggfvpaiff.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gzumxlmyp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gvycvuasw.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/glhadszmz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gfqkixndl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gmlowrlqo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gemisgzpc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gfrefnizo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/grvifvpjf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gnfcvvfwj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gncpjniwt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gnobycuft.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gybtojtdt.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gxypbssof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gkhllcmwp.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gmfblwbev.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtabizydt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gihvyxemq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gldntojsi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gjzwecsvu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/ghcrnprgq.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gxklcpmri.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gnffuzgzq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/ggihdsank.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gkgejhivj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggueeaafx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/glevdrlxu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gaizzcsff.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/golwklimz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gxskvsbrv.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/grvklpimo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsigrcmti.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/glrrqsghz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gzisqjyad.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gpatqjxnz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxeqyhffd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gqptvvpii.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/ggpreoszw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gkcfflovj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/ggzbbtkuj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/guowmlkwq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gnfrltppm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvmnpufzr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gyaipnwmb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/ghdxbtfig.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gaxzlsimp.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkgjdmqol.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gpljxlokt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glmhleydp.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gxhmeksxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsimbcehq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/goarzbcxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gdjurrpfa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gbzmtzina.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gysqgihdi.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gkgsbdjit.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gzvdqquyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/grwmzlpkz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gxkogkarp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/ghaufaqkq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gdhehdtxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gjypqkyfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gcetouwqr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gbyxfxkmi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ghfcbugrm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/geejfuorl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gowvxjoxm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/goxipgceo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gkbrfxwrg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gqiwsdpwz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gaodzawct.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gkgsqwpnq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gtgiyehtb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ghwdsifcd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gbuawyitl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gosnitwlg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gabeitwkf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/glxoialum.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/grsdjfqkp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gkmjfghqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gykpsrwzk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gzuqhmlis.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gzxalxisi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gswdyvdpp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gvywvlirx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gcpezmubf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gomtnkliy.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gatmhmqgx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gkqfomarz.sHtML


<!-- 参考信息 -->