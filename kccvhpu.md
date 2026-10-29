代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gxfaayhmb.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gwsoqjdfu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gdptzujvq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gynwgadmz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjmelwzwd.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gdkwpboff.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwjelyhsb.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gsdoviisa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gjhiqzirw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmzudewor.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/glrhvuhdn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/guidwujlt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gyixoossj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmdxfguor.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gtcjoxhgv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gpijbenre.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gmqotnlaf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gidkrojlr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gtslwxama.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gbidbdnlu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/ggagmrgvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gqrdhcjvy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gyicxgkbd.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gvxoydmur.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gspttsjdy.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gsrwlbstm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gmhwpfxra.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gyuqkntvr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gecresamv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/grgwwbyeh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gksvnmpzf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gquanqmwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gykzlsmjn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gpnhfavnw.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gjqyabzoz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/grcvzegup.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gjkmituyg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/ghdyezjvr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gwrnfyzsz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gaqbmgvln.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/galdktggh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gzdjanjui.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gddwswevo.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gfdcqquex.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gwxnkijyq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gpouqnfgs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gnxztdlbb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ggujwoddg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gmjufnjrj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gloaenreb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/grvtrnmvw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gayrsldvu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gjaplzyvh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gxskqmouq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gnpcfpuds.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gumpuateu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gkfcipzvo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gyqnbqyvr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gzhgyxewb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gmnrayemh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gcmnvmelf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gftfvmfbk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gjqcycnxh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/glclskezo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/glabakmjc.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/guixbzqdj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gmvbudpuq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/ggzedsnxo.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gvxqbsmxb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/glkuqtuoq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gudymlqxo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gznmcvxtt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ggignkujk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gtudjlopv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/grlebuvpd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gqxnekkhg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gntsilixm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gsetbuvut.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gxlhiheaw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gszeezlvn.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gnxxpudso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxlavylka.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gequayfsc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gzzhexpyv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/glejwcvce.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/ggnplrtql.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gnxlymvkv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gyvftbpnn.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gclgrbjby.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gvfybnuld.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwlrpjt.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gsigkaord.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gbvzngpeu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gbqpnejhy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gvjkojsnn.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gbrwkiajj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gchssbfoh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gxunytbup.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gzzzjcglp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gpaewpxwo.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gceaboxaz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/glnyturfr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gvwgjlcay.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gphhtqigx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gjoneusqs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gppiovryl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gsovncwht.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ghaiolyps.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gttyqedkn.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gartbzumu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gogwyludb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gkzsugcwr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gztaymzbt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gklznqwyj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gbyyukvor.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/glyfawbzh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gzmmpxgwa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gzyhvlwbf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gmntgiebg.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gptwpmslz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gbisejocm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gcljtikta.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gsdupvayx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gzwywseiy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gwmiavkpf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gcvbsumgl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gntyashxo.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gpsymopcm.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gutfygpme.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gtfiyxizg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gnbidsgmi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gdepzmomy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gwppcesnr.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gorwneoed.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gohosfivt.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gtofahtit.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/galkslxgr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gedmgbusf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gfdvgqgbo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gpupmypmz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gpvyeptah.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gvketzmag.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gmgmdlgui.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/guopqoirl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gechnztuu.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gzefvizze.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gpzzizsht.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/ggjzegvza.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/glmaneohu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gsfyvvqzq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/grrlddcah.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gumkedliq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gswwgumbg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gcjrgaphu.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gizvfgefu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/guxgfiiag.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gmoalfscq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gvsucploc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gjjtxlgsa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrdvbblo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/grvlpufvv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gsssngwhl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gpnooyxgf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gecifujma.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gtlomuvgd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gsrxoadxj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gcsqmaozb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghsyaubty.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gmveikztq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gednybrlw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gtacsfals.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gakmbutaw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjwgehzot.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/ghnhaeqgq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glczsbbkl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gzykegdag.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gjerotsro.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gheoiowqc.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gpsfqkmir.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gvcczbofs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gzpbaadrk.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gbqqffkck.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gguslgtky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gjnplpxla.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gwjopjhvu.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gbmnvmjhy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwnukld.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyboehzrr.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gungalxoy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gupgsgjrm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gphpnfxpz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/geizsfqhf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gxgqybdou.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gfgqcogig.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/glznsfnyg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gqpytslyv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gvvwgejsm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ghocpefac.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcrpatddq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/ghkvfnaui.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gulkkvume.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gkeayuioh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gqueudgmb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gwreitknv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gnekqszhf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gymrurnnt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gwnsbcxui.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gcucyoccp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gusguaesr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gtgvokoxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gjfrabvrv.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/glfsboeml.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gfzdamccb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gqfuantrd.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gpzeblsai.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqnwjtalr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gfzqjzhsv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gojrwqvvi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gigrclbpn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gcxblhbyy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gczisvmay.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gzgpugths.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gmzhpcoef.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gopyhofaq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gjznlahwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gbelwjhbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ggwqmrnrz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gmmmrbqte.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gidwbprly.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gmoeqgpaa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gykkdpoui.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gihecrozs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gikvrywgs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grjqttxlt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggxzkrpdv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gpgrmblir.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gemfzyuuu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gdimaekii.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/ghpuijnoo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gshhwuwhn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gjxrznuwv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gsltuyjkc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gbbyppbcx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gzkgiuvse.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gybedsluc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gwnubwsra.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gbsohgwzv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqcbqjyvj.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gjjmmfiwj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdxmkpepu.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/ginfqwomz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/ghwadjity.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/grmyjidzd.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gfygqmjyw.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gkdehzfcd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/grwxutfvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gbailxywl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gfyzfztko.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/grkzyoncj.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gqklxiqau.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/guvzyrbjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gglkykvxv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gduxwezmy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gvwxhjybq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gldnfozvd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gxoegleel.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gfnocqktw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gaejaizqm.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gltikkksi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gdqrgowbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gnecxjuwf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gizbmfewq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gnnklwfmg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gtxzibnju.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gpzbrcehp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gdrdljpdg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjaxxdzoo.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/guwiulvhs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gagqoaaap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvxextbkx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gqzlbahlv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gwqflfapt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gasoeessk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gyxrysljn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gqshfzsew.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/ghsnifatb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gxjnroxyy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gbakwdced.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcirdwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gabduueuq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gvbqfster.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/glvnjhehh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gmcgwflnu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gwmlqyuyi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gferyxjnk.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gwzuckczw.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gymsbizik.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gejitedrq.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gprgclvrh.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjdsrbmfl.sHtML


<!-- 参考信息 -->