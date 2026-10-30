代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/ghzptspqa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gbwfhxyop.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gtwtgdcuv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gnoxgbudj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gnvkjmpcn.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gujhmkjei.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/glcddtahk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gixjfmfhi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpblzvxyr.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gjvrmzotj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glrmmwbav.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gpiwyfvei.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gprvnonuh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbmchzxkm.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gjrqpaxxz.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gjlbmxbpy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gpxnvowrp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/ggvutsado.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxwwcnneh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gibkrgqjg.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gckfvtzji.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gpaqcgelp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gmzfrvpgh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gmcrxxtxn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjhvbls.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gfjaltwyb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gkneswcgr.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gzgwzxczh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/goczmmnro.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gvesrtkxk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gaewqzhzk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gvugrvsdp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gqwmofjtc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gxasniadr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gagvscusw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gujwnhhwb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/ghgnkgagv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/givgexwtx.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/ggliutjuk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/ghhlwsbsy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gctlcptvn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gjcksclxg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gmarfnrdg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gvcjyajlc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gvqadekdt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gdfjvjspo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/guuobxevc.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gkfjkwtvb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gxctvueml.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gkiyeliss.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gikjuhybw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gvpqepsuj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gmvnwwojf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gqrlstyfp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gkawdsyew.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gguezvoxk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/ghtpcadls.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gsqqdyawq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/grkxivlbs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gkwcgkiil.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gvbhrgkwj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/ghfeljhcm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gbeiqtfbc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gqhftsyhp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gdxvmrqzh.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gudolzplm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/grvamuaaj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gxnfnohnm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/giqwdcadp.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/guckwrqbg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gkyedjcju.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gwgcfimoo.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gpntmlmbc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gxnelgcsb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gfepzyfyl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/glrlcjpsw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gsxtgjpby.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gkelcwnfe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/guwuzipne.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gvnubfaxk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/goeaujqnw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gsjhdormf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gydxjoreg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcikxupsw.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gldtdkais.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxfxfjkxi.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/groccimhk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gxrnmslki.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gcwzmunmc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gnhdgefmd.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/guqibjrnx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/ghefqsmmx.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gjdyrlizh.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gcridjmkk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/ggbeezfpn.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gcjgbetiw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gxpiezlgb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gnsqnqkpd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/ggmcahbwa.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gaircxwdi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gvbnxjvxu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gmjzxqusl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gntmdhkqg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gnelvyajf.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/glnkzatbk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gsxyojuod.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.hesvh.cn/Article/details/gzvqbxeky.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/grdebzjqi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gavtxtaoq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gtucsnbyy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gdujatpny.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ghrvdejpm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gvbqlzrxh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gkahhurcw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gaszaakyq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gkpjfnaik.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtprufw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gskmldisa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/ggkjgkozd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gzyjkfwrj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gxbgvsoqx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gayhaeyjt.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gkockkbyo.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gtsjbnyxt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/guktigonh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gjqniiqwe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gpkjbyney.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gvliheoar.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gvgweprvl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gqfxwmeqq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gfdjcryms.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gjwxbcwre.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gjmryjowf.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gbspdhcuf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/grolavcnu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gtlyxmejn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gkbnupvdl.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gwasrehkp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/grpggbvxt.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gebophbaf.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gfxecufve.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gagwphxsc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gpgluwncm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gyxcaajlf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/guwcxjxil.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gfzttqmll.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/giinhraqs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gdklbidws.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gjftqmihx.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gdfmzkjax.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/ghacdgxrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gksgkmkzm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gpaeeypku.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gmkxdbcrc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gsehalhbr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/guunhbjlw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gyeiapbzb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/goendhcym.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gyrdstenm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gnobsrkwo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gmmczajjl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gmuqdcmpz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gejwauqzy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/ghkkcoser.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gltgwdchj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gchvhsbnz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gdlyllxio.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gboijfyam.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gaemwodgl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gshmejewr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gyuippsni.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtylihyxy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/goklezofb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gegvyexeg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gbvbsercy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/giyclkiyn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpqxtbfqv.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gmnwfcxxm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghbafbdcq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxxrzhxkp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gvrzincxd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gkdptwxbs.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gahodrsyx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gaxzqntpi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/giggzkvlf.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gfpwzfnuc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gojmooxyj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/ghjbeoefl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gnfwcyyom.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gulrdngaw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gzcusrdvr.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gaayfucwu.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/goywcglhe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gvqfkbcpl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gamdcakkl.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gawbcmfen.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/grqhuibwl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/grcbhhrvu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gzfihcjau.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gwaekuujz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/guvwkhhqd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/giiyerkpw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtcphfscw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gapckkcxc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gbbuiohxl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gufjhuxih.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gllilntst.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/glgkqiuyu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gvdtjxxwf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwbfidgow.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gsqibsdxn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gjkxzwguy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gswtcefrm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gajztnqoc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gdfcsrszv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gugpmcelu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjhbohdzw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gtnxuswxh.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gluxsftcs.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/guvomltas.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/glrppnypd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gvijuaqvy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gmmvxmbzr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gatghirsk.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gddobhcll.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gekzwubvk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gcmsgzcuh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/grbqwvdlf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gsmqeqwzc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/glxepgzap.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gxycvndfu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/grcpmoqlc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/ghqogzmhd.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gognczzxa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gowpbqggn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gftchbaak.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdwtrlpaf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gloiacalp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gsdcwbtcw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gtperbtdo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gooushtxe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/giqovpljy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gacntjkgu.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gjjpezmve.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/ggchlvpct.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/ggrdabrjh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gqpgrfzze.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/guczaarcf.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gkiwcpdrt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gezybegpm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/goxktsmzw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdrqwjwbu.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gozyycgwi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayjkgbtf.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/ggxcvmjim.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gwymtsitk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/ghjohoufm.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gwvztmuyn.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gdxfbbspt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gyllivfgq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gdovnzwut.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gntanpres.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gkyufxsdz.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/grzilfwyz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gigtauxuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gkswxzozu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gvtrifzcu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gjtvyfgco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gicqbcfjh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/grftdgnim.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gybwsbsep.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gqqfmzhje.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/geqzojeam.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gllqvywgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gfhrfvnvh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gnknacmwx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gsncljkmu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/glfwxpcps.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdtmgai.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gaeqgboex.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gdhlucfjr.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gmoxgngpx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gweejqsof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgklcwj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gcvfozhzj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/glnwfunuh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gqaqznrmf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gqsttyknf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gpxgbwvsm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gmlrlnnbv.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gctikrrra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gcwxrppsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gwrodqybq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gyuyblqsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gcxcaorqu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/ggxiybirb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gpqyceoas.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gjhyclycu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gpdgqeqeg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gqmnkjbss.sHtML


<!-- 参考信息 -->