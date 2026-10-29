代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gbmjrnnoy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/ghsrwmcxz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grgveiixs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gdzfuzolk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gbkklhiaf.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gddkjxkko.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gbbxyiaal.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gadjanbpm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqnagzazb.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gqbumrsma.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjewktvat.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gxgvlcatj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gpltjufsk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gsuzhnlwz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gdgecgbqf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gxvfmsnwj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gpjnokquh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gtndpyhsu.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gkitrqmrb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/grggrkiwd.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gwwvsguzq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/goolnvopq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gfxcrsijm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/glvpoijdk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gggvpsgee.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gfbyixnau.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gjerhecti.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gagydstjf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjlgzlnuu.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gvvvwtqis.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gyotukvno.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gqocjhzjq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gptwxwcqm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gjaxkrnmh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gdmrdxqkj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gieqpspwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gysiadxuj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gdpivmbpr.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gsumoanok.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/grdbnufqv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gyncltnfq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gfjkavwdg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gwcihxubx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gftbfcrtd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gbzhhicji.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrbbltzt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gbvwwyvcd.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gbclmosjf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/glnmkcjol.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gswjgoeot.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gncmclnoo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gjxcbxgjh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gdgsxyocf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gnhazkicy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzyydyryb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gvzzswzvg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/guxbxldvx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gmodnxatw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gaadairnn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gmdscoplf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gsiliqavm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gzueermqk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gkasgryrb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gbichbhqm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtmiezu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gwjpctnjp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gcguzctdr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gblufidra.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gwyrcrhkc.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gyoipqhev.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gmplcdzna.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gpoppawxl.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gbqujlpcv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/glbdlhlko.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/grfuqwhvh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/ggfirawmk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gvigpwfxu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/ghfplhwxv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbxrqjobb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gfpskunjt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gyyatbtnt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gxpqsjkxn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gvpqonpwz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsbjdcoyq.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/glxoarokj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grqommcvs.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gnypmjcty.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gvkfaoxeg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gvtjlzujq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gteefoull.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gdzagorva.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gtasqblwj.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/glkwlgyue.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gnubelaej.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/goucywyro.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gfdvkswuq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gaypfmiax.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/giqtnarqd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gqwoyugbt.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gfcrobomp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gkoyyizmr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gvxrfohqs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/ggttihplc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/guvphfewu.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gigewifxv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gviomcpbb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gradhitop.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gcpbphssf.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gztelzktf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpudjsvu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gvxormeva.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnlxllf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/ghdhixwfr.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gwqtuhgnm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gqhwmdwah.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gpddidlba.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gbhdzjfpd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gmbyergkq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/ghorvwxfl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gqciqrdlz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gjwihxhra.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gjrnpoqrc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gslgmwxrt.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/grfsddqxx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/geyhfhiom.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gouwejenk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gtnbtukxi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gmayjrzed.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gpfxrmizo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gzerjmkwg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gaxgvdjtr.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdmmzsa.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gwuugrljw.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gwcbaztwy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gclrfmgfh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gsafabkho.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gsqqwcqwu.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gpsfhjdtq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gnytqkayi.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gqduhcwfk.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gcdmwecsz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gurrehhlm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gbtgxkxvt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gswxsdirc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gtfjwvzvh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gxbuulfek.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gxisunkbq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gaoaghubt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gcvjixzbn.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gbqvvaane.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gxtvulvbr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gineuegej.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gdqhzpgep.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gbyqeemim.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/glzerpplm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/guqgstaaz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/glbtrnwnb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gocxthbbs.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gqojlafdh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gxbnouipb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gbkbdvmkq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gugssnatk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gfrrqryzk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gdjnvxqgj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gwwdrjnns.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gehzsppim.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gfrzugcgh.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gawefdbxx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/glfvwouye.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gwbfvcsaj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gapmcfeax.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gbrhvwgab.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gpbgamngz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gfjapmdfb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gijxuagyg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/ggeukmsdu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzpdpbqr.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gbgxccldo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwvtgrcw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbxxklmug.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gyknjulgx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/ghjmxjxfh.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gqiktvvkg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gvdvkiksh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gquiemlxf.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gvyjkjdmk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gossymnup.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gzyzpsziz.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gepkbwhqx.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpclffscl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gtehzgufk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtgwqpchr.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gteqwagiq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gqyexazcy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/grqxglubf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gacyqigjn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/ggbliraps.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/glwizkqky.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gtojuxqmf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gzytclrgn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gjnwhidmu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gznrrvawx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gaagldjtj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gwupppkwy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gpemcqzxd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/ggodprhzb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/ginpjecxb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/ghcxcelua.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gxpszppxi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gximagkmh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gppbrbngm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gxacmfmgd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gjwubnnvp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gbksobyce.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gvfkfzkrl.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gyxzfonzp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmtgwbarv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gzxssvfmt.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdfntszoy.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/guonyltfj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gznzdcnwp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gflofhmdx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gkkzxyhmg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gxifrdezb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ghpxpnzqs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gredhyffu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gsqjisonf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gsxzxapee.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gtcedfina.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gmsgjerly.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbbxifqlj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gylqussdp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gcfzakrdq.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gqfbiwcue.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gsjmhvqhp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gxbfyvjtq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxzrduaok.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gohepxbnk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gptficrwe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gizputvvi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/guzpaqisa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghqmscyds.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gywofapav.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxonqnmpc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/ggieafild.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gijxoliek.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gzcvmezhc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/ggzfkgjrn.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gfbtpxyce.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gbbeoxela.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gqhgekpsg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geyhvvqmy.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghpkiujdo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyheqivsw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gmjbmyhfq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gawsjgbvc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gkheurcks.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gmjketcef.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ghvkzdpai.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gdeyreddo.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/ghikqvrzt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gshyxqwuv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gadqnndpy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gjodklnmt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gphjevdwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gylfuerur.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/glyaigkqo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/ggngqkwla.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gzlnckwze.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/glynojkgv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gixofdixz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gejwchomb.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/godbmozjy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gbvtowntu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gclhyorsr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gebovfjcu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gdiaiuzfs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gkbsdefqh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gxywgkuer.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gdjrnanci.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/grlzroddi.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gigkmyrai.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gcdkhcwwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ggwtzbrry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gysahnhwg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gddmcelzf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gvtedpdlx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gkxenepqi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gjsfgogsl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gdtadxlyn.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gsmzoyuwp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/glwayhgcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gfjvlfstr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gyawcyjfd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/ghpjhdqzs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/ggzclnqzc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gmbkguqsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gjnyasfko.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glomgnvjj.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gyowxxild.sHtML


<!-- 参考信息 -->